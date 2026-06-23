# Mini Oyun ve Skor Platformu 🎮

Bu proje, Node.js kullanılarak geliştirilmiş interaktif bir mini oyun platformudur. Kullanıcılar sisteme kayıt olup giriş yapabilir, platformdaki mini oyunları oynayarak skorlarını kaydedebilir ve rekabetçi liderlik sıralamasında yer alabilirler. Aynı zamanda kullanıcıların kendi bilgilerini düzenleyebildiği ve sistemi yönetmek için gelişmiş bir admin paneli barındıran dinamik bir yapıya sahiptir.

## 📂 Proje Yapısı

\`\`\`text
PROJE_KLASORU/
│
├── Database/          # Kullanıcı, skor ve oyun verilerinin saklandığı yerel veritabanı dizini
├── public/            # Tarayıcıda listelenen statik dosyalar (Oyunlar, HTML, CSS, istemci JS)
├── src/               # Arka plan (backend) mantığı, skor hesaplamaları ve yardımcı kodlar
│
├── server.js          # Projenin ana Node.js sunucu dosyası
├── package.json       # Proje bağımlılıkları, scriptler ve meta veriler
└── package-lock.json  # Kurulan paketlerin kilitli ve birebir sürüm detayları
\`\`\`

## 🛠️ Gereksinimler ve Kurulum

Projeyi yerel bilgisayarınızda çalıştırmak için sisteminizde **Node.js** yüklü olmalıdır.

1. Bu depoyu bilgisayarınıza klonlayın veya ZIP olarak indirin.
2. Terminalinizi (veya Git Bash) projenin ana dizininde açın.
3. Gerekli tüm paketleri kurmak için şu komutu çalıştırın:
 
   npm install
 

## 🚀 Sunucuyu Başlatma

Kurulum tamamlandıktan sonra yerel sunucuyu ayağa kaldırmak ve projeyi çalıştırmak için terminalde şu komutu yürütmeniz yeterlidir:


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
