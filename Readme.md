\# 🎭 Deepfake Detection with Transfer Learning



Bu proje, sahte (deepfake) ve gerçek videoları ayırt etmek amacıyla derin öğrenme teknikleri kullanılarak gerçekleştirilmiştir. Projede, farklı transfer learning tabanlı modeller eğitilmiş ve ensemble yöntemleriyle doğruluk artırılmıştır.



---



\## 📌 Proje Amacı



Deepfake teknolojilerinin kötüye kullanımının önüne geçmek için sahte ve gerçek görüntüleri otomatik olarak sınıflandırabilen bir yapay zeka sistemi geliştirmek.



---



\## 🗂️ Kullanılan Veri Seti



\- \*\*FaceForensics++\*\* veri seti

\- Gerçek ve sahte videolardan elde edilen toplam \*\*9365 görüntü\*\*

\- Eğitim, doğrulama ve test olarak üçe ayrıldı.



---



\## 🛠️ Kullanılan Yöntemler ve Modeller



\- \*\*Transfer Learning Modelleri:\*\*

&nbsp; - VGG16

&nbsp; - Xception

&nbsp; - DenseNet121



\- \*\*Veri Ön İşleme:\*\*

&nbsp; - Görüntü yeniden boyutlandırma (224x224)

&nbsp; - Normalizasyon

&nbsp; - Data augmentation (rotation, shift, zoom, flip)



\- \*\*Eğitim:\*\*

&nbsp; - Feature extraction

&nbsp; - Fine-tuning

&nbsp; - EarlyStopping ve ReduceLROnPlateau



\- \*\*Ensemble Yöntemleri:\*\*

&nbsp; - Soft Voting

&nbsp; - Hard Voting

&nbsp; - Weighted Soft Voting



---



\## 📊 Performans Değerlendirmesi



Her model ayrı ayrı değerlendirilmiş ve ensemble yöntemleri ile genel başarı artırılmıştır. Precision, Recall, F1-Score ve Confusion Matrix sonuçları raporlanmıştır.



---





---



\## 💻 Proje Kurulumu



1\. Anaconda ortamınızı oluşturun:

&nbsp;  ```bash

&nbsp;  conda create -n deepfake\_env python=3.9

&nbsp;  conda activate deepfake\_env

&nbsp;  pip install tensorflow scikit-learn matplotlib seaborn



