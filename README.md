# Multi-Panel Dashboards in Pure Matplotlib

<details>
<summary>🇹🇷 Türkçe özet için tıklayın</summary>

Üç farklı veri setini, çok panelli "dashboard" figürleriyle görselleştiren bir çalışma. Her problem, matplotlib ile 4 farklı grafik tekniğini tek bir figürde birleştiriyor, hiçbir yerde seaborn/plotly gibi yüksek seviye bir kütüphane kullanılmadan.

**Problem 1, Streaming Users Dashboard:** keman grafiği, gruplu çubuk grafik, kabarcık grafiği ve yığılmış yatay çubuk grafikten oluşan 4 panelli bir gösterge paneli, ülkeler bölgelere göre gruplanmış.

**Problem 2, City Weather and AQI Dashboard:** ısı haritası, çentikli kutu grafiği, kabarcık dağılım grafiği ve yığılmış alan grafiğiyle iklim/hava kalitesi göstergesi, aylar doğru kronolojik sırayla.

**Problem 3, My Steam Library:** kişisel dokunuşu olan bölüm. Steam Web API'sinden çekilen gerçek oyun kütüphanesi verisiyle (50 oyun, oynama süreleri, türler, başarımlar) 4 panel: en çok oynanan 10 oyun, tür radar grafiği, oynama süresi ile başarım ilişkisi, en çok oynanan oyunun medeniyet tercihleri.

Toplamda tek bir çalışmada 9 farklı görselleştirme tekniği var, hepsi saf matplotlib ile.

</details>

---

Three unrelated datasets, each turned into a four-panel dashboard figure, using nothing but matplotlib. No seaborn, no plotly, no high-level plotting wrapper anywhere.

## Problem 1: Streaming Users Dashboard

Built from `streaming_users.csv`. Four panels: a violin plot, a grouped bar chart, a bubble chart, and a stacked horizontal bar chart. Countries are grouped by region (Americas and so on) throughout.

## Problem 2: City Weather and AQI Dashboard

Built from `city_weather_aqi.csv`. Four panels: a heatmap, a notched boxplot, a bubble scatter plot, and a stacked area chart. Months are kept in proper chronological order rather than alphabetical.

## Problem 3: My Steam Library

The personal one. Real data pulled from the Steam Web API for my own game library: 50 games, playtime, genres, achievements, plus a closer look at the most-played title (Age of Empires II: Definitive Edition). Four panels: top 10 most-played games, a genre radar chart, playtime versus achievement completion, and a pie chart of civilization choices in that top game.

## Techniques used

Nine visualization techniques across the three problems: violin plot, grouped bar, bubble chart, stacked horizontal bar, heatmap, notched boxplot, stacked area chart, radar chart, pie chart. All built directly in matplotlib, without a higher-level charting library doing the work underneath.

## Files

| File | What it is |
|---|---|
| `homework2.ipynb` | All three solutions, code and rendered figures |
| `streaming_users.csv` | Dataset for Problem 1 |
| `city_weather_aqi.csv` | Dataset for Problem 2 |

Problem 3's data (the Steam API output) is embedded directly in the notebook rather than kept as a separate file.

## Tools

Python, Pandas for data handling, Matplotlib for every chart, NumPy.
