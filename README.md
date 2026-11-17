# Derin Öğrenme Uygulamaları: CNN, RNN, LSTM

Geleceği Yazanlar derin öğrenme eğitimi kapsamında Keras/TensorFlow ile yapılan üç uygulama.

| Notebook | Problem | Model | Veri |
|---|---|---|---|
| `01_cnn_atik_siniflandirma.ipynb` | Atık görüntülerini sınıflandırma (karton, cam, metal, kâğıt, plastik, çöp) | Sıfırdan CNN (Conv2D, MaxPooling, Dropout), veri artırma | [Garbage Classification (Kaggle)](https://www.kaggle.com/datasets/asdasdasasdas/garbage-classification) |
| `02_rnn_havayolu_yolcu.ipynb` | Aylık havayolu yolcu sayısı tahmini: zaman serisi keşfi, ölçekleme ve train/test ayrımı | Veri hazırlığı (model kurulumu bu notebook'ta yok) | `data/international-airline-passengers.csv` (1949-1960) |
| `03_lstm_elektrik_tuketimi.ipynb` | Saatlik hane elektrik tüketimi tahmini (son 24 saatten bir sonraki saat) | LSTM, EarlyStopping + ModelCheckpoint | [UCI Individual Household Electric Power Consumption](https://archive.ics.uci.edu/dataset/235/individual+household+electric+power+consumption) |

Notebook'lar çalıştırılmış hâlde, çıktılarıyla birlikte duruyor. Eğitilmiş modeller `models/` klasöründe.

## Çalıştırma

```bash
pip install tensorflow pandas numpy matplotlib scikit-learn opencv-python
jupyter notebook
```

CNN ve LSTM notebook'larındaki veri setleri büyük olduğu için repoda yok. Yukarıdaki bağlantılardan indirilip notebook'taki dosya yolu güncellenmeli.
