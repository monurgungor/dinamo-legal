# Gizlilik Politikası ve KVKK Aydınlatma Metni

**Yürürlük tarihi:** 5 Haziran 2026
**Son güncelleme:** 5 Haziran 2026
**Politika sürümü:** 2.0

Bu metin, Dinamo iOS uygulamasının ("Dinamo", "uygulama") kullanıcılarının kişisel verilerinin nasıl işlendiğine ilişkin, 6698 sayılı Kişisel Verilerin Korunması Kanunu ("KVKK") kapsamında hazırlanmış **aydınlatma metni** ve gizlilik politikasıdır. Avrupa Birliği'nde bulunan kullanıcılar bakımından, uygulanabildiği ölçüde Genel Veri Koruma Tüzüğü ("GDPR") da gözetilmiştir. Lütfen uygulamayı kullanmadan ve herhangi bir veri paylaşımına izin vermeden önce dikkatlice okuyunuz.

---

## 0. Özet — 30 saniyede neyi kabul ediyorsunuz?

- Dinamo'yu kullanmak için **hesap açmanıza, giriş yapmanıza veya ad-soyad/e-posta vermenize gerek yoktur.**
- Uygulamanın temel işlevi (yakındaki şarj istasyonlarını harita üzerinde bulmak, arama yapmak, **rota planlamak**) **hiçbir veri paylaşımı olmadan tam olarak çalışır.**
- **Sizi takip eden bir geçmiş/iz kaydı tutmuyoruz.** Kişiye bağlı bir konum izi veya kişiye özel bir profil **yoktur**. Topladığımız her şey **kimliksiz** ve **toplulaştırılmıştır.**
- Aşağıdaki iki seçenek yalnızca siz **açıkça izin verirseniz** devreye girer. İlk açılışta her biri için **ayrı ayrı**, **varsayılan olarak KAPALI** seçenekler sunulur:
  1. **Anonim kullanım istatistikleri** — özellikle **rota planlayıcı** kullanıldığında, hangi bölgeler arasında, hangi araçla plan yapıldığı; ayrıca hangi ekranların/aramaların popüler olduğu. Tümü **kimliğe bağlanmadan, il/ilçe düzeyine kabalaştırılarak ve toplulaştırılarak** kaydedilir.
  2. **Çökme ve tanılama verisi** — uygulamanın kararlılığını ölçmek için **Firebase Crashlytics** (Google) aracılığıyla. Açana kadar **hiç başlatılmaz**.
- **Rota planlayıcının başlangıç noktası varsayılan olarak anlık konumunuzdur**; ama analitik kaydı yapılmadan **önce** il/ilçe düzeyine kabalaştırılır — ham koordinatınız hiçbir zaman kaydedilmez.
- Verdiğiniz her izni **istediğiniz zaman Ayarlar'dan geri alabilirsiniz**; izni kapatmak gelecekteki toplamayı **derhal durdurur.**
- **Reklam yok, reklam takibi (IDFA) yok, ATT izleme izni yok, veri satışı yok, üçüncü taraflarla pazarlama amaçlı paylaşım yok.**

Bu özet bilgilendirme amaçlıdır; bağlayıcı olan aşağıdaki tam metindir.

---

## 1. Veri Sorumlusu (KVKK m. 10/1-a)

Bu uygulama bir kurumsal şirket tarafından değil, **Mehmet Onur Güngör** adlı **gerçek kişi** tarafından kişisel proje olarak yayınlanmaktadır. KVKK anlamında **veri sorumlusu** bu gerçek kişidir.

- **Veri sorumlusu:** Mehmet Onur Güngör (gerçek kişi)
- **Adres:** İstanbul, Türkiye
- **İletişim e-postası:** monurgungor6@gmail.com

KVKK kapsamındaki tüm başvurularınızı ve gizlilikle ilgili sorularınızı yukarıdaki e-posta adresine iletebilirsiniz.

---

## 2. Hangi Verileri, Hangi Amaçla İşliyoruz? (KVKK m. 10/1-b, m. 4)

