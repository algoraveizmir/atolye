# Canlı Kodlama Sözlüğü

Canlı kodlama terimlerinin Türkçe açıklamaları.

**Bu sözlük terimleri Türkçeleştirmeyi dayatmıyor.** Pratikte kod yazarken İngilizce
terimleri kullanacaksınız — fonksiyonun adı `sound`, `fast`, `euclid`. Buradaki amaç
terimin **ne olduğunu** Türkçe anlatmak ve konuşurken kullanabileceğiniz bir karşılık
önermek.

Önerilen karşılıklar tartışmaya açıktır. Daha iyisini biliyorsanız
[issue açın](../../issues).

---

## Temel kavramlar

### live coding · canlı kodlama
Yazılımı çalışırken değiştirerek performans yapmak. Kod durdurulup yeniden başlatılmaz;
siz yazdıkça ses ve görüntü anında değişir.

### algorave
Canlı kodlamayla üretilen müziğin dans edilerek dinlendiği etkinlik.
*Algorithm* + *rave*. 2011'de Londra'da doğdu.

### pattern · örüntü
Canlı kodlamanın temel birimi. Zaman içinde tekrar eden bir olaylar dizisi — bir ritim,
bir nota dizisi, bir renk değişimi. "Pattern yazmak" bu alanda "beste yapmak"ın karşılığı.

### cycle · döngü
Örüntünün bir turu. Canlı kodlamada zaman saniyeyle değil döngüyle ölçülür: "bu örüntü
bir döngüde dört kez çalsın" dersiniz, döngünün kaç saniye sürdüğünü ayrı ayarlarsınız.

### cps — cycles per second · saniyedeki döngü
Tempo ölçüsü. Geleneksel BPM'in (dakikadaki vuruş) yerini alır.
`cps = 0.5` → bir döngü iki saniye sürer.

### sample · örneklem, ses örneği
Önceden kaydedilmiş kısa ses dosyası — bir davul vuruşu, bir nefes, bir çarpma.
Canlı kodlamada çoğu ses bu dosyaların tetiklenmesiyle üretilir.

### synth · sentezleyici
Kayıt kullanmadan sesi sıfırdan üreten yapı. Sample hazır sesi çalar, synth sesi hesaplar.

---

## Örüntü kurma

### euclidean rhythm · öklidyen ritim
Belirli sayıda vuruşu belirli sayıda adıma olabildiğince eşit dağıtan yöntem.
`euclid(3,8)` → sekiz adıma üç vuruş. Dünya müziğindeki pek çok geleneksel ritim bu
formülle çıkar; bu yüzden canlı kodlamada çok kullanılır.

### polyrhythm · polikritim, çokritim
Aynı anda farklı uzunlukta örüntülerin çalması. Üçlü bir örüntüyle dörtlü bir örüntü
üst üste bindiğinde on iki döngüde bir başa döner.

### stack · yığın
Birden fazla örüntüyü aynı anda çalmak. Katmanlama.

### cat / slowcat · sıralama
Örüntüleri arka arkaya çalmak. Yığının tersi: aynı anda değil, sırayla.

### rev · ters çevirme
Örüntüyü tersten çalmak.

### fast / slow · hızlandırma / yavaşlatma
Örüntüyü döngü içinde sıkıştırmak veya yaymak. `fast 2` → iki kat hızlı.

### degrade · seyreltme
Örüntüdeki olayların bir kısmını rastgele düşürmek. Makine gibi duran bir ritmi
insanileştirmek için kullanılır.

---

## Ses işleme

### gain · kazanç, ses seviyesi
Sesin yüksekliği.

### pan · yönlendirme
Sesin sağ-sol dengesi.

### lpf / hpf — low/high pass filter · alçak/yüksek geçiren süzgeç
Belirli frekansların üstünü veya altını kesen filtre. `lpf` tizleri keser, ses boğuklaşır;
`hpf` basları keser, ses inceleşir.

### reverb · yankı
Sesin bir mekânda çınlıyormuş gibi duyulmasını sağlayan efekt.

### delay · gecikme
Sesin belirli aralıklarla tekrar etmesi. Yankıdan farkı: tekrarlar ayrı ayrı duyulur.

---

## Araçlar ve ortam

### REPL — read-eval-print loop
Yazdığınız kodun anında çalıştırıldığı ortam. Strudel'in tarayıcıdaki editörü bir REPL'dir.

### evaluate · değerlendirme, çalıştırma
Yazdığınız satırı çalıştırmak. Genelde `Ctrl/Cmd + Enter`. Canlı kodlamada bu, bir
enstrümana dokunmanın karşılığıdır — her değerlendirme sesi anında değiştirir.

### hush · susturma
Çalan her şeyi durduran komut.

### boot · başlatma
Ortamı performansa hazır hâle getirme adımı.

### quark
SuperCollider'ın eklenti paketi. SuperDirt bir quark'tır.

---

## Topluluk

### TOPLAP
*Temporary Organisation for the Promotion of Live Algorithm Programming.* 2004'te
Hamburg'da kurulan, canlı kodlama topluluklarını birbirine bağlayan küresel ağ.
Algorave İzmir bu ağın kayıtlı bir üyesidir.

### node · düğüm
TOPLAP ağındaki yerel topluluk. Her node bağımsız çalışır; merkezi bir hiyerarşi yoktur.

### ICLC — International Conference on Live Coding
Canlı kodlamanın yıllık uluslararası akademik konferansı.

---

<!-- Yeni terim eklerken: başlığa İngilizce terimi yazın, varsa önerilen Türkçe
     karşılığı "·" ile ayırıp ekleyin, sonra iki üç cümleyle açıklayın.
     Terimleri bölüm içinde mantıklı bir sırayla dizin, alfabetik olmak zorunda değil. -->
