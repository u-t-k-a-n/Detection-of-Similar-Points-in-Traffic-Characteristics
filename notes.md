# verileri görselleştirme falan, grafikleri


## data nerede? data cleaning yapacağız.


## outlierları ekleyecek miyiz modele?
- bunda outlierları koymak gerekir gibi geliyor çünkü clustering yapıyoruz


cvp: 5dklık verileri alacağız. temizlenmiş ve üzerinden ön işlem yapılmış halde elimizde var. 
ilk etapta ekstra iş yapmayacaksınız doğrudan o datayı kullanabiliriz.



b veride 10km/s altı ve 132 km/s üstü kullanılmamalı. hatalı veri olabilir, bazıları doğru olsa da.

10 kesin değil belki alt sınır 5 de yapılabilir.


asıl amacımız 0dan kurtulmak. 



## ANOVA ile parametreleri karşılaştıracağız. bir parametre mi, birden fazla mı. 


## dosyaları ilçeler olarak bölgelere ayırıp onun üzerinden işleme başlayalım.
- hiç oraya girmeyin.




elinizde ana arterlerin (çevre yolu, boğaz köprüsüne giden yollar, TEM, basın ekspres yolu, sahil yolu gibi oraların verileri elimizde düzgün var. yaklaşık 400 500 segment. 200-250 lokasyon x2 (karşılıklı yönler olduğu için))


"kadıköy" den yola çıkmak yerine 


haritaya bakıp konumlandırıp çember çizebilirsiniz. elle kendiniz seçip işaretlemeniz daha iyi gözüküyor. 


## ilk adım: data cleaning, görselleştirme etc.

## ikinci adım: 
- pzt ayrı salı-çarş-perş, cuma, haftasonu ayrı

- iş günlerinde grafiklerde 2 tane tepe bekliyoruz iş saatlerinde. 

- cross correlation: bir ilçeyi seçtik x mahallesi ve yanındaki y mahallesi. cross correlation hesaplayıp katsayısını alacağız, +1e ne kadar yakınsa o kadar benzer olduğunu gösteriyor. önce ilçe ilçe

- en büyük ölçek ilçe olarak ilçe ilçe bakacağız. 


her gün içerisindeki 5 dakika

ay bazında yapabiliriz, hafta içinde yapabiliriz. 

segment ID, yönü, kaydedilen hız, timestamp.

faceID ve shazam gibi


benim size tavsiyem: verileri nasıl organize edeceksiniz, benzerliğini hesaplamak için nasıl algoritma kullancaksınız nasıl input output alcaksınız ve bu segmentleri nasıl grupplayacaksınız, gruplar oluşurken özel bişey yapacak mısınız yoksa k-means ile gruplayacak mısınız hierarchical clustering mi kullanacaksınız 

ilk etapta sinyal benzerliğini ölçmek

3-4 tane yakın benzseme ihtimali olan, 7-8tane alakasız segment seç. bak. çıkan sonuçlar mantıklı gruplamaya uygunsa doğru yolda olduğunuzu anlayabilirsiniz.

--------------------------


## başlangıç için bu kadar. 

## bi sonraki adım:


- kümeleme algoritmaları.

- verisetiyle ilgili farklı algoritmalar kullanarak model oluşturma 

- en büyük ölçek ilçe olacak şekilde validation testi oluşturmak için korelasyon yakınlıklarına göre gruplayacağız