> **Önemli — neyi YAPMIYORUZ:** Dinamo'da sizi takip eden bir "şarj geçmişi" özelliği **yoktur**. Cihazınıza bağlanmış kalıcı bir konum izi veya kişiye özel bir profil **tutmuyoruz**. Uygulama, gerçek şarj olaylarını **gözlemleyemez ve gözlemlemez** — bunu yapacak bir özellik yoktur. Yalnızca uygulama içindeki kullanıcı eylemlerini (en zengini rota planlayıcı olmak üzere) **kimliksiz ve toplu** olarak ölçeriz.

### 2.0 Temel işlev — anlık konum (kalıcı saklanmaz, izne tabi değildir)

- **İşlenen veri:** Anlık konum.
- **Amaç:** (1) Yakındaki şarj istasyonlarını haritada göstermek; (2) rota planlayıcının başlangıç noktasını belirlemek.
- **Yöntem:** Yalnızca uygulama açık ve kullanımdayken. Arka planda konum **toplanmaz**; "Her Zaman (Always)" izni **istenmez.**
- **Saklama:** Kalıcı olarak **saklanmaz.** Sizi takip eden bir iz oluşturulmaz.
- **Hukuki sebep:** Hizmetin ifası (KVKK m. 5/2-c).

> **Şeffaflık notu (rota planlayıcı + analitik):** Rota planlayıcının başlangıç noktası çoğu zaman **hassas anlık konumunuzdur.** Bu yüzden, **eğer analitiğe izin vermişseniz**, bu nokta herhangi bir kayıt yapılmadan **önce** il/ilçe düzeyine **kabalaştırılır** ve ancak kimliksiz olarak işlenir (bkz. 2.1). Analitiğe izin vermediyseniz hiçbir rota verisi gönderilmez.

### 2.1 Anonim kullanım istatistikleri (isteğe bağlı — varsayılan KAPALI)

**(a) Rota planlama istatistikleri.** Rota planlayıcı çalıştırıldığında: **Başlangıç BÖLGESİ** ve **varış BÖLGESİ** (ham koordinat değil; il/ilçe düzeyine kabalaştırılmış), seçilen **araç**, **tercih** (en hızlı/en ucuz) ve **önerilen istasyonlar**. Hiçbir kalıcı kimlik eklenmez; sunucuda kimliksiz ve toplulaştırılmış olarak saklanır. Ender kombinasyonlar k-anonimlik eşiğiyle bastırılır; zaman bilgisi gün düzeyine kabalaştırılır.

**(b) Etkileşim istatistikleri.** İstasyon görüntüleme, arama, yakındakiler sorgusu, filtre kullanımı, ekran görüntülemeleri — kimliksiz sayılar, ham koordinat yok.

- **Hukuki sebep:** Veriler anonim olduğundan KVKK kapsamı dışındadır (m. 28/1-b). Buna rağmen şeffaflık ve Apple etiketi dürüstlüğü için **açık izninize tabi tutulmuştur**, varsayılan KAPALI.
- **Anonimlik teminatı:** Kabalaştırma cihazda yapılır, kimlik eklenmez, k-anonimlik uygulanır. Bu güvenceler geçersizleşirse toplama **durdurulur.**

### 2.2 Çökme ve tanılama verisi — Firebase Crashlytics (isteğe bağlı — varsayılan KAPALI)

- **İşlenen veri:** Çökme yığın izleri, uygulama/işletim sistemi sürümü, cihaz modeli ve bir **Firebase kurulum kimliği**. Google LLC'ye (ABD) iletilir.
- **Kimliğe bağlı:** **Evet** — Firebase kurulum kimliği kalıcı bir tanımlayıcıdır.
- **Başlatma:** Siz açana kadar **başlatılmaz** (`FirebaseCrashlyticsCollectionEnabled = false`). Reklam/Analytics bileşenleri dahil edilmediğinden IDFA ve ATT izni **gerekmez.**
- **Saklama:** Google'da yaklaşık **90 gün.**
- **Hukuki sebep:** Açık rıza (KVKK m. 5/1).

### 2.3 Sunucu istek kayıtları

