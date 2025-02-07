# Neden Temiz Kod Prensibini Uygulamalıyız? 
## 1. Kodun Okunabilirliğini ve Anlaşılabilirliğini Artırır:
Bir yazılımcı, bir projeye yeni başladığında veya başkası tarafından yazılmış bir kodu incelediğinde, tutarlı bir isimlendirme ve yapılandırma standardı sayesinde kodu hızlıca anlayabilir. Örneğin:

- PascalCase ile yazılmış sınıf ve metod isimleri, ne tür bir yapı olduğunu hemen anlamayı sağlar.
- camelCase ile yazılmış metod argümanları ve yerel değişkenler, işlevlerinin ne olduğunu anlamayı kolaylaştırır.
- Tutarsızlıklar ve karışıklıklar, zaman içinde kodun karmaşıklaşmasına ve geliştiricilerin hata yapmasına yol açabilir.

## 2. Ekip İçi İletişimi Güçlendirir:
Ekip içinde farklı yazılımcılar farklı yazım stilleri kullanırsa, bu durum yanlış anlamalara veya kafa karışıklığına yol açabilir. Aynı isimlendirme kuralları, tüm ekip üyelerinin yazdığı kodu daha hızlı anlamasına yardımcı olur.

Örneğin, bir yazılımcı orderTotal isminde bir değişken kullandığında, başka bir yazılımcı OrderTotal yazmışsa, bu iki değişkenin farklı işlevler taşıdığı düşünülerek yanlış anlaşılmalar yaşanabilir.
Standartlara uymak, ekip üyelerinin birbirlerinin kodunu çok daha kolay bir şekilde okuyup anlayabilmesini sağlar.

## 3. Hata Oranını Düşürür:
Kod yazımında tutarsızlıklar genellikle hatalara yol açar. Yanlış yazım veya isimlendirme farkları, özellikle büyük projelerde büyük sorunlar yaratabilir. Örneğin:

- Public alanlar için PascalCase kullanırken, Private alanlar için camelCase ile alt çizgi (_) eklemek, hangi alanın özel olduğunu anlamanızı sağlar. Eğer bu kurallar izlenmezse, bir geliştirici yanlışlıkla private bir alana dışarıdan erişmeye çalışabilir.
- Bu tür hataları en aza indirgemek için kodlama standartlarına uymak büyük bir avantaj sağlar.

## 4. Bakım Kolaylığı:
Yazılım projeleri genellikle zamanla büyür ve uzun süre devam eder. Bu süreçte, birçok yeni özellik eklenir ve mevcut kod üzerinde değişiklikler yapılır. Eğer kodun içinde tutarlı bir yapı varsa, bakım süreci çok daha kolay hale gelir. Mesela:

- Sabitler için belirlenen PascalCase isimlendirmesi, sabitlerin başka türdeki değişkenlerden hemen ayrılmasını sağlar.
- Eğer her geliştirici farklı bir isimlendirme tarzı kullanırsa, mevcut kodda değişiklik yaparken hata yapma olasılığı artar.
- İyi bir isimlendirme ve yapılandırma, yazılımın uzun süre sürdürülebilir olmasına katkı sağlar.

## 5. Kodun Geliştirilebilirliğini Artırır:
- Proje büyüdükçe yeni özellikler eklenir. Yeni geliştiriciler katıldığında, projenin nasıl organize edildiğini ve kodun nasıl işlediğini anlamak için tutarlı bir yapı gerekir.

- Eğer belirli kurallara ve standartlara uyulmuşsa, yeni bir özellik eklemek veya mevcut bir özellik üzerinde değişiklik yapmak daha hızlı ve hatasız yapılabilir.
Kodun tutarlı olması, yazılımcıların yazdıkları kodu daha iyi entegre etmesine ve projeyi hızlıca geliştirmesine olanak tanır.

