# CNN Modelleri Kullanılarak Çiçek Türlerini Tanınması 

Bu proje, çeşitli çiçek türlerini sınıflandırmak için kullanılan üç farklı Convolutional Neural Network (CNN) modelini içerir. Proje, TensorFlow ve Keras kütüphaneleriyle geliştirilmiştir ve çiçek türlerini tanımak üzere eğitilmiştir.

## Proje Açıklaması

Bu Python dosyası, çiçek türlerini tanımak için eğitilmiş bir derin öğrenme modeli oluşturmayı amaçlamaktadır. Veri seti, Ayçiçeği, Gül, Karahindiba, Lale, Papatya ve Süsen gibi altı farklı çiçek kategorisini içermektedir.

## Veri Seti ve Görselleştirme

Veri seti, her biri altı çiçek sınıfından gelen 500 görüntü içerir. Veri seti, her sınıftan örnek görseller içeren bir görsel içermektedir.

## Veri Ön İşleme

Veri seti, 3. modelde ImageDataGenerator kullanılarak ön işleme adımlarından geçirilmiştir projenin başarımını artırmak amacı ile . Görüntüler, döndürme, ölçeklendirme, kaydırma ve diğer veri artırma teknikleri kullanılarak çeşitlendirilmiştir.

## Model Oluşturma

Oluşturulan CNN modeli, Conv2D, MaxPooling2D, Flatten ve Dense katmanlarından oluşmaktadır. Modeller , belirli bir çiçek türünü tanımak için eğitilmiştir.

## Model Eğitimi

Model, eğitim verileri üzerinde eğitilmiştir. Eğitim sırasında kullanılan optimizasyon algoritması "adam" ve "Adamax" kulanılmıştır  kayıp fonksiyonu "categorical_crossentropy" olarak belirlenmiştir.

## Eğitim Sonuçları

Eğitim sonuçları, başarı grafiği ve kayıp grafiği şeklinde görselleştirilmiştir.

## Test ve Değerlendirme

Model, ayrı bir test veri seti üzerinde değerlendirilmiştir. Elde edilen sonuçlar, doğruluk ve kayıp metrikleri üzerinden raporlanmıştır.

### Gereksinimler
- Python==3.8.18
- tensorflow==2.12.0
- numpy==1.26.2
- matplotlib==3.5.0
- Pillow==10.0.1
- scikit-learn==1.0.2
- keras==2.12.0
- imageio==2.16.0
- tensorflow-estimator==2.12.0
- h5py==3.9.0
