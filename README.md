# Kepler Data Analysis

## Proje Amacı / Project Goal

Bu proje, **Kepler Teleskobu** tarafından sağlanan exoplanet verilerini kullanarak gezegenlerin yaşanabilirlik potansiyelini analiz etmeyi amaçlamaktadır. Veriler, gezegenlerin çeşitli fiziksel özelliklerine dayalı olarak analiz edilmiş ve görselleştirilmiştir. Projede gezegenlerin yaşanabilirlik skoru hesaplanmış, gezegenlerin özellikleri arasındaki ilişkiler görselleştirilmiş ve farklı gezegen adaylarının durumları üzerinde analizler yapılmıştır.

This project aims to analyze exoplanet data provided by the **Kepler Space Telescope**. The project focuses on evaluating the habitability potential of planets and visualizing the characteristics of different planet candidates. Key features such as **koi_score**, **koi_prad** (planet radius), and **koi_steff** (star temperature) are used to calculate the habitability scores of the planets, which are then visualized through various charts and plots.

---

## Yapılan Analizler ve Görselleştirmeler / Performed Analyses and Visualizations

### 1. Yaşanabilirlik Skoru Hesaplaması / Habitability Score Calculation

Gezegenlerin yaşanabilirliğini değerlendirmek için bir **yaşanabilirlik skoru** hesaplanmıştır. Bu skor şu parametrelere dayanır:
- **Gezegen Yarıçapı**: Yarıçapı 2'nin altındaki gezegenler daha yaşanabilir olarak değerlendirilmiştir.
- **Yıldız Sıcaklığı**: Yıldızın yüzey sıcaklığı 5300–6000 K arasında ise gezegenin yaşanabilirliği daha olası kabul edilmiştir.
- **Yörünge Süresi**: Yörünge süresi 200-400 gün arasında olan gezegenler daha yaşanabilir kabul edilmiştir.
- **Koi Skoru**: Koi skoru yüksek olan gezegenler, yaşanabilirlik açısından daha umut verici olarak değerlendirilmiştir.

A **habitability score** for planets has been calculated to assess their habitability. This score is based on the following parameters:
- **Planet Radius**: Planets with a radius less than 2 are considered more habitable.
- **Star Temperature**: Planets with a star surface temperature between 5300–6000 K are considered more likely to be habitable.
- **Orbital Period**: Planets with an orbital period between 200-400 days are considered more habitable.
- **Koi Score**: Planets with a high koi score are considered more promising in terms of habitability.

### 2. Yaşanabilir Gezegen Adaylarının Sayısı / Number of Viable Planet Candidates

Yaşanabilirlik skoru hesaplanan gezegenlerden yaşanabilirlik potansiyeline sahip olanlar (skoru yüksek olanlar) belirlenmiş ve bu gezegenlerin sayısı raporlanmıştır.

The planets with the highest habitability scores were identified, and the number of viable planet candidates was reported.

### 3. Gezegen Yarıçapı ve Yörünge Süresi Dağılımı (Scatter Plot) / Planet Radius vs. Orbital Period Distribution (Scatter Plot)

Gezegenlerin **yarıçapı** (koi_prad) ile **yörünge süresi** (koi_period) arasındaki ilişkiyi görselleştirmek amacıyla scatter plot kullanılmıştır. Bu görselleştirme gezegenlerin büyüklüğü ile yörüngelerinin süresi arasındaki ilişkiyi anlamaya olanak tanır.

A scatter plot was used to visualize the relationship between **planet radius** (koi_prad) and **orbital period** (koi_period). This visualization helps us understand the relationship between the size of planets and their orbital durations.

### 4. Yıldız Sıcaklığı ve Gezegen Yarıçapı Isı Haritası (Heatmap) / Star Temperature vs. Planet Radius Heat Map

**Yıldız sıcaklığı** (koi_steff) ile **gezegen yarıçapı** (koi_prad) arasındaki ilişkiyi göstermek için bir ısı haritası (heatmap) kullanılmıştır. Bu görselleştirme, yıldızların sıcaklıkları ile gezegenlerin büyüklükleri arasındaki korelasyonu görsel olarak sunar.

A heatmap was used to visualize the relationship between **star temperature** (koi_steff) and **planet radius** (koi_prad), showing the correlation between these two variables.

### 5. Gezegen Adaylarının Durum Dağılımı (Bar Chart) / Planet Disposition Distribution (Bar Chart)

