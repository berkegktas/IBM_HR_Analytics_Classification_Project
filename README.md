# IBM_HR_Analytics_Classification_Project
Amaç, çalışanların işten ayrılma olasılığını tahmin eden bir sınıflandırma modeli geliştirmek ve bu tahminlerde etkili olan faktörleri analiz etmektir.

# Çalışan Ayrılma Tahmini (Employee Attrition Prediction)

## Proje Amacı
Bu projenin amacı, çalışanların işten ayrılma (attrition) olasılığını tahmin eden bir makine öğrenmesi modeli geliştirmek ve çalışan ayrılmalarında etkili olan faktörleri analiz etmektir.

Proje, sınıflandırma problemleri, dengesiz veri setleri ve model yorumlanabilirliği konularına odaklanmaktadır.
---
## Veri Seti
- Kaynak: IBM HR Analytics Attrition Dataset (Kaggle)
- Gözlem sayısı: 1470
- Değişken sayısı: 35
- Hedef değişken: `Attrition` (Yes / No)
- Eksik veri: Yok

Veri seti sentetiktir ve eğitim amaçlı oluşturulmuştur.
---
## Kullanılan Yöntemler
- Keşifsel Veri Analizi (EDA)
- Özellik seçimi ve özellik mühendisliği
- Dengesiz sınıf problemi ile başa çıkma (class weight / oversampling)
- Makine öğrenmesi modelleri:
  - Lojistik Regresyon
  - Random Forest
- Model değerlendirme metrikleri:
  - ROC-AUC
  - Recall (Attrition = Yes)
---
## Öne Çıkan Bulgular
- Fazla mesai (OverTime) yapan çalışanların işten ayrılma olasılığı daha yüksektir.
- Aylık gelir arttıkça ayrılma olasılığı azalmaktadır.
- Bazı iş rollerinde ayrılma riski diğerlerine göre daha yüksektir.

Bu ilişkiler istatistiksel olup nedensellik ifade etmemektedir.
---
## Modelleme Yaklaşımı
- Lojistik regresyon temel (baseline) model olarak kullanılmıştır.
- Ağaç tabanlı modeller ile performans karşılaştırması yapılmıştır.
- Dengesiz veri problemi değerlendirme aşamasında dikkate alınmıştır.
- Oversampling yalnızca eğitim verisi üzerinde uygulanmıştır.
---
## Sınırlamalar
- Veri seti sentetik olduğu için gerçek dünya sonuçlarını birebir yansıtmayabilir.
- Zaman boyutu bulunmadığından çalışan davranışları dinamik olarak incelenememektedir.
---
## Kullanılan Teknolojiler
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib / Seaborn
---
## Lisans
MIT License

