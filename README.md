Bu GitHub reposunda, el yazısı rakamları tanımak için Convolutional Neural Networks (CNN) kullanarak bir derin öğrenme modeli oluşturulmuştur. Aşağıda bu modelin nasıl inşa edildiği ve işlendiği hakkında kısa bir özet bulunmaktadır:

### Kullanılan Kütüphaneler:
- **NumPy ve Pandas**: Veri manipülasyonu ve analiz için.
- **Seaborn ve Matplotlib**: Görselleştirme için.
- **Keras**: Derin öğrenme modeli oluşturma ve eğitim için.

### Veri Hazırlığı:
- **Veri Seti Yükleme**: Eğitim ve test veri setleri `train.csv` ve `test.csv` dosyalarından yüklendi.
- **Veri İnceleme**: Veri setlerinin yapısı ve içerikleri incelendi.
- **Normalizasyon**: Piksel değerleri 0-255 arasında olup, bu değerler 0-1 aralığına ölçeklendirildi.
- **Yeniden Şekillendirme**: Görüntüler 28x28x1 boyutunda 3B matrislere dönüştürüldü.
- **Etiket Kodlama**: Etiketler tek sıcak vektörlere dönüştürüldü.

### Model Oluşturma:
- **CNN Yapısı**: 
  - **Convolutional Layers**: Evrişim katmanları ile özellikler çıkarıldı.
  - **Max Pooling Layers**: Boyut küçültme ve genelleme işlemleri yapıldı.
  - **Dropout Layers**: Aşırı öğrenmeyi önlemek için dropout katmanları kullanıldı.
  - **Flatten Layer**: Düzleştirme işlemi yapıldı.
  - **Dense Layers**: Tam bağlantılı katmanlarla sınıflandırma gerçekleştirildi.

### Model Eğitimi:
- **Optimizasyon Algoritması**: Adam optimizasyon algoritması kullanıldı.
- **Loss Function**: Kategorik çapraz entropi kayıp fonksiyonu kullanıldı.
- **Epochs ve Batch Size**: Model 10 epoch boyunca ve her bir batch boyutu 250 olacak şekilde eğitildi.
- **Veri Artırma**: Veri çeşitliliğini artırmak için çeşitli dönüşümler uygulandı.

### Model Değerlendirme:
- **Test Kaybı Görselleştirme**: Eğitim ve doğrulama kayıpları görselleştirildi.
- **Karışıklık Matrisi**: Modelin sınıflandırma performansı karışıklık matrisi ile değerlendirildi.

### Sonuç:
Bu repo, el yazısı rakamları tanıma problemini çözmek için CNN kullanarak adım adım bir derin öğrenme modelinin nasıl oluşturulacağını, eğitileceğini ve değerlendirileceğini göstermektedir. Modelin performansı görselleştirmeler ve karışıklık matrisi ile detaylandırılmıştır.
