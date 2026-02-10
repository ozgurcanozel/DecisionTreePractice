# Decision Tree Practice - Graduate Admission Prediction

Bu proje, öğrencilerin akademik verilerini kullanarak lisansüstü eğitim başvurularında üniversite kabul alma olasılığını tahmin eden bir **Makine Öğrenmesi (Machine Learning)** çalışmasıdır.

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

## 🛠️ Teknik Detaylar
- **Veri Ön İşleme:** Tahminleme için doğrudan etkisi olmayan `Serial No.` sütunu veri setinden çıkarılmıştır.
- **Ölçeklendirme:** Model performansını artırmak için veriler `StandardScaler` ile normalize edilmiştir.
- **Model:** Tahminleme işlemi için `DecisionTreeRegressor` algoritması tercih edilmiştir.
- **Optimizasyon:** `GridSearchCV` kullanılarak en iyi hiperparametreler belirlenmiştir.

## 📈 Model Performansı
Hiperparametre optimizasyonu sonrası elde edilen sonuçlar:
- **R² Skoru:** ~0.78
- **En İyi Parametreler:** `criterion='squared_error'`, `max_depth=5`, `splitter='random'`.
