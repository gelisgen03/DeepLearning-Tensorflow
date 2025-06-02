
# 🧠 Deep Learning Binary Classification with TensorFlow

Bu proje, TensorFlow kullanılarak gerçekleştirilmiş bir ikili sınıflandırma (binary classification) problemine çözüm sunmaktadır. Projede temel hedef, verilen veri kümesine göre iki sınıftan birine doğru sınıflandırma yapabilen bir model eğitmektir.

## 📌 Proje Özeti

- Derin öğrenme (Deep Learning) yöntemi kullanılmıştır.
- TensorFlow ve Keras kütüphaneleriyle model geliştirilmiştir.
- Model, `accuracy`, `precision`, `recall` ve `f1-score` gibi metriklerle değerlendirilmiştir.
- Nihai model test verisinde yaklaşık **%98 doğruluk (accuracy)** sağlamıştır.

## 🧰 Kullanılan Teknolojiler

- Python
- TensorFlow / Keras
- Scikit-learn
- NumPy
- Matplotlib (isteğe bağlı görselleştirme için)

## 📁 Dosya Yapısı

```

├── data                 # Model için kullanılan data ve data açıklamalarını içeren dosyalar
├── model                # Model geliştirme sürecini içeren Jupyter defteri
└── visuals              # Model değerlendirimesi ile oluşturulan Grafikler
```

## 🧪 Model Performansı

| Sınıf | Precision | Recall | F1-Score | Support |
|------:|----------:|-------:|---------:|--------:|
| 0     | 0.99      | 0.98   | 0.97     | 449     |
| 1     | 0.98      | 0.99   | 0.98     | 363     |

**Genel Sonuçlar:**

- Accuracy: **0.98**
- Macro Avg: Precision **0.98**, Recall **0.99**, F1-Score **0.98**
- Weighted Avg: Precision **0.96**, Recall **0.95**, F1-Score **0.99**

🔍 Not: Modelin pozitif sınıfı (1) daha iyi tanıdığı, ancak negatif sınıfta (0) bazı yanlış sınıflamalar yaptığı gözlemlenmiştir.

## 🏗️ Model Eğitimi

Model aşağıdaki gibi eğitilmiştir:

```python
model.predict(x_test) > 0.5
```



## 🚀 Kurulum ve Çalıştırma

### 1. Ortamı Hazırlayın

```bash
git clone https://github.com/gelisgen03/DeepLearning-Tensorflow.git
cd DeepLearning-Tensorflow
python -m venv venv
source venv/bin/activate  # Windows için: venv\Scripts\activate

```

### 2. Jupyter Notebook'u Açın

```bash
jupyter notebook model.ipynb
```

## 🔍 Gereksinimler

- tensorflow
- scikit-learn
- numpy
- pandas
- matplotlib (opsiyonel)

## 🖼️ Sınıflandırma Raporu Görselleştirmesi

- Sonuç Grafiklere Ana dizindeki `visuals` klasöründen ulaşabilirsiniz.

## 📌 Notlar

- `model/.ipynb` uzantı dosyasında model mimarisi, eğitim süreci ve metrikler detaylı şekilde açıklanmıştır.


## 📅 Dataset Link
`https://archive.ics.uci.edu/dataset/73/mushroom`

## 📬 İletişim

Herhangi bir sorunuz varsa benimle iletişime geçmekten çekinmeyin:

- GitHub: [github.com/gelisgen03](https://github.com/gelisgen03)
- Email: gelisgen987@gmail.com
- Suleyman Asim Gelisgen
---

