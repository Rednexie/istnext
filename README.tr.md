# istnext (eski adıyla iettnext)

> **"16 milyonu verisine kavuşturuyoruz."**

**v2:** [istnext.com.tr/app](https://istnext.com.tr/app)



**v1:** [iett.rednexie.workers.dev](https://iett.rednexie.workers.dev)



🇬🇧 [English README](./README.md)

---

## Hakkında
istnext, İstanbul'un toplu taşıma veri kaynaklarını modern, açık kaynaklı, hızlı bir arayüzden erişilebilir hale getirmeyi amaçlayan bir projedir.

> [!Caution]
> istnext, İstanbul Büyükşehir Belediyesi (İBB) veya İETT'nin resmi bir uygulaması ya da hizmeti **değildir**.

> [!Caution]
>  Önceden sunulan bazı özellikler ve bilgiler, İBB ilgili verileri paylaşmayı bıraktığı için artık sağlanmamaktadır. Bu nedenle bazı özellikler kısıtlı olabilir, kullanılamayabilir veya zamanla kaldırılabilir.

---

## Özellikler

### Araç Sorgulama (`/app/arac`)
- **Kapı kodu** veya **plaka** ile canlı İETT, ÖHO ve Otobüs A.Ş. araçlarını dilediğince sorgula.
- Anlık GPS konumu, hız, model ve teknik/filo bilgilerine eriş.
- Aracın konumunu haritada görüntüle.
- Araçları sonradan da sorgulayabilmek için favorilere kaydet.
- Bilgileri uygulamayı kullanmayanlarla da paylaş: cihazda paylaş, WhatsApp, Markdown kopyala, metin kopyala, paylaşım bağlantısı

### Yolculuk: Durak ve Hat Sorgulama (`/app/yolculuk`)
- **Durak arama:** durak bilgileri ve yaklaşan otobüslerin canlı varış süreleri
- **Hat arama:** güzergâh, sefer saatleri (kalkış), hattaki canlı araçlar ve hat bilgisi
- Durakta yön değiştirme ve hat filtreleme
- Durak ve hat duyuruları, duyuruları paylaşma
- Durak ve hat favorileri
- Çevrimdışı mod: bağlantı yokken önceden kaydedilmiş veriler gösterilir

### Ana Sayfa (`/app`)
- Durak, Hat, Araç ve Keşfet'e hızlı erişim
- **Trafik durumu:** trafik endeksi ile Avrupa ve Anadolu yakası yüzdeleri
- **Şehir duyuruları:** Tümü / Güzergâh-Yol / Sefer İptalleri filtreleri
- **Kısayollarım:** kayıtlı favori durak, hat ve araçlar
- **Baraj Bilgileri**: İstanbul'daki barajların su seviyeleri

### Keşfet ve Veri Merkezi (`/app/kesfet`)
- Açık veri istatistikleri, metro hat güzergâhları, yakıt tüketimi, arşiv seferleri ve anlık duyurular
- Eski hatlar ve arşiv: geçmiş yılların hat verileri, kaldırılan rotalar ve arşivlenmiş sefer kayıtları

---

## Gizlilik (özet)

- **Konum:** cihaz konumunuz yalnızca yakındaki durak özellikleri için tarayıcı belleğinde geçici olarak işlenir, sunucuya kaydedilmez.
- **Local Storage:** yalnızca tema ve favori durak/hat tercihleriniz için kullanılır. Reklam çerezi veya profilleme yoktur.
- **Güvenlik verileri:** güvenlik, bot engelleme ve anonim istatistikler için IP adresiniz ve temel cihaz verileriniz işlenebilir.
- **Altyapı:** ağ güvenliği ve hızlı hizmet için Cloudflare kullanılır.

Tam metin için web sitesindeki *Gizlilik Politikası* ve *Kullanım Koşulları* bölümlerine göz atabilirsiniz.

---

## Veri Kaynakları ve Doğruluk

Araç konumları, sefer bilgileri, durak verileri ve diğer istatistikler, [İBB Açık Veri Portalı](https://data.ibb.gov.tr/) dahil çeşitli açık veri kaynaklarından derlenir. Daha önce paylaşılan bazı veriler İBB tarafından artık sağlanmadığından, ilgili özellikler ve bilgiler kullanılamamaktadır. Verilerin gecikmesinden, hatalı gelmesinden veya eksikliğinden istnext sorumlu tutulamaz. Hizmet "olduğu gibi" sunulur ve kesintisiz çalışma garantisi verilmez.

---

## Teknoloji

- **Sunucu Runtime'ı:** Cloudflare Workers
- **Veritabanı:** PostgreSQL
- **Dil:** TypeScript
- **Web Arayüzü:** HTML, JavaScript, CSS

---

## Katkıda Bulunma

- Problemler için -> issue
- Kod değişiklikleriniz için -> pull request 
- Özellik önerileri, tartışma, muhabbet için -> discussions

---

## Lisans

Bu projenin kaynak kodu **MIT Lisansı** ile lisanslanmıştır. Ayrıntılar için [LICENSE](./LICENSE) dosyasına göz atabilirsiniz.

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
