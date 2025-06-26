# flower-classification-cnn
Bu proje, derin öğrenme tabanlı bir çiçek sınıflandırma sistemidir. Görüntü verileri, MobileNetV2 modeliyle eğitilmiş ve veri artırma teknikleriyle desteklenmiştir. Eğitim sürecinde en iyi başarıyı sağlayan model .keras formatında kaydedilmiş ve test sonuçları görsel olarak analiz edilmiştir.

Özellikler
    •    Transfer Learning yöntemiyle MobileNetV2 kullanılarak sınıflandırma yapılmıştır.
    •    Eğitim ve doğrulama verileri üzerinde veri artırma uygulanmıştır.
    •    Model, düzenli katman yapısı ve dropout ile overfitting’e karşı optimize edilmiştir.
    •    Test sonuçları hem sayısal hem de görsel olarak değerlendirilmiştir.

Kullanılan Teknolojiler
    •    Python
    •    TensorFlow / Keras
    •    MobileNetV2 (pre-trained)
    •    Matplotlib, PIL
    •    Pandas, NumPy

Proje Dosyaları
Dosya Adı
Açıklama
mobilenetv2_final_best.keras
Eğitilmiş modelin ağırlıkları
Untitled-1.ipynb
Eğitim, test ve değerlendirme kodlarını içeren Jupyter Notebook
README.md
Bu dosya

Eğitim Detayları
    •    Model: MobileNetV2 (pre-trained, imagenet)
    •    Giriş boyutu: 224x224x3
    •    Optimizasyon: Adam (learning rate: 1e-4)
    •    Kayıp fonksiyonu: Categorical Crossentropy
    •    EarlyStopping: 7 epoch boyunca iyileşmeyen val_loss durumunda eğitim durdurulur
    •    Kullanılan veri artırma teknikleri:
    ◦    Dönme, kaydırma, yakınlaştırma, parlaklık değişimi, yatay çevirme

Sonuç Görselleri
Doğru tahmin edilen örnek görüntüler ve yanlış tahmin edilen örnek görüntüler analiz edilmiştir. Görseller GitHub deposuna dahil edilmiştir.

Nasıl Çalıştırılır
# Gerekli kütüphanelerin kurulumu
pip install tensorflow matplotlib pandas numpy pillow

# Jupyter Notebook ile çalıştırmak için
jupyter notebook
Not: Kodlar, train_df, val_df, test_df ve classes adlı değişkenlerin önceden tanımlandığını varsayar.

Açıklamalar
    •    Projede farklı modeller test edilmiş, en iyi sonuç MobileNetV2 modeliyle elde edilmiştir.
    •    Eğitilmiş model ağırlıkları .keras formatında sunulmuştur.
    •    Eğitim verileri DataFrame yapısında tanımlanmış ve flow_from_dataframe ile kullanılmıştır.

Geliştiren
Bu proje, bireysel bir öğrenme ve uygulama çalışması olarak geliştirilmiştir. Eğitim amaçlıdır ve GitHub üzerinden erişilebilir durumdadır.


