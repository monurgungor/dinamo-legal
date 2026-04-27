# Gizlilik Politikası

**Yürürlük tarihi:** 27 Nisan 2026
**Son güncelleme:** 27 Nisan 2026

Bu metin, Dinamo iOS uygulamasının ("Dinamo", "uygulama") kullanıcılarının kişisel verilerinin nasıl işlendiğine ilişkin 6698 sayılı Kişisel Verilerin Korunması Kanunu ("KVKK") kapsamında hazırlanmış aydınlatma metnidir. Lütfen uygulamayı kullanmadan önce dikkatlice okuyunuz.

## 1. Veri Sorumlusu

Bu uygulama bir kurumsal şirket tarafından değil, **Mehmet Onur Güngör** adlı gerçek kişi tarafından kişisel proje olarak yayınlanmaktadır.

- **Adres:** İstanbul, Türkiye
- **TC Kimlik No (vergi kimlik no olarak):** 34633588246
- **İletişim e-posta:** monurgungor6@gmail.com

KVKK kapsamındaki tüm başvurularınızı yukarıdaki e-posta adresine iletebilirsiniz.

## 2. Topladığımız Veriler

Dinamo, yalnızca uygulamanın temel işlevini yerine getirebilmek için gerekli olan minimum veriyi işler:

- **Hassas konum (precise location)** — Yalnızca uygulama açık ve kullanımdayken, yakınınızdaki elektrikli araç şarj istasyonlarını harita üzerinde göstermek amacıyla. Bu veri cihazınızda veya sunucularımızda saklanmaz, üçüncü taraflarla paylaşılmaz.
- **Yaklaşık konum (coarse location)** — Hassas konuma erişim verilmediği veya kullanılamadığı durumlarda aynı amaçla kullanılır.

İzin metni: Uygulama yalnızca `NSLocationWhenInUseUsageDescription` (uygulama kullanımdayken konum) izni talep eder. Arka planda konum verisi toplanmaz.

## 3. Toplamadığımız Veriler

Şeffaflık adına, Dinamo'nun **toplamadığı** verileri açıkça beyan ederiz:

- Ad, soyad, e-posta, telefon numarası gibi kimlik veya iletişim bilgisi toplamayız.
- Kullanıcı hesabı, kayıt veya giriş sistemi v1.0.0 sürümünde aktif değildir.
- Hiçbir analitik (analytics) servisi kullanmıyoruz. Davranışsal izleme yapmıyoruz.
- Reklam SDK'sı, reklam tanımlayıcısı (IDFA) veya pazarlama izleyicileri kullanmıyoruz.
- Cihazınızda çerez (cookie) saklamayız.
- Fotoğraf, kamera, mikrofon, kişiler, takvim, sağlık verisi gibi hassas verilere erişim talep etmiyoruz.

## 4. Üçüncü Taraf Servisleri

Dinamo'nun çalışabilmesi için aşağıdaki üçüncü taraf servisler kullanılmaktadır:

- **Mapbox (Mapbox, Inc., ABD)** — Harita döşemelerini (map tiles) sunmak için kullanılır. Mapbox SDK'sının analitik telemetrisi `MGLMapboxMetricsEnabled = false` Info.plist anahtarı ile devre dışı bırakılmıştır. Ancak harita döşemeleri yüklenirken Mapbox sunucuları, herhangi bir harita SDK'sı için kaçınılmaz olduğu üzere IP adresinizi görür. Kişisel tanımlayıcı gönderilmez. Detay: https://www.mapbox.com/legal/privacy
- **EPDK (Enerji Piyasası Düzenleme Kurumu)** — sarjtr.epdk.gov.tr üzerinden kamuya açık olarak yayınlanan şarj istasyonu listesi kaynak olarak kullanılır. Bu veri, doğrudan cihazınızdan değil, Dinamo'nun arka uç (backend) sunucusu üzerinden çekilir. Yani EPDK yalnızca Dinamo sunucusunun IP'sini görür, sizin IP'nizi görmez.
- **Railway (Railway Corp., Frankfurt — AB)** — Dinamo'nun arka uç sunucusu Railway altyapısında, Almanya/Frankfurt bölgesinde barındırılır. Standart web sunucusu logları kapsamında istek IP adresleri 30 günden kısa süreyle, sadece kötüye kullanım önleme ve hız sınırlaması (rate limiting) amacıyla tutulur. Detay: https://railway.com/legal/privacy

