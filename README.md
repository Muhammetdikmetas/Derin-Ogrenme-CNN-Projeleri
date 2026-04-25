# 🧠 Derin Öğrenme CNN Projeleri

Bu depo, Evrişimli Sinir Ağları (CNN) alanındaki çalışmalarımı sergilemek amacıyla oluşturulmuştur.

## 📂 Proje 1: CIFAR-10 Görüntü Sınıflandırma

CIFAR-10 veri seti kullanılarak geliştirilen, görüntü sınıflandırma tabanlı bir CNN modelidir.

### ⚙️ Teknik Detaylar
* **Veri Boru Hattı:** `tf.data.Dataset` kullanılarak optimize edilmiştir.
* **Mimari:** Çok katmanlı Evrişimli Sinir Ağı (Conv2D, MaxPooling, Flatten, Dense).
* **Optimizasyon:** `adam` optimizer ve `sparse_categorical_crossentropy` kayıp fonksiyonu kullanılmıştır.
* **Güvenlik Önlemleri:** Overfitting'i önlemek için `EarlyStopping` ve `ModelCheckpoint` callback'leri uygulanmıştır.

### 📊 Eğitim Analizi
Eğitim sürecinde doğrulama kaybının (val_loss) artış göstermesi, modelin veri setini ezberleme (overfitting) eğiliminde olduğunu göstermektedir. Bu durum, gelecekteki projelerde Dropout ve Veri Çoğaltma (Data Augmentation) teknikleri ile iyileştirilecektir.