## 6. Endüstri Standartlarına Uygunluk:
Birçok yazılım projesi endüstri standartlarına dayanır ve bu standartlar, projeyi daha profesyonel ve sürdürülebilir hale getirir. C# gibi dillerin kendi içinde kabul edilen isimlendirme kuralları vardır ve bu kurallara uymak:

Diğer geliştiricilerle işbirliği yaparken daha verimli olmanızı sağlar.
Open Source projelerinde ya da büyük projelerde çalışırken kodun daha anlaşılır olmasını sağlar.
Bunların yanında, bu standartlara uymak yazılım geliştirme sürecini daha sistemli hale getirir.

# C-sharp---Coding-Standards(EN)
| **Object Name**        | **Notation** | **Length** | **Plural** | **Prefix** | **Suffix** | **Abbreviation** | **Char Mask** | **Underscores** |
|------------------------|--------------|-------------|------------|------------|------------|------------------|---------------|-----------------|
| **Namespace name**      | PascalCase   | 128         | Yes        | Yes        | No         | No               | [A-z][0-9]     | No              |
| **Class name**          | PascalCase   | 128         | No         | No         | Yes        | No               | [A-z][0-9]     | No              |
| **Constructor name**    | PascalCase   | 128         | No         | No         | Yes        | No               | [A-z][0-9]     | No              |
| **Method name**         | PascalCase   | 128         | Yes        | No         | No         | No               | [A-z][0-9]     | No              |
| **Method arguments**    | camelCase    | 128         | Yes        | No         | No         | Yes              | [A-z][0-9]     | No              |
| **Local variables**     | camelCase    | 50          | Yes        | No         | No         | Yes              | [A-z][0-9]     | No              |
| **Constants name**      | PascalCase   | 50          | No         | No         | No         | No               | [A-z][0-9]     | No              |
| **Field name (Public)** | PascalCase   | 50          | Yes        | No         | No         | Yes              | [A-z][0-9]     | No              |
| **Field name (Private)**| _camelCase   | 50          | Yes        | No         | No         | Yes              | _[A-z][0-9]    | Yes             |
| **Properties name**     | PascalCase   | 50          | Yes        | No         | No         | Yes              | [A-z][0-9]     | No              |
| **Delegate name**       | PascalCase   | 128         | No         | No         | Yes        | Yes              | [A-z]          | No              |
| **Enum type name**      | PascalCase   | 128         | Yes        | No         | No         | No               | [A-z]          | No              |

## C# Kodlama Standartları ve İsimlendirme Konvansiyonları (TR)
| **Nesne Adı**          | **Notasyon** | **Uzunluk** | **Çoğul** | **Önek** | **Sonek** | **Kısaltmalar** | **Karakter Maskesi** | **Alt Çizgi** |
|------------------------|--------------|-------------|-----------|----------|-----------|-----------------|----------------------|---------------|
| **Namespace adı**       | PascalCase   | 128         | Evet      | Evet     | Hayır     | Hayır           | [A-z][0-9]           | Hayır         |
| **Sınıf adı**           | PascalCase   | 128         | Hayır     | Hayır    | Evet      | Hayır           | [A-z][0-9]           | Hayır         |
| **Yapıcı adı (Constructor)** | PascalCase | 128 | Hayır | Hayır | Evet | Hayır | [A-z][0-9] | Hayır |
| **Metod adı**           | PascalCase   | 128         | Evet      | Hayır    | Hayır     | Hayır           | [A-z][0-9]           | Hayır         |
| **Metod argümanları**   | camelCase    | 128         | Evet      | Hayır    | Hayır     | Evet            | [A-z][0-9]           | Hayır         |
| **Yerel değişkenler**   | camelCase    | 50          | Evet      | Hayır    | Hayır     | Evet            | [A-z][0-9]           | Hayır         |
| **Sabitler adı**        | PascalCase   | 50          | Hayır     | Hayır    | Hayır     | Hayır           | [A-z][0-9]           | Hayır         |
| **Alan adı (Public)**   | PascalCase   | 50          | Evet      | Hayır    | Hayır     | Evet            | [A-z][0-9]           | Hayır         |
| **Alan adı (Private)**  | _camelCase   | 50          | Evet      | Hayır    | Hayır     | Evet            | _[A-z][0-9]          | Evet          |
| **Özellikler adı**      | PascalCase   | 50          | Evet      | Hayır    | Hayır     | Evet            | [A-z][0-9]           | Hayır         |
| **Delegat adı**         | PascalCase   | 128         | Hayır     | Hayır    | Evet      | Evet            | [A-z]                | Hayır         |
| **Enum türü adı**       | PascalCase   | 128         | Evet      | Hayır    | Hayır     | Hayır           | [A-z]                | Hayır         |

