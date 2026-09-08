# Atölyeler

Yaptığımız atölyelerin materyalleri ve notları.

Her atölye kendi klasöründe: `YYYY-AA-GG-etkinlik-adi/`
Tarihi başa yazmak dosyaların kronolojik sıralanmasını sağlar.

_Henüz yayımlanmış bir atölye kaydı yok. İlk atölyeden sonra buraya eklenecek._

---

## Standart atölye akışımız

Aşağıdaki akış her etkinlikte kullanabileceğimiz temel şablon. Etkinliğe göre süre ve
sıra değişir; klasörünü açarken bu akışı kopyalayıp o etkinliğe uyarlayın.

### Künye

| | |
|---|---|
| Süre | 30–45 dakika |
| Katılımcı | Ön bilgi gerekmez |
| Gereken | Kendi cihazı (dizüstü, tablet veya telefon) |
| Araçlar | [Strudel](https://strudel.cc) (müzik) + [Hydra](https://hydra.ojack.xyz) (görsel) |
| Kurulum | Yok — ikisi de tarayıcıda çalışır |

Strudel'in mobil uygulaması da var; masaüstünde doğrudan [strudel.cc](https://strudel.cc)
açılıyor. Kurulum istememek bilinçli bir tercih: 30 dakikalık bir atölyede kurulumla
uğraşmak zamanın yarısını yer.

### Nasıl anlatıyoruz

Canlı kodlama, yazılımı çalışırken değiştirerek müzik ve görsel üretmek demek. Kod
durdurulup yeniden başlatılmıyor — bir satır değişip çalıştırıldığı anda ses değişiyor.

Katılımcı üç şey yapıyor: bir satır yazıyor, çalıştırıyor, duyduğunu değiştiriyor.
Nota bilgisi ya da kod deneyimi gerekmiyor; ilk beş dakikada herkesin bir ritmi oluyor.

### Akış — 45 dakika

| Süre | Bölüm | İçerik |
|---|---|---|
| 5 dk | **Giriş** | Canlı kodlama nedir, algorave nedir, neden ekranı gösteriyoruz |
| 10 dk | **İlk ses** | Strudel'i açma, `sound("bd")`, örüntü kurma, hızlandırma |
| 10 dk | **Ritim** | Katmanlama, öklidyen ritim, seyreltme |
| 10 dk | **Görsel** | Hydra ile ilk şekil, sese tepki veren görsel |
| 10 dk | **Serbest** | Katılımcılar kendi parçalarını kuruyor, isteyen paylaşıyor |

### Akış — 30 dakika

Süre kısalırsa **Hydra bölümünü tamamen çıkarın**, kalan zamanı ritim ve serbest bölüme
dağıtın. İkisini birden yarım bırakmaktansa müziğe odaklanmak daha iyi sonuç veriyor.

| Süre | Bölüm |
|---|---|
| 5 dk | Giriş |
| 10 dk | İlk ses |
| 8 dk | Ritim |
| 7 dk | Serbest |

Materyal: [`../baslangic/`](../baslangic/) klasöründeki örnekler bu akışın yazılı hâli.
Katılımcılar atölyeden sonra oradan devam edebilir.

---

## Hazırlık listesi

- [ ] Mekânda kablosuz ağ var mı, kaç kişiyi kaldırıyor?
- [ ] Projeksiyon veya ekran
- [ ] Ses sistemi ve kablo
- [ ] Yedek cihaz — cihazı olmayan katılımcı için
- [ ] Kısa bağlantı ya da QR kod, `strudel.cc` hızlı açılsın
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
- Uygulanan akış (yukarıdakinden farklıysa)
- **Ne tuttu, ne tutmadı** — hangi bölüm uzun geldi, hangi soru tekrar tekrar geldi

Son madde en değerlisi. Bir sonraki atölyeyi hazırlayan kişi — muhtemelen yine siz —
bunu okuyacak.
