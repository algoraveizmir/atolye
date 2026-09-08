# Kurulum

**Kısa yol: hiçbir şey kurmayın.**

[strudel.cc](https://strudel.cc) ve [hydra.ojack.xyz](https://hydra.ojack.xyz) tarayıcıda
çalışır. Telefonda bile açılır. Atölyelerimizde bunları kullanıyoruz — kimse kurulumla
uğraşmasın diye.

Aşağısı, kendi bilgisayarınızda **TidalCycles** kurmak isteyenler için. Sahne
performanslarımızda bunu kullanıyoruz.

> Komutlar sürümden sürüme değişiyor. Buraya sabit komut yazmak yerine mantığı anlatıyoruz;
> güncel adımlar için her zaman resmî kaynağa bakın:
> **[tidalcycles.org/docs/getting-started/installation](https://tidalcycles.org/docs/getting-started/installation)**

---

## Neyin neye bağlı olduğu

TidalCycles tek başına ses çıkarmaz. Zincir şöyle işler:

```
Editörünüz  →  TidalCycles  →  (OSC mesajları)  →  SuperDirt  →  SuperCollider  →  hoparlör
   (kod)        (Haskell)                          (quark)      (ses motoru)
```

Bu yüzden dört parça kurmanız gerekiyor:

1. **SuperCollider** — ses motoru
2. **sc3-plugins** — bazı efektlerin ihtiyaç duyduğu ek UGen'ler
3. **SuperDirt** — SuperCollider içine kurulan quark; sample'ları çalar
4. **TidalCycles** — Haskell kütüphanesi

Bir de kod yazacağınız **editör eklentisi**.

---

## Kurulum sırası

Sıra önemli — SuperCollider olmadan SuperDirt kurulamaz.

### 1. SuperCollider

[supercollider.github.io/downloads](https://supercollider.github.io/downloads)

### 2. sc3-plugins

[supercollider.github.io/sc3-plugins](https://supercollider.github.io/sc3-plugins/) —
SuperCollider'ın eklenti klasörüne kopyalanır.

### 3. SuperDirt

SuperCollider'ı açın, şu satırın üzerindeyken `Cmd/Ctrl + Enter`:

```supercollider
Quarks.checkForUpdates({Quarks.install("SuperDirt", "v1.7.3")});
```

Birkaç dakika sürer. Bitince SuperCollider'ı yeniden başlatın.

> Sürüm numarası zamanla değişir; güncelini
> [SuperDirt deposundan](https://github.com/musikinformatik/SuperDirt) kontrol edin.

### 4. TidalCycles

Tidal bir Haskell kütüphanesi, önce **GHCup** (Haskell araç zinciri) gerekiyor.
Resmî kurulum sayfasında macOS, Linux ve Windows için ayrı ayrı anlatılıyor.

### 5. Editör

Atom artık geliştirilmiyor. Güncel seçenekler:

- **[Pulsar](https://pulsar-edit.dev/)** — Atom'un devamı, `tidalcycles` paketiyle
- **[VS Code](https://code.visualstudio.com/)** — `vscode-tidalcycles` eklentisiyle
- **Vim / Neovim** — `vim-tidal`
- **Emacs** — `tidal.el`

---

## Her oturumda

1. SuperCollider'ı açın, çalıştırın:
   ```supercollider
   SuperDirt.start
   ```
2. Editörünüzde Tidal'ı başlatın (boot)
3. Satırları tek tek değerlendirin — `Cmd/Ctrl + Enter`
4. Susturmak için: `hush`

---

## Sık karşılaşılan sorunlar

**Ses gelmiyor, hata da yok**
SuperCollider'da `SuperDirt.start` çalıştırıldı mı? Sistem ses çıkışı doğru cihazda mı?

**`Command not found: ghc` / `cabal`**
Haskell araç zinciri PATH'e eklenmemiş. Terminali kapatıp açın; sürerse GHCup kurulumunu
gözden geçirin.

**Editör "Tidal: boot failed" diyor**
Tidal kütüphanesi kurulu değil ya da eklenti GHC'yi bulamıyor. Eklenti ayarlarında
`ghci` yolunu elle vermeniz gerekebilir.

**`SuperDirt` bulunamıyor**
Quark kurulduktan sonra SuperCollider yeniden başlatılmadı.

---

<!-- Kendi yaşadığınız sorunları ve çözümlerini buraya ekleyin —
     bir sonraki kuran kişi için en değerli kısım burası olacak. -->
