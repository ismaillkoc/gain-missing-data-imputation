# GAIN ile Tablosal Verilerde Eksik Veri Tamamlama

Bu proje, **GAIN (Generative Adversarial Imputation Nets)** derin öğrenme mimarisini kullanarak tablosal verilerdeki eksik değerleri tamamlamayı ve performansını geleneksel **KNN** ve **MICE** yöntemleriyle karşılaştırmayı amaçlamaktadır.

## 📌 Proje Özeti
- **Veri Seti:** UCI Concrete Compressive Strength (1030 satır, 9 nitelik)
- **Eksiklik Mekanizması:** Rastgele Tamamen Eksik (MCAR - %10, %20, %30 oranlarında)
- **Kullanılan Yöntemler:** GAIN (Deep Learning), KNN Imputer, MICE (Iterative Imputer)
- **Değerlendirme Metrikleri:** RMSE (Root Mean Squared Error), MAE (Mean Absolute Error)

## 📊 Öne Çıkan Sonuçlar
- **%10 ve %20 Eksiklik:** Küçük/orta boyutlu veri setinde komşuluk ilişkilerini kullanan **KNN** en düşük hatayı vermiştir.
- **%30 Eksiklik:** Bilgi kaybı arttıkça zincirleme regresyon modeli olan **MICE** en yüksek başarıya ulaşmıştır.
- **GAIN Modeli:** 400. epoch'tan itibaren kararlı bir yakınsama göstermiş ve veri yapısını bozmadan doldurma işlemini gerçekleştirmiştir.