## 5. Veri Saklama Süreleri

- Cihazınızda hiçbir kişisel veri kalıcı olarak saklanmaz.
- Arka uç sunucu logları en fazla 30 gün tutulur, ardından otomatik olarak silinir.
- Konum veriniz hiçbir zaman kalıcı olarak kaydedilmez; yalnızca yakındaki istasyon sorgusu için anlık olarak kullanılır.

## 6. Çocukların Gizliliği

Dinamo App Store'da 4+ yaş derecelendirmesine sahiptir, ancak özel olarak 13 yaş altı çocuklara yönelik tasarlanmamıştır. 13 yaş altı çocuklardan bilerek kişisel veri toplamayız.

## 7. Yurt Dışına Veri Aktarımı

Arka uç sunucumuz Avrupa Birliği üyesi ülke olan Almanya'nın Frankfurt bölgesinde bulunmaktadır. Konum sorgusu yapıldığında, koordinatlarınız işlenmek üzere bu sunucuya iletilir; ancak işlem tamamlandıktan sonra saklanmaz. Bu durum KVKK'nın 9. maddesi kapsamında yurt dışına veri aktarımı niteliğindedir ve uygulamayı kullanmanız bu aktarıma açık rızanız anlamına gelir.

## 8. Haklarınız

KVKK Madde 11 ve GDPR Madde 15-22 kapsamında aşağıdaki haklara sahipsiniz:

- Kişisel verinizin işlenip işlenmediğini öğrenme,
- İşlenmişse buna ilişkin bilgi talep etme,
- İşlenme amacını ve amacına uygun kullanılıp kullanılmadığını öğrenme,
- Yurt içinde/yurt dışında aktarıldığı üçüncü kişileri bilme,
- Eksik veya yanlış işlenmişse düzeltilmesini isteme,
- Silinmesini veya yok edilmesini isteme,
- Düzeltme/silme işleminin aktarıldığı üçüncü kişilere bildirilmesini isteme,
- Otomatik sistemlerle yapılan analiz sonucu aleyhinize bir sonuç çıkmasına itiraz etme,
- Hukuka aykırı işlenme nedeniyle zarara uğramanız halinde tazminat talep etme.

Bu haklarınızı kullanmak için monurgungor6@gmail.com adresine başvurabilirsiniz. Başvurunuza KVKK Madde 13 uyarınca en geç otuz (30) gün içinde yanıt verilir.

## 9. Politikadaki Değişiklikler

Bu gizlilik politikasını gerektiğinde güncelleyebiliriz. Önemli değişiklikler uygulama içinde duyurulur ve "Son güncelleme" tarihi her revizyonda güncellenir.

## 10. İletişim

KVKK kapsamındaki başvurularınız ve gizlilikle ilgili tüm sorularınız için:

**E-posta:** monurgungor6@gmail.com

---

# Privacy Policy

**Effective date:** April 27, 2026
**Last updated:** April 27, 2026

This document explains how the Dinamo iOS application ("Dinamo", "the app") handles your personal data. It is prepared in compliance with both Turkey's Personal Data Protection Law No. 6698 ("KVKK") and the EU General Data Protection Regulation ("GDPR"). Please read it carefully before using the app.

## 1. Who We Are

Dinamo is published as a personal project by an individual, not by an incorporated company. The data controller is **Mehmet Onur Güngör**, an individual residing in Türkiye.