IP adresi gibi alanlar mümkün olduğunca redakte edilir; loglar analitik kaynağı olarak kullanılmaz. Amaç: kötüye kullanım önleme ve hata teşhisi (KVKK m. 5/2-f, m. 12).

---

## 3. Verilerin Kimlere Aktarılabileceği (KVKK m. 10/1-c)

| Alıcı | Rolü | Ne görür? |
|---|---|---|
| **Railway Corp.** (Frankfurt, Almanya — AB) | Veri işleyen (barındırma) | Anonim istatistikleri barındırır; kişisel konum geçmişi **saklanmaz.** |
| **Google LLC** (ABD) — Firebase Crashlytics | Veri işleyen (çökme/tanılama) | Yalnızca izin açıksa: çökme verisi + Firebase kurulum kimliği. |
| **Mapbox, Inc.** (ABD) | Bağımsız sağlayıcı | Harita yüklenirken IP adresinizi görür. Mapbox analitik telemetrisi devre dışı. |
| **EPDK** (Türkiye) | Kamu veri kaynağı | Yalnızca sunucu IP'mizi görür, sizinkini görmez. |

Pazarlama amaçlı hiçbir üçüncü taraf reklam/izleme SDK'sı kullanılmamaktadır.

---

## 4. Yurt Dışına Veri Aktarımı (KVKK m. 9 — 7499 sayılı Kanun, yürürlük 01.06.2024)

Üç alıcıya yurt dışı aktarım söz konusudur: Railway (Almanya), Mapbox (ABD), Google/Firebase (ABD). Bu aktarımlar "uygulamayı kullanmaya devam etmeniz = onay" gibi zımni bir onaya **dayandırılmamaktadır.**

Aktarım temeli: Kurul onaylı **standart sözleşme** ve/veya sağlayıcıların DPA/SCC taahhütlerinin bu çerçeveye oturtulması; imzadan itibaren **5 iş günü içinde Kurul'a bildirim.** (AB veya ABD için yeterlilik kararı bulunmamaktadır.)

---

## 5. Veri Saklama Süreleri

| Veri türü | Saklama |
|---|---|
| Anlık konum | Saklanmaz |
| Anonim istatistikler (ham) | Birkaç gün; toplulaştırılıp ham kayıtlar silinir |
| Anonim istatistikler (toplu) | Süresiz (anonim veri) |
| Firebase Crashlytics | ~90 gün (Google) |
| Sunucu logları | Kısa süreli; IP redakte edilir |

---

## 6. İzni Geri Alma ve Verilerin Silinmesi (KVKK m. 7, m. 11)

1. **İzni geri alma:** Her iki seçeneği Ayarlar'dan istediğiniz zaman kapatabilirsiniz; gelecekteki toplama **derhal durur.**
2. **Anonim istatistikler:** Kimliksiz ve toplulaştırılmış olduğundan size ait bir kayıt yoktur. Anlamlı silme = toplamayı durdurmaktır.
3. **Crashlytics verisi:** Tanılama iznini kapatmanız toplamayı durdurur. Halihazırda Google'da tutulan kayıtların silinmesini monurgungor6@gmail.com adresine e-posta ile talep edebilirsiniz; talebiniz 30 gün içinde yanıtlanır.

---

## 7. Haklarınız (KVKK m. 11, GDPR m. 15-22)

Kişisel verinizin işlenip işlenmediğini öğrenme, bilgi talep etme, düzeltme, silme, aktarım, itiraz ve tazminat talep etme haklarına sahipsiniz. Başvuru için: monurgungor6@gmail.com (30 gün içinde yanıt).

---

## 8. Açık Rıza ve Niteliği

