# Mini Oyun ve Skor Platformu 🎮

Bu proje, Node.js kullanılarak geliştirilmiş interaktif bir mini oyun platformudur. Kullanıcılar sisteme kayıt olup giriş yapabilir, platformdaki mini oyunları oynayarak skorlarını kaydedebilir ve rekabetçi liderlik sıralamasında yer alabilirler. Aynı zamanda kullanıcıların kendi bilgilerini düzenleyebildiği ve sistemi yönetmek için gelişmiş bir admin paneli barındıran dinamik bir yapıya sahiptir.

## 📂 Proje Yapısı

```text
PROJE_KLASORU/
│
├── Database/          # Kullanıcı, skor ve oyun verilerinin saklandığı yerel veritabanı dizini
├── public/            # Tarayıcıda listelenen statik dosyalar (Oyunlar, HTML, CSS, istemci JS)
├── src/               # Arka plan (backend) mantığı, skor hesaplamaları ve yardımcı kodlar
│
├── server.js          # Projenin ana Node.js sunucu dosyası
├── package.json       # Proje bağımlılıkları, scriptler ve meta veriler
└── package-lock.json  # Kurulan paketlerin kilitli ve birebir sürüm detayları
```

## 🛠️ Gereksinimler ve Kurulum

Projeyi yerel bilgisayarınızda kurmak ve çalıştırmak için aşağıdaki adımları sırasıyla takip edin:

### 1. Node.js Kurulumu
Bilgisayarınızda Node.js kurulu değilse, terminali (PowerShell) açarak tarayıcıya gerek kalmadan şu komutla doğrudan yükleyebilirsiniz:

winget install OpenJS.NodeJS.LTS

*(Not: Kurulum bittikten sonra terminali kapatıp projenizin dizininde yeniden açmanız gerekir.)*

### 2. Proje Dosyalarını Hazırlama
Bu depoyu bilgisayarınıza klonlayın veya ZIP olarak indirip çıkartın. Ardından terminalinizi projenin ana dizininde açın.

### 3. PowerShell İzinlerinin Ayarlanması (Olası Hatalar İçin)
Eğer bir sonraki adımda `npm` komutlarını çalıştırırken script engelleme (UnauthorizedAccess) hatası alırsanız, sistemin bu script'i çalıştırmasına izin vermek için şu komutu uygulayın:

Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser


### 4. Bağımlılıkların Yüklenmesi
Projenin ihtiyaç duyduğu tüm paketleri ve modülleri yüklemek için proje klasörünün içindeyken şu komutu çalıştırın:

npm install


## 🚀 Sunucuyu Başlatma

Kurulumlar tamamlandıktan sonra yerel sunucuyu (server) ayağa kaldırmak ve projeyi çalıştırmak için terminalde şu komutu yürütmeniz yeterlidir:


node server.js


Sunucu başarıyla başladıktan sonra tarayıcınızı açıp, kodunuzda ayarlı olan port üzerinden (örneğin `http://localhost:3000`) platforma ve oyunlara erişebilirsiniz.

## 🔐 Yönetici (Admin) Giriş Bilgileri

Sistemdeki admin paneline erişmek, kullanıcıları veya skorları yönetmek için tanımlanmış varsayılan giriş kimlik bilgileri aşağıdadır:

* **Kullanıcı Adı:** `admin123`
* **Şifre:** `admin123`

## ✨ Öne Çıkan Özellikler

* **🎮 Mini Oyunlar ve Skor Takibi:** Kullanıcılar platformdaki mini oyunları oynayabilir ve elde ettikleri skorlar anlık olarak sisteme kaydedilir.
* **🏆 Liderlik Sıralaması (Leaderboard):** Kaydedilen en yüksek skorlar, kullanıcılar arasında rekabet yaratmak amacıyla liderlik tablosunda listelenir.
* **👤 Profil Yönetimi ve Güncelleme:** Sisteme kayıtlı kullanıcılar kendi profillerine erişebilir ve kişisel bilgilerini diledikleri zaman güncelleyebilirler.
* **🔐 Admin Kontrol Paneli:** Özel yetkili yöneticiler için verileri, kullanıcıları ve genel sistemi kontrol edebilecekleri özel bir panel bulunur.
* **💾 JSON Tabanlı Veri Kaydı:** Tüm kullanıcı, şifre ve skor verileri hafif ve hızlı bir yapı olan JSON formatında işlenerek `Database` klasöründe güvenle saklanır.
