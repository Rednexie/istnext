# istnext (eski adıyla iettnext)

> Gerçek zamanlı İstanbul toplu taşıma araç takibi ve şehir verileri platformu.
> **"16 milyonu verisine kavuşturuyoruz."**

**v2:** [istnext.com.tr/app](https://istnext.com.tr/app)



**v1:** [iett.rednexie.workers.dev](https://iett.rednexie.workers.dev)



🇬🇧 [English README](./README.md)

---

## Hakkında

istnext, İstanbul'un toplu taşıma ve şehir verilerini tek bir hızlı arayüzde buluşturan bağımsız ve açık kaynaklı bir projedir. Otobüsleri canlı takip edebilir, durak ve hat sorgulayabilir, araç bilgilerine ulaşabilir ve şehir istatistiklerini keşfedebilirsiniz.

> [!Caution]
> **Uyarı:** istnext, İstanbul Büyükşehir Belediyesi (İBB) veya İETT'nin resmi bir uygulaması ya da hizmeti **değildir**. Bağımsız geliştiriciler tarafından hazırlanmıştır.

> [!Caution]
> **Veri erişilebilirliği notu:** Daha önce sunulan bazı özellikler ve bilgiler, İBB ilgili verileri paylaşmayı bıraktığı için artık sağlanmamaktadır. Bu nedenle bazı özellikler kısıtlı olabilir, kullanılamayabilir veya zamanla kaldırılabilir.

---

## Özellikler

### 🚍 Araç Sorgulama (`/app/arac`)
- **Kapı kodu** veya **plaka** ile canlı İETT, ÖHO ve Otobüs A.Ş. araçlarını sorgulama
- Anlık GPS konumu, hız, model ve teknik/filo bilgileri
- Aracın konumunu haritada görme ve Google Maps'te açma
- Favori araçlar
- Araç kartını paylaşma: cihazda paylaş, WhatsApp, Markdown kopyala, metin kopyala, paylaşım bağlantısı
- "İETT'de Gör" kısayolu

### 🚏 Yolculuk: Durak ve Hat Sorgulama (`/app/yolculuk`)
- **Durak arama:** durak bilgileri ve yaklaşan otobüslerin canlı varış süreleri
- **Hat arama:** güzergâh, sefer saatleri (kalkış), hattaki canlı araçlar ve hat bilgisi
- Durakta yön değiştirme ve hat filtreleme
- Durak ve hat duyuruları, duyuruları paylaşma
- Hat türü göstergeleri: ÖHO (kırmızı) ve İETT (normal)
- Durak ve hat favorileri
- Çevrimdışı mod: bağlantı yokken önceden kaydedilmiş veriler gösterilir

### 🏠 Ana Sayfa (`/app`)
- Durak, Hat, Araç ve Keşfet'e hızlı erişim
- **Trafik durumu:** trafik endeksi ile Avrupa ve Anadolu yakası yüzdeleri
- **Şehir duyuruları:** Tümü / Güzergâh-Yol / Sefer İptalleri filtreleri
- **Kısayollarım:** kayıtlı favori durak, hat ve araçlar
- **Senkronizasyon anahtarı:** hesap açmadan, kişisel anahtarla (`IST-XXXX-XXXX-XXXX` biçimi) favorilerinizi cihazlar arasında taşıma

### 🧭 Keşfet ve Veri Merkezi (`/app/kesfet`)
- Açık veri istatistikleri, metro hat güzergâhları, yakıt tüketimi, arşiv seferleri ve anlık duyurular
- Eski hatlar ve arşiv: geçmiş yılların hat verileri, kaldırılan rotalar ve arşivlenmiş sefer kayıtları
- Şehir bilgileri: İstanbul baraj doluluk oranları, canlı trafik yoğunluğu ve güncel kent verileri
- Resmi kaynak sayfalara bağlantılar

### 📱 PWA
- Cihaza uygulama olarak yüklenebilir; daha hızlı ve tam ekran deneyim
- İsteğe bağlı lansman bildirimleri
- Karanlık ve aydınlık tema

---

## Gizlilik (özet)

- **Konum:** cihaz konumunuz yalnızca yakındaki durak özellikleri için tarayıcı belleğinde geçici olarak işlenir, sunucuya kaydedilmez.
- **Local Storage:** yalnızca tema ve favori durak/hat tercihleriniz için kullanılır. Reklam çerezi veya profilleme yoktur.
- **Güvenlik verileri:** güvenlik, bot engelleme ve anonim istatistikler için IP adresiniz ve temel cihaz verileriniz işlenebilir.
- **Altyapı:** ağ güvenliği ve hızlı hizmet için Cloudflare kullanılır.

Tam metin için web sitesindeki *Gizlilik Politikası* ve *Kullanım Koşulları* bölümlerine bakın.

---

## Veri Kaynakları ve Doğruluk

Araç konumları, sefer bilgileri, durak verileri ve diğer istatistikler, [İBB Açık Veri Portalı](https://data.ibb.gov.tr/) dahil çeşitli açık veri kaynaklarından derlenir. Daha önce paylaşılan bazı veriler İBB tarafından artık sağlanmadığından, ilgili özellikler ve bilgiler kullanılamamaktadır. Verilerin gecikmesinden, hatalı gelmesinden veya eksikliğinden istnext sorumlu tutulamaz. Hizmet "olduğu gibi" sunulur ve kesintisiz çalışma garantisi verilmez.

---

## Teknoloji

- **Çalışma ortamı / Barındırma:** Bun.js
- **Veritabanı:** PostgreSQL
- **Dil:** TypeScript
- **Ön yüz:** HTML, JavaScript, CSS

---

## Katkıda Bulunma

Issue ve pull request'ler memnuniyetle karşılanır. Büyük değişiklikler için önce bir issue açarak konuşalım.

---

## Lisans

Bu projenin kaynak kodu **MIT Lisansı** ile lisanslanmıştır. Ayrıntılar için [LICENSE](./LICENSE) dosyasına bakın.

İBB Açık Veri Portalı'ndan alınan veriler kendi kullanım koşullarına tabidir: [data.ibb.gov.tr/license](https://data.ibb.gov.tr/license).

---

## Değişiklik Günlüğü

### v2.0.1
- Baraj bilgileri desteği eklendi
- Eski hat verileri geri geldi
- Araç bilgi sayfasındaki sorun düzeltildi

### v2.0.0
- Progressive Web App (PWA) desteği eklendi
- Keşfet sayfasındaki metrikler bölümü genişletildi
- Sorgu sonuçları için biçimlendirilmiş paylaşım eklendi
- Aydınlık tema eklendi

### v1 — iettnext
- İlk sürüm, [iett.rednexie.workers.dev](https://iett.rednexie.workers.dev) adresinde hâlâ kullanılabilir
