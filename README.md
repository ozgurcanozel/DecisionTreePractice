# Decision Tree Practice - Graduate Admission Prediction

Bu proje, bir öğrencinin akademik verilerini kullanarak lisansüstü eğitim başvurularında üniversite kabul alma olasılığını tahmin eden bir **Makine Öğrenmesi (Machine Learning)** çalışmasıdır.

## 🚀 Proje Özeti
Proje kapsamında, `Admission_Predict_Ver1.1.csv` veri seti kullanılarak öğrencilerin kabul şansları (`Chance of Admit`) regresyon modelleri ile tahmin edilmiştir. Veri analizi sürecinde veri temizleme, görselleştirme ve model optimizasyonu adımları uygulanmıştır.



## 📊 Veri Seti İçeriği
Modelin eğitilmesinde kullanılan temel parametreler şunlardır:
- **GRE Score:** Lisansüstü Giriş Sınavı puanı.
- **TOEFL Score:** İngilizce yeterlilik sınavı puanı.
- **University Rating:** Mezun olunan üniversitenin derecesi.
- **SOP & LOR:** Niyet ve Referans mektuplarının gücü.
- **CGPA:** Lisans not ortalaması.
- **Research:** Araştırma deneyimi (0 veya 1).

## 🛠️ Teknik Detaylar ve Kullanılan Araçlar
Proje Python programlama dili ile geliştirilmiştir. Kullanılan temel kütüphaneler:
- **Veri Analizi:** `Pandas`, `NumPy`
- **Görselleştirme:** `Seaborn`, `Matplotlib`
- **Model Geliştirme:** `Scikit-Learn`

### Uygulanan İşlemler:
1. **Veri Ön İşleme:** Gereksiz olan `Serial No.` sütunu veri setinden çıkarılmıştır.
2. **Ölçeklendirme:** Model performansını artırmak için `StandardScaler` kullanılmıştır.
3. **Model:** Tahminleme işlemi için `DecisionTreeRegressor` algoritması tercih edilmiştir.
4. **Optimizasyon:** `GridSearchCV` kütüphanesi ile en iyi hiperparametreler (`max_depth`, `criterion`, `splitter`) belirlenmiştir.

## 📈 Model Sonuçları
Hiperparametre optimizasyonu sonrası elde edilen en iyi sonuçlar:
- **R² Skoru:** ~0.78 (Modelin veriyi açıklama oranı).
- **En İyi Parametreler:** `criterion='squared_error'`, `max_depth=5`, `splitter='random'`.



## ⚙️ Kurulum
Bu projeyi kendi ortamınızda çalıştırmak için:

1. Depoyu klonlayın:
   ```bash
   git clone [https://github.com/ozgurcanozel/DecisionTreePractice.git](https://github.com/ozgurcanozel/DecisionTreePractice.git)