Gezegen adaylarının durumları (CONFIRMED, CANDIDATE, FALSE POSITIVE) **koi_disposition** sütununa göre gruplanmış ve bar grafikler ile görselleştirilmiştir. Bu görselleştirme, gezegen adaylarının farklı durumlarını ve bu durumların sayısal dağılımını sunar.

The planet candidates' dispositions (CONFIRMED, CANDIDATE, FALSE POSITIVE) were grouped by the **koi_disposition** column and visualized using bar charts. This visualization provides insights into the distribution of planet candidates in different statuses.

### 6. Transit Süresi ve Işık Kaybı Dağılımı (Scatter Plot) / Transit Time vs. Light Loss Distribution (Scatter Plot)

Gezegenlerin **transit süresi** ile **ışık kaybı** arasındaki ilişkiyi incelemek için bir scatter plot kullanılmıştır. Bu görselleştirme, gezegenlerin transiti sırasında ışık kayıplarının süreleri arasındaki ilişkiyi gösterir.

A scatter plot was used to examine the relationship between **transit time** and **light loss**. This visualization shows the correlation between the duration of light loss during the planet's transit.

### 7. Kepler Teleskobu Gözlemleri (RA / DEC Koordinatları) / Kepler Telescope Observations (RA / DEC Coordinates)

**RA (Right Ascension)** ve **DEC (Declination)** koordinatları kullanılarak Kepler teleskobunun yaptığı gözlemlerin konumları görselleştirilmiştir. Bu görselleştirme, Kepler teleskobunun gökyüzündeki farklı bölgelerdeki gözlemlerini göstermektedir.

The positions of Kepler telescope observations were visualized using **RA (Right Ascension)** and **DEC (Declination)** coordinates. This visualization shows where the Kepler telescope made observations in different regions of the sky.

---

## Kullanılan Görselleştirme Türleri / Visualization Types Used

Projede, gezegenlerin yaşanabilirliğini analiz etmek ve gezegen adaylarının özelliklerini görselleştirmek için çeşitli grafikler ve görselleştirmeler kullanılmıştır:

Various charts and visualizations were used to analyze the habitability of planets and visualize the characteristics of planet candidates:

1. **Scatter Plotlar / Scatter Plots**:
   - Gezegen yarıçapı ve yörünge süresi arasındaki ilişkiyi görselleştirmek için scatter plotlar kullanılmıştır.
   - Transit süresi ile ışık kaybı arasındaki ilişkiyi göstermek için de scatter plot kullanılmıştır.

2. **Isı Haritaları / Heatmaps**:
   - Yıldız sıcaklığı ile gezegen yarıçapı arasındaki ilişkiyi görselleştirmek için bir ısı haritası kullanılmıştır. Bu görselleştirme, bu iki değişken arasındaki korelasyonu çok net bir şekilde sunmaktadır.

3. **Bar Grafikler / Bar Charts**:
   - Gezegen adaylarının **koi_disposition** değerine göre (CONFIRMED, CANDIDATE, FALSE POSITIVE) dağılımını görselleştiren bar grafikler kullanılmıştır. Bu görselleştirme gezegenlerin farklı durumlarını analiz etmeyi kolaylaştırır.

---

## Sonuçlar ve Gelecek Çalışmalar / Results and Future Work

- **Yaşanabilir Gezegenler / Habitable Planets**: Proje, gezegenlerin yaşanabilirlik potansiyelini değerlendirmekte ve hangi gezegenlerin daha yaşanabilir olduğunu belirlemektedir.
- **Gezegen Özelliklerinin İlişkisi / Relationship Between Planet Characteristics**: Gezegenlerin fiziksel özellikleri, yıldız sıcaklığı, yarıçapı, yörünge süresi gibi faktörlerin birbiriyle olan ilişkileri görselleştirilmiştir. Bu analizler, gezegenlerin yaşam barındırabilme potansiyeli hakkında daha fazla bilgi sunmaktadır.
- **Kepler Verisi ve Gelecek Çalışmalar / Kepler Data and Future Work**: Kepler teleskobu verileri, gezegenlerin ve yıldızlarının özelliklerini daha derinlemesine anlamamıza olanak sağlar. Gelecekte bu analizler, daha büyük veri setleri ve ek özellikler kullanılarak genişletilebilir.

---

