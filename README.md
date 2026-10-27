# EczaStok – Kullanım Kılavuzu

EczaStok, eczanelerde ilaç sayımını telefon veya tablet kamerasıyla hızlandıran bir uygulamadır.
İlaç karekodlarını (GS1 DataMatrix) ve ürün barkodlarını okur, sayım listelerini oluşturur ve
eczane programınıza aktarabileceğiniz dosyalar üretir.

- [Gizlilik Politikası](gizlilik.md) · [Privacy Policy (English)](privacy.md)
- Destek: [gokrememre@gmail.com](mailto:gokrememre@gmail.com)

---

## İçindekiler

1. [Ana ekran ve ayarlar](#ana-ekran-ve-ayarlar)
2. [İlaç Bilgi](#ilaç-bilgi)
3. [Karekod Sayım](#karekod-sayım)
4. [Barkod Sayım](#barkod-sayım)
5. [Karekod Karşılaştırma](#karekod-karşılaştırma)
6. [Sayım Birleştirme](#sayım-birleştirme)
7. [Dışa aktarılan dosyalar](#dışa-aktarılan-dosyalar)
8. [Ücretsiz sürüm ve abonelik](#ücretsiz-sürüm-ve-abonelik)
9. [Kamera ipuçları](#kamera-ipuçları)
10. [Sık sorulan sorular](#sık-sorulan-sorular)

---

## Ana ekran ve ayarlar

Ana ekranda her satırda bir mod bulunur. Kilit simgesi olan modlar tam sürümde açılır.

Uygulama açıldığında ilaç adı ve fiyat verilerinin güncel olup olmadığını kontrol eder. Yeni
liste varsa indirir; üstte kısa süre "Veriler güncelleniyor…" yazar, bitince kaybolur. İnternet
yoksa cihazda kayıtlı son liste kullanılır.

Sağ üstteki **dişli** simgesiyle ayarlara ulaşırsınız:

- **Tema:** Sistem, Açık veya Koyu
- **Okutma sesi:** Yeni bir kod listeye eklendiğinde bip sesi
- **İlaç verilerini güncelle:** Listeyi elle yeniden kontrol eder
- **Tam sürüm / Satın alımları geri yükle / Aboneliği yönet**

## İlaç Bilgi

Bir ilacın karekodunu veya barkodunu kameraya gösterin. Alttaki kartta ilacın adı, fiyatı,
firması, barkodu ve karekoddaysa **son kullanma tarihi (SKT)**, kalan gün sayısı, seri ve parti
numarası görünür.

## Karekod Sayım

Raflardaki ilaçların karekodlarını okutarak sayım listesi oluşturur.

- **Aynı anda birden fazla kutu** okunabilir; kutuları yan yana dizip kamerayı üzerlerinde gezdirin.
- Her karekodun çevresine bir çerçeve çizilir. Renkler SKT'yi gösterir:
  - **Yeşil:** SKT'ye 6 aydan fazla var
  - **Turuncu:** SKT'ye 6 aydan az kaldı
  - **Kırmızı:** SKT geçmiş
- Yeni eklenen kutuda kısa süre **EKLENDİ**, daha önce okunmuş kutuda **OKUNDU** yazar. Her kutu
  (karekod) benzersiz olduğundan aynı kutu iki kez sayılmaz.
- **İlaç adı** düğmesi açıkken ilacın adı çerçevenin altında görünür.
- Listeden bir satırı silmek için sola kaydırın; tüm listeyi silmek için çöp kutusu simgesi.
- Liste uygulama kapansa da saklanır.

## Barkod Sayım

Karekodu olmayan barkodlu ürünler (dermokozmetik, medikal ürünler vb.) içindir.

- Barkodu okuttuğunuzda **adet** sorulur. Aynı barkodu tekrar okutursanız girilen adet mevcut adede eklenir.
- Listedeki bir ürüne dokunarak adedi düzeltebilirsiniz.
- Kamerayla okunamayan barkodları **Elle gir** düğmesiyle yazabilirsiniz.
- Dışa aktarmada her barkod, adedi kadar alt alta yazılır (ör. A barkodu 10 adet → 10 satır A).
  Eczane programları barkodlu ürün stoğunu genellikle bu biçimde alır.

## Karekod Karşılaştırma

Eczane programınızdaki stok ile raftaki fiziki stoğu karşılaştırır.

Ekranın üstündeki numaralı adımları sırayla izleyin; alttaki **İleri** / **Geri** düğmeleriyle
veya adım numarasına dokunarak geçebilirsiniz.

1. **Sistem listesi:** Eczane programınızdan aldığınız karekod listesini **Dosyadan** (xlsx, csv,
   txt) veya **Panodan** içe aktarın.
2. **Fiziki sayım:** **Tara** ile raftaki kutuları okutun veya **Sayımdan al** ile Karekod Sayım
   listesini aktarın. Taramada sistemde olmayan kutuların üzerinde **SİSTEMDE YOK** yazar.
3. **Sonuç:**
   - **Kırmızı – EKSİK:** Sistemde var, rafta yok
   - **Turuncu – FAZLA:** Rafta var, sistemde yok
   - **Yeşil – TAMAM:** İkisinde de var

   Etiketlere dokunarak listeyi süzebilirsiniz. **Eksikleri kopyala** / **Fazlaları kopyala**
   düğmeleri ilgili karekodları panoya kopyalar; eczane programınıza doğrudan yapıştırabilirsiniz.

Sağ üstteki paylaş menüsünden eksik veya fazla karekodları **Metin (.txt)** olarak, ya da tüm
sonucu **Excel** olarak dışa aktarabilirsiniz.

## Sayım Birleştirme

Farklı zamanlarda veya farklı cihazlarda yapılmış sayım dosyalarını tek dosyada birleştirir.

- **Dosya ekle** ile birden fazla TXT/CSV dosyası seçin; **Uygulamadan** ile cihazdaki mevcut
  sayımları da ekleyebilirsiniz.
- Karekodlar birleştirilirken **tekrar edenler bir kez sayılır**. Tekrar eden karekod varsa
  "tekrar eden karekod çıkarıldı" satırına dokunarak hangi ilacın hangi dosyalarda tekrar ettiğini
  görebilirsiniz.
- Barkod dosyalarındaki **adetler toplanır**.
- Sonucu birleşik karekod listesi (TXT) ve birleşik barkod listesi (TXT veya Excel) olarak alın.

## Dışa aktarılan dosyalar

Dışa aktarma, telefonun paylaşım menüsünü açar; dosyayı e-posta, WhatsApp, Dosyalar, Google
Drive vb. ile gönderebilir veya kaydedebilirsiniz.

| Mod | Dosya | İçerik |
|---|---|---|
| Karekod Sayım | `.txt` | Her satırda bir karekod (okunduğu haliyle) |
| Karekod Sayım | `.xlsx` | Barkod, ilaç adı, seri no, parti no, SKT, SKT durumu, fiyat, okunma zamanı |
| Barkod Sayım | `.txt` | Her barkod adedi kadar alt alta |
| Barkod Sayım | `.xlsx` | Barkod, ürün adı, adet, birim fiyat |
| Karşılaştırma | `.txt` | Eksik veya fazla karekodlar, her satırda bir karekod |
| Karşılaştırma | `.xlsx` | Durum (eksik/fazla/eşleşti), barkod, ilaç adı, seri no, parti no, SKT |
| Birleştirme | `.txt` / `.xlsx` | Birleşik karekod ve barkod listeleri |

## Ücretsiz sürüm ve abonelik

| Özellik | Ücretsiz | Tam sürüm |
|---|---|---|
| İlaç Bilgi | ✓ | ✓ |
| Karekod Sayım | En fazla 30 karekod | Sınırsız |
| Barkod Sayım | – | ✓ |
| Karekod Karşılaştırma | – | ✓ |
| Sayım Birleştirme | – | ✓ |

Tam sürüm **yıllık, otomatik yenilenen bir aboneliktir.** Ücret App Store veya Google Play
hesabınızdan alınır. Abonelik, dönem bitiminden en az 24 saat önce iptal edilmezse otomatik
olarak yenilenir.

- **İptal / yönetim:** Uygulamada Ayarlar → Tam sürüm etkin → **Yönet**, ya da
  - iPhone/iPad: Ayarlar → [adınız] → Abonelikler
  - Android: Google Play → Profil → Ödemeler ve abonelikler → Abonelikler
- **Yeni cihaz / yeniden yükleme:** Ayarlar → **Satın alımları geri yükle**. Aboneliği satın
  aldığınız Apple ID / Google hesabıyla oturum açmış olmanız gerekir.

## Kamera ipuçları

- **Flaş:** Karanlık raflarda kamera ekranındaki **Flaş** düğmesini kullanın.
- **Zoom:** Küçük karekodlar için **Zoom** düğmesiyle 2x veya 3x yakınlaştırın. Bazı telefonlar
  çok yakına odaklanamaz; kamerayı 15–25 cm uzakta tutup yakınlaştırmak daha iyi sonuç verir.
- **Odak:** Görüntüde bir noktaya dokunarak oraya odaklayabilirsiniz.
- **Siyah karekod (Android):** Bazı kutularda karekod siyah zemin üzerine beyaz basılıdır. Android'de bu
  kodlar okunmuyorsa kamera ekranındaki **Siyah Karekod** düğmesini açın. Pil tüketimini biraz
  artırdığı için yalnızca gerektiğinde açmanız önerilir. iPhone/iPad bu kodları ayarsız okur.
- **Pil tasarrufu:** 60 saniye boyunca hiç kod görülmezse kamera durur; devam etmek için ekrana
  dokunun.
- Karekod parlak ambalaj üzerindeyse yansımayı önlemek için kamerayı hafif eğik tutun.

## Sık sorulan sorular

**Kamera açılmıyor.**
Uygulamaya kamera izni verilmemiş olabilir. iPhone/iPad: Ayarlar → EczaStok → Kamera.
Android: Ayarlar → Uygulamalar → EczaStok → İzinler → Kamera.

**Okutma sesi gelmiyor.**
Uygulamada Ayarlar → **Okutma sesi** açık olmalı ve cihazın ses seviyesi kısık olmamalıdır.
Ses yalnızca listeye yeni bir kod eklendiğinde çalar; daha önce okunmuş kutuda çalmaz.

**İlaç adı görünmüyor, "Listede bulunamadı" yazıyor.**
İlaç fiyat listesi henüz inmemiş veya ilaç listede bulunmuyor olabilir. Ayarlar → **İlaç
verilerini güncelle** ile tekrar deneyin. Sayım işlemi ilaç adı olmadan da çalışır.

**Sayım listem kayboldu mu?**
Listeler cihazda saklanır ve uygulama kapansa da korunur. Uygulamayı silerseniz listeler de
silinir; önemli sayımları dışa aktarmayı unutmayın.

**Eczane programım dosyayı kabul etmiyor.**
Programınızın beklediği biçimi bize örnek bir dosyayla iletin:
[gokrememre@gmail.com](mailto:gokrememre@gmail.com)

---

© 2026 Emre Gökrem · EczaStok
