# Atölyeler

Yaptığımız atölyelerin materyalleri ve notları.

Her atölye kendi klasöründe: `YYYY-AA-GG-etkinlik-adi/`
Tarihi başa yazmak dosyaların kronolojik sıralanmasını sağlar.

_Henüz yayımlanmış bir atölye kaydı yok. İlk atölyeden sonra buraya eklenecek._

---

## Standart atölye akışımız

Her etkinlikte kullanabileceğimiz temel şablon. Klasörünü açarken bu akışı kopyalayıp
o etkinliğe uyarlayın.

### Künye

| | |
|---|---|
| Süre | 60 dakika (30 dk ses + 30 dk görsel) |
| Katılımcı | Ön bilgi gerekmez |
| Gereken | Kendi cihazı — dizüstü, tablet veya telefon |
| Araçlar | [Strudel](https://strudel.cc) (ses) + [Hydra](https://hydra.ojack.xyz) (görsel) |
| Kurulum | Yok — ikisi de tarayıcıda çalışır |

Strudel'in mobil uygulaması da var; masaüstünde doğrudan [strudel.cc](https://strudel.cc)
açılıyor. Kurulum istememek bilinçli bir tercih: kısa bir atölyede kurulumla uğraşmak
zamanın yarısını yer.

### Nasıl anlatıyoruz

Canlı kodlama, yazılımı çalışırken değiştirerek müzik ve görsel üretmek demek. Kod
durdurulup yeniden başlatılmıyor — bir satır değişip çalıştırıldığı anda ses değişiyor.

Katılımcı üç şey yapıyor: bir satır yazıyor, çalıştırıyor, duyduğunu değiştiriyor.
Nota bilgisi ya da kod deneyimi gerekmiyor; ilk beş dakikada herkesin bir ritmi oluyor.

---

## Akış — 60 dakika

### Birinci yarı: Ses · Strudel (30 dk)

| Süre | Bölüm | İçerik |
|---|---|---|
| 5 dk | **Giriş** | Canlı kodlama nedir, algorave nedir, neden ekranı gösteriyoruz |
| 5 dk | **İlk ses** | `strudel.cc`'yi açma, `sound("bd")`, çalıştırma, `hush` |
| 8 dk | **Örüntü** | Boşlukla ayırma, `~` sessizlik, `fast` / `slow` |
| 7 dk | **Ritim** | `stack` ile katmanlama, `euclid` ile öklidyen ritim |
| 5 dk | **Ses işleme** | `lpf`, `room`, `gain` — sayıları değiştirip dinleme |

Bu bölümün sonunda herkesin çalan bir ritmi olmalı. Olmayan varsa devam etmeyin,
o kişiye dönün — ikinci yarıya ses olmadan geçilmiyor.

### İkinci yarı: Görsel · Hydra (30 dk)

| Süre | Bölüm | İçerik |
|---|---|---|
| 5 dk | **Geçiş** | `hydra.ojack.xyz`'i açma, ikinci sekmede çalıştığını gösterme |
| 7 dk | **İlk şekil** | `osc()`, `noise()`, `shape()` — tek satırla ekranı doldurma |
| 8 dk | **Dönüştürme** | `.rotate()`, `.kaleid()`, `.color()` zincirleme |
| 10 dk | **Sesle birleştirme** | Hydra'yı mikrofondan gelen sese tepki verecek şekilde bağlama; Strudel sekmesi çalarken görselin oynaması |

Son bölüm atölyenin doruk noktası: katılımcı kendi yazdığı sesin kendi yazdığı görseli
oynattığını görüyor.

### Kapanış

Kalan 2–3 dakikada bu deponun adresini gösterin: katılımcı evde
[`../baslangic/`](../baslangic/) klasöründen devam edebilir.

---

## Akış — 30 dakika

Süre yarıya inerse **Hydra'yı tamamen çıkarın**, sadece Strudel yapın. İkisini birden
yarım bırakmaktansa sese odaklanmak çok daha iyi sonuç veriyor.

| Süre | Bölüm |
|---|---|
| 5 dk | Giriş |
| 8 dk | İlk ses |
| 10 dk | Örüntü ve ritim |
| 7 dk | Serbest — katılımcılar kendi parçasını kuruyor |

---

## Hazırlık listesi

- [ ] Mekânda kablosuz ağ var mı, kaç kişiyi kaldırıyor?
- [ ] Projeksiyon veya ekran
- [ ] Ses sistemi ve kablo
- [ ] Yedek cihaz — cihazı olmayan katılımcı için
- [ ] Kısa bağlantı ya da QR kod, `strudel.cc` hızlı açılsın
- [ ] Hydra'nın mikrofon izni: tarayıcı soracak, önceden deneyin
- [ ] Bu deponun adresi görünür bir yerde

---

## Yeni atölye klasörü açarken

```
atolyeler/2026-01-01-etkinlik-adi/
  README.md
```

`README.md` içine şunları yazın:

- Etkinlik adı, tarih, mekân
- Kaç kişi katıldı
- Uygulanan akış — yukarıdakinden farklıysa
- **Ne tuttu, ne tutmadı** — hangi bölüm uzun geldi, hangi soru tekrar tekrar geldi

Son madde en değerlisi. Bir sonraki atölyeyi hazırlayan kişi — muhtemelen yine siz —
bunu okuyacak.
