
# 🧠 Deep Learning Binary Classification with TensorFlow

Bu proje, TensorFlow kullanılarak gerçekleştirilmiş bir ikili sınıflandırma (binary classification) problemine çözüm sunmaktadır. Projede temel hedef, verilen veri kümesine göre iki sınıftan birine doğru sınıflandırma yapabilen bir model eğitmektir.

## 📌 Proje Özeti

- Derin öğrenme (Deep Learning) yöntemi kullanılmıştır.
- TensorFlow ve Keras kütüphaneleriyle model geliştirilmiştir.
- Model, `accuracy`, `precision`, `recall` ve `f1-score` gibi metriklerle değerlendirilmiştir.
- Nihai model test verisinde yaklaşık **%82 doğruluk (accuracy)** sağlamıştır.

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
| 0     | 1.00      | 0.69   | 0.82     | 449     |
| 1     | 0.72      | 1.00   | 0.84     | 363     |

**Genel Sonuçlar:**

- Accuracy: **0.83**
- Macro Avg: Precision **0.86**, Recall **0.84**, F1-Score **0.83**
- Weighted Avg: Precision **0.87**, Recall **0.83**, F1-Score **0.83**

🔍 Not: Modelin pozitif sınıfı (1) daha iyi tanıdığı, ancak negatif sınıfta (0) bazı yanlış sınıflamalar yaptığı gözlemlenmiştir.

## 🏗️ Model Eğitimi

Model aşağıdaki gibi eğitilmiştir:

```python
model.predict(x_test) > 0.5
```

### Kayıp ve Doğruluk:

- Loss: `0.5712`
- Accuracy (test set): `0.8288`

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

- `model.ipynb` dosyasında model mimarisi, eğitim süreci ve metrikler detaylı şekilde açıklanmıştır.
- İleri düzey performans için katman sayısı ve hiperparametreler üzerinde oynama yapılabilir.

## 📬 İletişim

Herhangi bir sorunuz varsa benimle iletişime geçmekten çekinmeyin:

- GitHub: [github.com/gelisgen03](https://github.com/gelisgen03)
- Email: gelisgen987@gmail.com
- Suleyman Asim Gelisgen
---

