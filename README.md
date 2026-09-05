# Data Visualization — Homework 2

İTÜ YZV475E (Data Visualization) dersi kapsamında hazırlanmış, üç farklı veri setini çok panelli "dashboard" figürleriyle görselleştiren bir ödev. Her problem, matplotlib ile 4 farklı grafik tekniğini tek bir figürde birleştiriyor.

## İçerik

### Problem 1 — Streaming Users Dashboard
`streaming_users.csv` verisiyle 4 panelli bir gösterge paneli: keman grafiği (violin plot), gruplu çubuk grafik, kabarcık grafiği (bubble chart), yığılmış yatay çubuk grafik. Ülkeler bölgelere (Americas, vb.) gruplanarak analiz ediliyor.

### Problem 2 — City Weather and AQI Dashboard
`city_weather_aqi.csv` verisiyle iklim ve hava kalitesi göstergesi: ısı haritası (heatmap), çentikli kutu grafiği (notched boxplot), kabarcık dağılım grafiği, yığılmış alan grafiği (stacked area chart). Aylar doğru kronolojik sırayla işleniyor.

### Problem 3 — My Steam Library: How Did I Spend My Gaming Hours?
Kişisel bir dokunuş — Steam Web API'sinden çekilen gerçek kendi oyun kütüphanesi verisi (50 oyun, oynama süreleri, türler, başarımlar) + en çok oynanan oyun (Age of Empires II: Definitive Edition) için detaylı istatistikler. 4 panel: en çok oynanan 10 oyun çubuk grafiği, tür radar grafiği, oynama süresi vs. başarım dağılım grafiği, AoE2 medeniyet tercihleri pasta grafiği.

## Kullanılan Teknikler

Tek bir ödevde 9 farklı görselleştirme tekniği: violin plot, grouped bar, bubble chart, stacked horizontal bar, heatmap, notched boxplot, stacked area chart, radar chart, pie chart — hepsi saf matplotlib ile (yüksek seviye görselleştirme kütüphanesi kullanılmadan).

## Dosyalar

| Dosya | Açıklama |
|---|---|
| `homework2.ipynb` | Tüm çözümler ve üretilen görseller |
| `streaming_users.csv` | Problem 1 veri seti |
| `city_weather_aqi.csv` | Problem 2 veri seti |

Problem 3'ün verisi (Steam API çıktısı) notebook içine doğrudan gömülü.

## Kullanılan Araçlar

Python — Pandas (veri işleme), Matplotlib (tüm görselleştirmeler), NumPy.