- **Address:** İstanbul, Türkiye
- **National ID (used as tax identifier):** 34633588246
- **Contact email:** monurgungor6@gmail.com

You may contact us at the email address above for any privacy-related request.

## 2. What Data We Collect

Dinamo processes only the minimum data required to deliver its core function:

- **Precise location** — Used solely while the app is open and in use, in order to display nearby electric vehicle charging stations on the map. This data is never persisted on your device or on our servers, and is never shared with third parties.
- **Coarse location** — Used as a fallback when precise location is unavailable, for the same purpose.

The app requests only the `NSLocationWhenInUseUsageDescription` permission ("location while in use"). Background location is not collected.

## 3. What We Do NOT Collect

For full transparency, here is what Dinamo explicitly does **not** collect:

- We do not collect your name, surname, email address, phone number, or any other identifier.
- There is no user account, sign-up, or sign-in feature in v1.0.0.
- We use no analytics services. We perform no behavioral tracking.
- We use no advertising SDKs, no advertising identifiers (IDFA), and no marketing trackers.
- We store no cookies on your device.
- We do not request access to photos, camera, microphone, contacts, calendar, or health data.

## 4. Third-Party Services

Dinamo relies on the following third-party services to operate:

- **Mapbox (Mapbox, Inc., USA)** — Used to render map tiles. The app explicitly disables Mapbox's analytics telemetry via the `MGLMapboxMetricsEnabled = false` Info.plist key. However, when map tiles are loaded, Mapbox's servers will see your IP address — this is unavoidable for any map SDK. No personal identifier is sent. See: https://www.mapbox.com/legal/privacy
- **EPDK (Energy Market Regulatory Authority of Türkiye)** — The public list of EV charging stations published at sarjtr.epdk.gov.tr is used as the data source. This data is not fetched directly from your device; it is proxied through Dinamo's own backend. As a result, EPDK only sees the backend's IP, never yours.
- **Railway (Railway Corp., Frankfurt — EU)** — Dinamo's backend is hosted on Railway infrastructure in the Frankfurt, Germany region. Standard webserver logs may contain request IP addresses, retained for less than 30 days for the sole purpose of rate limiting and abuse prevention. See: https://railway.com/legal/privacy

## 5. Data Retention

- No personal data is permanently stored on your device.
- Backend webserver logs are retained for at most 30 days, then automatically deleted.
- Your location is never persisted; it is used only momentarily to query nearby stations.

## 6. Children's Privacy

Dinamo carries a 4+ age rating on the App Store but is not specifically directed at children under 13. We do not knowingly collect personal data from children under the age of 13.

## 7. International Data Transfers

Our backend is located in Frankfurt, Germany — an EU member state. When you query nearby stations, your coordinates are transmitted to this server for processing and are not retained afterwards. Under KVKK Article 9, this constitutes an international transfer of personal data; your continued use of the app constitutes explicit consent to this transfer.

## 8. Your Rights

Under KVKK Article 11 and GDPR Articles 15-22, you have the right to:

- Learn whether your personal data is being processed,
- Request information about the processing,
- Learn the purpose of processing and whether it is used in line with that purpose,
- Know the third parties to whom data has been transferred, domestically or abroad,
- Request correction of incomplete or inaccurate data,
- Request erasure or destruction of your data,
- Request that any correction or erasure be communicated to third parties,
- Object to outcomes derived from purely automated processing,
- Claim damages where unlawful processing has caused harm.

To exercise these rights, contact monurgungor6@gmail.com. Per KVKK Article 13, we will respond within thirty (30) days.

## 9. Changes to This Policy

We may update this privacy policy from time to time. Significant changes will be announced inside the app, and the "Last updated" date will be revised on each revision.

## 10. Contact

For all privacy-related questions and KVKK requests:

**Email:** monurgungor6@gmail.com
