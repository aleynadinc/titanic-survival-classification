# Titanic — Hayatta Kalma Tahmini

Klasik Titanic veri seti üzerinde yolcuların hayatta kalıp kalmadığını tahmin eden bir Lojistik Regresyon projesi.

## Problem Türü
İkili Sınıflandırma — hedef `Survived` (0: öldü, 1: hayatta kaldı).

## Veri Seti
Titanic yolcu kayıtları. Kullanılan özellikler:
- `Pclass`: Yolcu sınıfı (1, 2, 3)
- `SibSp`: Gemideki kardeş/eş sayısı
- `Parch`: Gemideki ebeveyn/çocuk sayısı
- `Fare`: Bilet ücreti

## Yaklaşım
1. Veriyi URL üzerinden içe aktarma
2. `info()` ve `describe()` ile keşif
3. 4 sayısal özellik ile X ve y oluşturma
4. `train_test_split` (random_state=0)
5. `StandardScaler` ile ölçeklendirme
6. `LogisticRegression` eğitimi
7. Model doğruluğu: **~%71**
8. Yeni bir yolcu için tahmin

## Kullanılan Kütüphaneler
- `pandas`, `scikit-learn`
- `StandardScaler`, `LogisticRegression`

## Ana Çıkarım
%71 doğruluk, lojistik regresyonun varsayılan metriği olan accuracy'nin anlamını kavramak için iyi bir başlangıç. Model doğru tahminlerin yaklaşık %71'ini yapıyor; daha fazla özellik veya karmaşık model ile iyileştirilebilir.
