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

# C-sharp---Coding-Standards
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

C# Kodlama Standartları ve İsimlendirme Konvansiyonları
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

Örnek  
1. Namespace Name (Ad Alanı)
Notasyon: PascalCase
Uzunluk: 128 karaktere kadar
Çoğul: Evet
Önek: Evet
Ayrıca: Abbr. kullanılmaz, alt çizgi yok.

namespace MyApplication.Utilities
{
    // Burada 'MyApplication.Utilities' bir namespace ismi olup PascalCase kullanılmıştır.
}
