# 3B Medikal Resim Segmentasyonu İçin Modalite Bağımsız SAM Adaptasyonu İncelemesi 

Bu çalışmada MA-SAM, nnU-Net ve Mask R-CNN modelleri BraTS20 veri üzerine uygulanmış ve sonuçları karşılaştırılmıştır. Modellerin kodlari ilgili dosyalarda paylaşılmıştır. 
3 Model için de başlangıç noktası Google Drive içerisinde BraTS20 veri setinin arşiv dosyasının bulunmasıdır. Dikkat edilmesi gereken nokta ise arşiv dosyası çıkartılırken doğru yolun yazılmasıdır.

### MA-SAM
Bu model için eğitimde yapılması gereken MA-SAM kodu Drive içine klonlandıktan sonra tüm hücrelerin yukarıdan aşağıya çalıştırılmasıdır. Veriler hazırlandıktan sonra eğitime başlayacaktır. Test verileri üzerinde tahmin yapmak içinse aşağıdaki kod çalıştırılmalıdır. 
```
!python /path/to/test.py --adapt_ckpt /content/output/epoch_xx.pth --data_path /content/data --vit_name vit_b --ckpt /path/to/pre-trained-weight --is_savenii
```

### MASK R-CNN ve nnU-Net
Tüm hücrelerin yukarıdan aşağıya çalıştırılması yeterlidir.