## 1. Namespace name (Ad alanı adı)
- Notasyon: PascalCase
- Örnek: MyApplication.Data
- Namespace, genellikle büyük projelerde kategorilere göre düzenlenmiş dosyalar ve sınıflar için kullanılır. Bu örnek, uygulamanın veri ile ilgili sınıflarını barındıran bir namespace’i ifade eder.
## 2. Class name (Sınıf adı)
- Notasyon: PascalCase
- Örnek: CustomerManager
- Bu sınıf adı, müşteri yönetimini sağlayan bir sınıfı temsil eder. PascalCase kullanımı, sınıfların isimlerinin her kelimesinin büyük harfle başlamasını sağlar.
## 3. Constructor name (Yapıcı adı)
- Notasyon: PascalCase
- Örnek: CustomerManager()
- Bu, CustomerManager sınıfının yapıcı metodudur. Yapıcılar sınıfın örneği oluşturulurken çağrılır ve genellikle sınıf adıyla aynı adı taşır.
## 4. Method name (Metod adı)
- Notasyon: PascalCase
- Örnek: CalculateDiscount()
- Metodlar, genellikle bir işlevi yerine getiren ve PascalCase ile yazılan fonksiyonlardır. Bu örnekte, "indirim hesaplama" işlevini yerine getiren bir metodun adı verilmiştir.
## 5. Method arguments (Metod argümanları)
- Notasyon: camelCase
- Örnek: calculateDiscount(double originalPrice)
- Metod argümanları genellikle camelCase ile yazılır. Bu örnekte, originalPrice bir argümandır ve küçük harf ile başlanmıştır.
## 6. Local variables (Yerel değişkenler)
- Notasyon: camelCase
- Örnek: int discountAmount
- Yerel değişkenler genellikle küçük harf ile başlar ve camelCase stiline uyar. Bu örnekte, discountAmount yerel bir değişkendir.
## 7. Constants name (Sabitler adı)
- Notasyon: PascalCase
- Örnek: MaxDiscountRate
- Sabitler genellikle PascalCase ile yazılır. Bu örnekte, MaxDiscountRate sabiti en yüksek indirim oranını temsil eder.
## 8. Field name (Public) (Alan adı - Public)
- Notasyon: PascalCase
- Örnek: public int customerCount
- Public alanlar genellikle PascalCase kullanılarak yazılır. Bu örnekte, müşteri sayısını tutan bir alan örneği gösterilmiştir.
## 9. Field name (Private) (Alan adı - Private)
- Notasyon: _camelCase
- Örnek: private string _customerName
- Private alanlar genellikle alt çizgi (_) ile başlar ve camelCase ile yazılır. Bu örnekte, bir müşterinin adını tutan bir private alan gösterilmiştir.
## 10. Properties name (Özellikler adı)
- Notasyon: PascalCase
- Örnek: public string CustomerName { get; set; }
- Özellikler (properties), genellikle PascalCase ile yazılır. Bu örnekte, bir müşterinin adını tutan özellik gösterilmiştir.
## 11. Delegate name (Delegat adı)
- Notasyon: PascalCase
- Örnek: public delegate void DiscountAppliedEventHandler()
- Delegatlar, bir işlevi temsil eden türlerdir ve genellikle PascalCase kullanılarak yazılır. Bu örnekte, bir "indirim uygulandı" olayını temsil eden delegat adı verilmiştir.
## 12. Enum type name (Enum türü adı)
- Notasyon: PascalCase
- Örnek: public enum DiscountType { Percentage, Amount }
- Enum türleri de PascalCase kullanılarak yazılır. Bu örnekte, bir indirim türünü temsil eden enum gösterilmiştir.

