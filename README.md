# 🏠 House Price Prediction Project

Bu proje, Kaggle üzerindeki "House Prices: Advanced Regression Techniques" veri seti kullanılarak geliştirilmiş uçtan uca bir makine öğrenmesi projesidir.

## 🎯 Projenin Amacı
Evlerin çeşitli özelliklerine (oda sayısı, metrekare, mahalle, malzeme kalitesi vb.) bakarak satış fiyatlarını tahmin etmek ve gayrimenkul değerlemesi için istatistiksel bir model oluşturmak.

## 🛠️ Kullanılan Teknolojiler ve Yöntemler
* **Python** (Pandas, NumPy)
* **Veri Görselleştirme:** Matplotlib, Seaborn
* **İstatistiksel Analiz:** Log Transformation, Z-Score Scaling, Correlation Analysis
* **Modeller:**
    * Lineer Regresyon (Baseline)
    * Ridge & Lasso Regresyon (Regularization)
    * Random Forest Regressor
    * XGBoost Regressor

## 📊 Sonuçlar
Proje kapsamında farklı modeller denenmiş ve başarı skorları ($R^2$) karşılaştırılmıştır:

| Model | R^2 Skoru | RMSE (Log) |
|-------|----------|------------|
| Linear Regression | 0.77 | 0.20 |
| Ridge Regression (En İyi) | **0.895** | **0.14** |
| Random Forest | 0.88 | 0.15 |
| XGBoost | 0.89 | 0.14 |

**Sonuç:** Veri setindeki doğrusal ilişkilerin baskın olması nedeniyle, optimize edilmiş **Ridge Regresyon** modeli en iyi sonucu vermiştir.

## 🚀 Nasıl Çalıştırılır?
1. Repoyu klonlayın.
2. `House_Price_Prediction.ipynb` dosyasını Jupyter Notebook veya Google Colab ile açın.
3. Gerekli kütüphaneleri yükleyin (`pip install pandas sklearn xgboost seaborn`).