Kişisel veri içeren işleme (Crashlytics) için hukuki temel açık rızadır. Rıza: **belirli** (ayrı toggle), **bilgilendirilmiş** (bu metin), **özgür irade** (tüm seçenekler varsayılan KAPALI; hiçbirini açmadan uygulama tam çalışır), **geri alınabilir** (Ayarlar'dan). Hizmetin kullanımı bu işlemelere izin verme koşuluna **bağlanmamıştır.**

---

## 9. Çocukların Gizliliği

4+ yaş derecelendirmesi vardır; 13 yaş altı çocuklara yönelik tasarlanmamıştır ve onlardan bilerek kişisel veri toplanmaz.

---

## 10. Veri Güvenliği (KVKK m. 12)

TLS/HTTPS şifrelemesi; koordinatlar analitik kaydından önce kabalaştırılır; loglarda IP redakte edilir; Crashlytics izin açılana kadar başlatılmaz. Veri ihlali hâlinde Kurul'a 72 saat içinde bildirim yapılır.

---

## 11. VERBİS

Veri sorumlusu, Kurul 2023/1154 sayılı kararındaki istisna kriterlerinin (50'den az çalışan, 100 milyon TL altı bilanço, özel nitelikli veri işleme ana faaliyet değil) altında kalan bir gerçek kişidir; VERBİS kaydından büyük olasılıkla muaftır. Tüm KVKK yükümlülükleri geçerliliğini korur.

---

## 12. Politikadaki Değişiklikler

Toplanan veri kapsamını genişleten önemli değişikliklerde "kullanmaya devam etmeniz = onay" yaklaşımına dayanmayız; yeniden bilgilendirip gerektiğinde açık rızanızı yeniden alırız.

---

## 13. İletişim

**Veri sorumlusu:** Mehmet Onur Güngör (İstanbul, Türkiye)
**E-posta:** monurgungor6@gmail.com

---
---

# Privacy Policy and Data Protection Notice

**Effective date:** June 5, 2026
**Last updated:** June 5, 2026
**Policy version:** 2.0

This document is the disclosure notice and privacy policy explaining how the Dinamo iOS app ("Dinamo", "the app") handles users' personal data, prepared in compliance with Turkey's Personal Data Protection Law No. 6698 ("KVKK"). For users in the EU, the GDPR is also observed where applicable.

---

## 0. Summary — 30 seconds

- You **do not need an account or any personal details** to use Dinamo.
- The core app (map, search, route planning) **works fully with no data sharing.**
- **No history or trail follows you.** No device-keyed location trail, no personal profile. Everything we collect is **id-less and aggregated.**
- Two options activate **only with your explicit opt-in** — both **default OFF:**
  1. **Anonymous usage analytics** — route-plan areas, vehicle, preference, station suggestions, screen/search counts. Id-less, coarsened to city/district, aggregated.
  2. **Crash & diagnostics** — via **Firebase Crashlytics** (Google). Never started until you turn it on.
- The route planner's **origin defaults to your precise location** but is **coarsened before any logging** — raw coordinates are never stored.
- Revoke any consent **anytime in Settings**; turning a toggle off **immediately stops** collection.
- **No ads, no IDFA, no ATT prompt, no data sale.**

---

## 1. Data Controller

**Mehmet Onur Güngör** (an individual, not a company) — İstanbul, Türkiye — monurgungor6@gmail.com.

---

## 2. What We Process and Why

> **What we do NOT do:** No "charging history" feature. No persistent device-keyed location trail. No per-user store. The app cannot observe real charging events — there is no such feature. We only measure in-app actions (primarily route planning) in id-less, aggregated form.

### 2.0 Core function — momentary location (not stored)

Used for: (1) nearby station display; (2) route planner origin. When-in-use only, no background, no Always permission. **Not persisted.** Legal basis: service performance (KVKK Art. 5/2-c).

> **Transparency note:** Route origin is often your precise current location. If you opted into analytics, it is **coarsened to city/district before any logging.** If you did not opt in, no route data is sent at all.

### 2.1 Anonymous usage analytics (optional — default OFF)

**(a) Route-plan analytics.** When you run the route planner: **origin AREA** and **destination AREA** (coarsened, not raw coordinates), **vehicle**, **preference** (fastest/cheapest), **suggested stations**. No persistent identifier. Stored id-less and aggregated. Rare combinations suppressed via k-anonymity; timestamps coarsened to the day. Output: market insight (popular corridors, destination demand, vehicle mix) — **not a per-user trip history.**

**(b) Interaction analytics.** Id-less counts: station views, searches, nearby queries, filter use, screen views. No coordinates.

Legal basis: anonymized data falls outside KVKK (Art. 28/1-b). Still opt-in for transparency. Anonymity guarantee: coarsening on-device, no identifier, k-anonymity suppression — if guarantee breaks, collection stops.

### 2.2 Crash & diagnostics — Firebase Crashlytics (optional — default OFF)

Crash stack traces, app/OS version, device model, and a **Firebase installation ID** sent to **Google LLC (USA)**. **Never started until you opt in** (`FirebaseCrashlyticsCollectionEnabled = false`). No ad/Analytics components → no IDFA, no ATT. Retention ~90 days (Google). Legal basis: explicit consent (KVKK Art. 5/1).

### 2.3 Server request logs

IP fields redacted where possible. Used only for abuse prevention and error diagnosis (KVKK Art. 5/2-f, Art. 12).

---

## 3. Recipients

| Recipient | Role | What it sees |
|---|---|---|
| **Railway Corp.** (Frankfurt, Germany — EU) | Data processor (hosting) | Anonymous aggregated analytics. No personal location history stored. |
| **Google LLC** (USA) — Firebase Crashlytics | Data processor (crash/diagnostics) | Only if opted in: crash data + Firebase installation ID. |
| **Mapbox, Inc.** (USA) | Independent provider | Your IP when map tiles load. Mapbox analytics telemetry disabled. |
| **EPDK** (Türkiye) | Public data source | Only our server's IP, never yours. |

No third-party advertising or tracking SDK is used.

---

## 4. International Data Transfers (KVKK Art. 9, Law 7499, in force 01.06.2024)

Transfers to Railway (Germany), Mapbox (USA), and Google/Firebase (USA). **Not** based on implied "continued use = consent." No adequacy decision for EU or USA. Legal basis: **appropriate safeguards** — Board-approved standard contract / DPA-SCC mapping with each recipient + notification to the Board within **5 business days** of execution.

---

## 5. Data Retention

| Data type | Retention |
|---|---|
| Momentary location | Not stored |
| Anonymous analytics (raw) | A few days; rolled up then deleted |
| Anonymous analytics (aggregated) | Indefinite (anonymous, Art. 28) |
| Firebase Crashlytics | ~90 days (Google default) |
| Server logs | Short; IP redacted |

---

## 6. Withdrawing Consent and Data Deletion

1. **Withdraw consent:** Turn either toggle off in Settings — future collection **immediately stops.**
2. **Anonymous analytics:** Id-less and aggregated, so no record identifies you. Meaningful erasure = stopping collection.
3. **Crashlytics data:** Turning the diagnostics toggle off stops collection. For records already at Google, email monurgungor6@gmail.com — we will action the deletion within 30 days.

---

## 7. Your Rights (KVKK Art. 11, GDPR Arts. 15-22)

Right to learn, access, correct, erase, object, and claim damages. Contact: monurgungor6@gmail.com (response within 30 days).

---

## 8. Explicit Consent

Legal basis for crash/diagnostics: explicit consent. It is **specific** (separate toggle), **informed** (this notice), **freely given** (all defaults OFF; core app fully functional without any consent), and **revocable** (Settings at any time). Service use is **not** conditioned on these non-essential processings.

---

## 9. Children's Privacy

4+ rating, not directed at children under 13. We do not knowingly collect personal data from children under 13.

---

## 10. Data Security (KVKK Art. 12)

TLS/HTTPS; origin/destination coarsened before logging; IP redacted from logs; Crashlytics not initialized until consent. Breach notification to the Board within 72 hours per Board decision 2019/10.

---

## 11. VERBİS

As an individual below Board threshold (2023/1154: <50 employees, <100M TL balance, no special-category processing as main activity), the controller is very likely exempt from registry. All KVKK obligations still apply.

---

## 12. Changes to This Policy

For material changes that expand data collection, we will re-inform you in-app and obtain explicit consent again rather than relying on continued use.

---

## 13. Contact

**Data controller:** Mehmet Onur Güngör (İstanbul, Türkiye)
**Email:** monurgungor6@gmail.com