# Summary  
< summary > etiketi, özellikle C# gibi programlama dillerinde, XML yorumları (XML comments) içerisinde kullanılan ve bir metodun, sınıfın, özelliğin veya başka bir yapının ne işe yaradığını açıklayan bir etikettir. Bu etiket, kodun okunabilirliğini artırmak ve yazılım belgelerini oluşturmak için yaygın bir yöntemdir. 
Kullanmak için 3 adet /// eğik çizgi (slash) olarak kullanılır. 
## Ne zaman kullanılır?
- <summary> etiketi, genellikle metodların, sınıfların, özelliklerin ve diğer yapıların açıklamalarını eklemek için kullanılır. Bu, başkalarının (veya sizin) yazdığınız kodu anlamasını kolaylaştırır. Ayrıca, bu etiketler IntelliSense (Visual Studio'da veya başka bir IDE'de kullanılan kod tamamlama aracında) gibi araçlar tarafından okunarak otomatik dokümantasyon sağlar. 
- Kodun daha okunabilir ve kodun karmaşık görüntülenmesi önüne geçmek için kullanılır. 

## Örnek Kullanım
![Ekran Görüntüsü (314)](https://github.com/user-attachments/assets/42dc150a-e7d3-43fb-80cc-6b504026887a)

## Yukarıdaki örnekte:
- < summary > etiketi, metodun genel amacını açıklar.
- < param > etiketi, metodun aldığı parametreleri açıklar.
- < returns > etiketi, metodun döndürdüğü değeri açıklar.  
![Ekran Görüntüsü (316)](https://github.com/user-attachments/assets/e7e1046f-301a-4cc8-ac84-689f09c9dd26)
![Ekran Görüntüsü (315)](https://github.com/user-attachments/assets/9413ac8b-9070-4a15-8da8-46025d0bd8c6)

## Avantajları:
- Kodun Anlaşılabilirliğini Arttırır: Başka bir yazılımcı kodunuzu incelediğinde, kodun ne amaçla yazıldığını ve nasıl kullanıldığını hızlıca anlayabilir.
- Auto-Documentation (Otomatik Belgeleme): XML yorumları, dokümantasyon araçları tarafından otomatik olarak işlenebilir. Böylece kodunuzdan otomatik belgeler oluşturulabilir.
- IDE Desteği: Visual Studio ve diğer IDE'ler, XML yorumlarını tanıyıp, geliştiricilere IntelliSense önerileri sunar.

# Önemli Noktalar:
- Gereksiz Yorumlardan Kaçının: summary açıklamalarını yalnızca kodun gerçekten karmaşık olduğu veya başkaları tarafından sıklıkla kullanılacağı yerlerde kullanmak iyi bir uygulamadır. Kendi kendini açıklayan kodlar için gereksiz açıklamalardan kaçının.
- Doğru ve Kapsamlı Olun: Yorumlar, doğru ve anlamlı olmalı. Kodu açıklamaya çalışırken, kodun mantığı ve işlevi hakkında yanlış bilgi vermemek önemlidir.

# Ne Zaman Kullanılmamalı?
- Eğer kod oldukça açık ve anlaşılırsa, summary yorumları eklemek gereksiz olabilir. Bu tür yorumlar yalnızca gerekli olduğunda kullanılmalıdır.
- Basit Yapılar İçin: Bir değişken veya basit bir metod için açıklama eklemek genellikle gereksizdir. Kodun kendisi zaten yeterince açık olabilir.
