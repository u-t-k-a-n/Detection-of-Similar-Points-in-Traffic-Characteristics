
## 1) FileCleaning_2017
- Herhangi bir anda hız değeri 10 km/h'nin altındaki veya 130 km/h'nin üzerindeki dosyaların tespiti yapıldı
- Bütün dosyalarda herhangi bir anda hız değeri 10 km/h'nin altına düştüğü görülmüştür
- Dosyaların yarıdan fazlasında herhangi bir anda hız değeri 130 km/h'nin üstüne çıktığı görülmüştür
- Bazı dosyaların hız değeri tüm yıl boyunca 10 km/h'nin altında olduğu görülmüştür. Öte yandan dosyaların tüm yıl 
  boyunca hız değerlerinin 130 km/h'yi geçip geçmediği incelendiğinde, bir yıl boyunca hız değeri 130 km/h'yi aşan değerler, 
  tüm yıl boyunca hız değerlerinin en fazla %12'sini oluşturduğu gözlenmiştir.
- Çalışmamızı olumsuz yönde etkilememesi için, hızı 10 km/h'nin altında olan değerler tüm yıl boyunca hız değerlerinin %30'u ve üzerinde ise o dosyaları sildik.
- Son olarak koordinatları belli olmayan dosyaları da sildik.

## 2) FeatureEngineering_2017
- Hız değeri 10 km/h'nin altında olan değerler 10 km/h yapıldı ve bunun bilgisi veri setine yeni sütün olarak eklendi
- Hız değeri 130 km/h'nin üstünde olan değerler 130 km/h yapıldı ve bunun bilgisi veri setine yeni sütün olarak eklendi

## 3) DataVisualization_2017
- Herhangi bir ayın, istenilen gün bazında 5 dakikalık periyotlarla trafik akış hızının çizgi grafiğini gösteren fonksiyon: show_plotline_5minutes(filename,month,day)
- Herhangi bir ayın, istenilen gün bazında 5 dakikalık periyotlarla trafik akış hızının çubuk grafiğini gösteren fonksiyon: show_barplot_5minutes(filename,month,day)
- Herhangi bir ayın, istenilen gün ve periyot bazında  trafik akış hızının çizgi grafiğini gösteren fonksiyon: show_plotline(filename,month,day,minute)

## 4) Coordinates_2017
- Coordinates.json dosyasından elimizde bulunan dosyaların koordinatlarını çektik
- Bütün dosyalar için eşsiz koordinatları belirledik ve bunları csv dosyası olarak kaydettik

## 5) Map_2017 
- Elimizde bulunan koordinatlara göre, dosyaların harita üzerinde görüntülenmesi

## 6) SimilarityScore
- İki dosya arasında istenilen ay,gün,periyot bakımından korelasyon katsayısını hesaplayan fonksiyon: score_corrcoef(file1,file2,month=None,day=None,minute=5)

## 7) 




