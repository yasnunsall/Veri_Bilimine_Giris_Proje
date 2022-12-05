## Makine Öğrenimi Nedir ?


Makine Öğrenmesi, bilgisayarların tıpkı insanlar gibi elde ettikleri verilerden çıkarım yapıp algoritma
ve modeller oluşturmasını sağlayan bilim dalıdır. Bu algoritmalar sayesinde bilgisayar belirli bir
veri kümesinden sonuçları daha doğru tahmin edebilir. Örneğin çok sayıda tarama görüntüsü ve bunların
raporlarını kullanarak modelimizi kanserleri teşhis edecek şekilde eğitebiliriz. 

---

## Makine Öğrenimi Nasıl Çalışır ?


Makine Öğrenimi'nde temel mantık elimizdeki verilerin girdi ve çıktıları arasındaki ilişkilerle 
bir fonksiyon oluşturmaktır. Kabul edelimki elimizde mxn boyutlu girdi ve mx1 boyutlu çıktı(etiket) olsun. 
Fonksiyonumuz f olsun. O halde fonksiyonumuzun girdisi n-boyutlu ve çıktısı ise 1-boyutlu olacaktır.
Başlangıç için f fonksiyonunun katsayılarını random şekilde belirliyoruz. İlk verimiz x11,x12,...,x1n ve
etiketi de b1 olsun. f fonksiyonumuzun katsayılarına da a1,a2,...,an diyelim. İlk verimizi fonksiyona sokarız ve
b1' çıktısını elde ederiz. ( f(x11,x12,...,x1n) = x11.a1 + x12.a2 + ... + x1n.an = b1' ). Bundan sonra
sürece loss fonksiyonu [ e(bn, bn') ] dahil oluyor. Loss fonksiyonu f fonksiyonunun çıktısını ve gerçek
etiketi karşılaştırarak her bir iterasyonda f fonksiyonunun katsayılarının güncellenmesine yardımcı olur.
Bu şekilde m iterasyon sonunda tüm veriler kullanılır ve model hazırlanmış olur. 

---

## Makine Öğrenimi Türleri Nelerdir ?

Makine Öğrenimi girdi ve çıktı türüne bağlı olarak 4 ayrı gruba ayrılabilir :

### 1. Denetimli Makine Öğrenimi

Etiketli veriler kullanılarak modelin eğitilmesine Denetimli Makine Öğrenimi denir. Örneğin yüzlerce
kedi ve köpek fotoğrafının bulunduğu bir veri seti...

### 2. Denetimsiz Makine Öğrenimi

Etiketsiz veriler kullanılarak modelin eğitilmesine Denetimli Makine Öğrenimi denir. Peki etiketsiz
veriler nasıl eğitilir ? Burada karşımıza kümelendirme algoritmaları çıkıyor. Burada bilgisayar
verileri yorumlar ve en anlamcı olacak şekilde verileri kümelere ayırır. Örneğin etiketsiz kedi
ve köpek resimlerinin ayırt edici özellikleri sayesinde kümelere ayrılması...

### 3. Yarı denetimli öğrenme

Denetimli ve denetimsiz öğrenmenin bir arada kullanıldığı öğrenmedir. İlk önce etiketli verilerle 
model kısmen eğitilir. Sonra etiketsiz veri bu modelle eğitilir ve etiketlenir. En sonunda iki
veri karıştırılır ve model yeniden eğitilir.

### 4. Pekiştirmeli öğrenme

Pekiştirmeli Öğrenme her bir adımda ceza ve ödülün verildiği öğrenim türüdür. Bu öğrenimde modelin
amacı mümkün olduğunca fazla ödül puanı almaktır. Video oyunları denetimsiz öğrenmenin en çok kullanıldığı
alanlardan biridir. 


