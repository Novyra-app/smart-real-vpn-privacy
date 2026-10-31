# سياسة الخصوصية لتطبيق Smart Real VPN | Privacy Policy for Smart Real VPN

* **اسم التطبيق (Application Name):** Smart Real VPN
* **معرّف الحزمة (Package Name):** `com.smartreal.vpn`
* **المطور / الجهة المسؤولة (Developer / Data Controller):** Novyra
* **البريد الإلكتروني للتواصل وطلبات الخصوصية (Contact Email):** [apps.novyra@gmail.com](mailto:apps.novyra@gmail.com)
* **تاريخ السريان وآخر تحديث (Effective & Last Updated Date):** 1 نوفمبر 2026 (November 1, 2026)

---

## أولاً: النسخة العربية (Arabic Version)

### 1. مقدمة والتزام الشفافية
توضح سياسة الخصوصية هذه كيفية تعامل تطبيق **Smart Real VPN** (المشار إليه بـ «التطبيق»)، والمطور بواسطة **Novyra**، مع البيانات والأذونات عند استخدامك للتطبيق على أجهزة Android. صُمم التطبيق لتوفير اتصال شبكة افتراضية خاصة (VPN) مشفر عبر بروتوكول **OpenVPN** دون الحاجة إلى إنشاء حساب أو تسجيل دخول.

### 2. استخدام خدمة `VpnService` في نظام أندرويد
يستخدم التطبيق واجهة برمجة التطبيقات الرسمية `android.net.VpnService` في نظام أندرويد لإنشاء نفق شبكي مشفر (Encrypted Tunnel) على مستوى الجهاز أو للتطبيقات التي يحددها المستخدم، وذلك لحماية حركة مرور البيانات على الشبكات العامة وتوجيهها عبر خادم الـ VPN المختار.
* لا يقوم المطور (**Novyra**) بتشغيل خوادم مركزية لتخزين أو بيع أو مراقبة محتوى تصفحك أو سجل المواقع التي تزورها.

### 3. البيانات التي يعالجها التطبيق محليًا على جهازك
لا يطلب التطبيق منك تقديم أي بيانات شخصية (مثل الاسم أو رقم الهاتف أو البريد الإلكتروني) لتشغيله. يتم تخزين التفضيلات التالية **محليًا على جهازك فقط** (`SharedPreferences` وذاكرة التخزين الداخلية للتطبيق):
1. معرّف آخر خادم تم اختياره وقائمة الدول المفضلة.
2. إعدادات مزود DNS المختار (`Cloudflare` أو `AdGuard` أو `Quad9` أو `Google DNS`).
3. إعدادات تقسيم النفق (**Split Tunneling**): أسماء حزم التطبيقات (`Package Names`) التي تختار تمريرها عبر نفق الـ VPN.
4. نسخة مخبأة مؤقتًا (Cache) من قائمة الخوادم العامة لتسريع فتح التطبيق.
5. سجل تشخيص الجلسة الحالية (يُعرض لك داخل نافذة «تشخيص النفق» في الذاكرة المؤقتة أثناء الجلسة فقط ولا يُرسل إلى المطور).

### 4. البيانات التي تجمعها خدمات الطرف الثالث (Third-Party Services)
يعتمد التطبيق في عمله المجاني وتشغيل الخوادم على الخدمات الخارجية التالية، والتي قد تعالج بيانات تقنية وفق سياساتها الخاصة:

#### أ. إعلانات Google AdMob (`com.google.android.gms:play-services-ads`)
يستخدم التطبيق حزمة تطوير البرمجيات **Google Mobile Ads SDK (AdMob)** لعرض إعلانات البانر وإعلانات المكافأة (Rewarded Ads) لفتح خوادم VIP مجانًا. قد تقوم شركة Google تلقائيًا بجمع ومشاركة البيانات التالية لأغراض عرض الإعلانات والقياس ومنع الاحتيال:
* معرّف الإعلانات في أندرويد (**Advertising ID / AD_ID**).
* عنوان البروتوكول (**IP Address**) لتقدير الموقع الجغرافي التقريبي.
* معلومات الجهاز ونظام التشغيل وإصدار التطبيق.
* بيانات التفاعل مع الإعلانات وبيانات التشخيص والأداء.
* للاطلاع على سياسة خصوصية Google وكيفية معالجة البيانات: [https://policies.google.com/privacy](https://policies.google.com/privacy)

#### ب. دليل وخوادم شبكة VPN Gate العامة (`vpngate.net`)
يجلب التطبيق قائمة الخوادم العامة من مشروع **VPN Gate Academic Public VPN Relay** (التابع لجامعة تسوكوبا في اليابان عبر `https://www.vpngate.net/api/iphone/`).
* عند اتصالك بأحد خوادم VPN Gate العامة، تمر حركة مرور الشبكة عبر الخادم المضيف الذي يديره متطوعو شبكة VPN Gate.
* وفقًا لسياسة مشروع VPN Gate الرسمية لمكافحة إساءة الاستخدام والجرائم الإلكترونية، قد يحتفظ مشغلو خوادم VPN Gate بسجلات اتصال تقنية (Packet Headers / Connection Logs مثل طابع الوقت وعنوان IP المتصل) لمدة محدودة (عادةً أسبوعين `2 Weeks` كما يظهر في بيانات كل خادم).
* لا يملك المطور (**Novyra**) وصولًا إلى خوادم VPN Gate أو سجلات مشغليها.

#### ج. مزودو خدمة DNS الاختياريون
عند اختيارك لمزود DNS داخل إعدادات التطبيق، يتم توجيه استعلامات أسماء النطاقات (DNS Queries) عبر النفق إلى المزود الذي اخترته:
* **Cloudflare DNS:** `1.1.1.1` / `1.0.0.1`
* **AdGuard DNS:** `94.140.14.14` / `94.140.15.15`
* **Quad9 Security DNS:** `9.9.9.9` / `149.112.112.112`
* **Google Public DNS:** `8.8.8.8` / `8.8.4.4`

### 5. الأذونات الحساسة والغرض من استخدامها
يطلب التطبيق الأذونات التالية في ملف `AndroidManifest.xml` للأغراض الموضحة حصراً:
* **`android.net.VpnService` و `FOREGROUND_SERVICE` و `FOREGROUND_SERVICE_SPECIAL_USE`:** لإنشاء نفق OpenVPN المشفر وإبقاء الاتصال نشطًا في الخلفية أثناء استخدام تطبيقات أخرى.
* **`QUERY_ALL_PACKAGES`:** يُستخدم **محليًا فقط على جهازك** لقراءة قائمة التطبيقات المثبتة القابلة للتشغيل وعرضها لك داخل شاشة الإعدادات لتتمكن من اختيار التطبيقات المشمولة في ميزة **تقسيم النفق (Split Tunneling)**. لا يقوم التطبيق برفع أو مشاركة قائمة تطبيقاتك مع أي خادم خارجي.
* **`INTERNET` و `ACCESS_NETWORK_STATE` و `ACCESS_LOCAL_NETWORK`:** للاتصال بالإنترنت، جلب قائمة الخوادم، وقياس زمن الاستجابة الفعلي (`TCP Ping`).
* **`POST_NOTIFICATIONS`:** لإظهار إشعار حالة اتصال الـ VPN الدائم وأزرار التحكم السريع (إيقاف / إيقاف مؤقت / استئناف).
* **`RECEIVE_BOOT_COMPLETED`:** لإعادة تفعيل نفق الحماية عند إعادة تشغيل الجهاز إذا قام المستخدم بتفعيل ميزة Always-On VPN.
* **`READ_EXTERNAL_STORAGE`:** مضمّن لدعم استيراد ملفات تعريف OpenVPN المحلية على إصدارات أندرويد الأقدم.

### 6. الاحتفاظ بالبيانات وحذفها والتحكم بها
* **البيانات المحلية:** تبقى إعداداتك المحفوظة محليًا على جهازك فقط، ويمكنك حذفها بالكامل في أي وقت عبر التوجه إلى: **إعدادات أندرويد ← التطبيقات ← Smart Real VPN ← مكان التخزين ← مسح البيانات (Clear Data)** أو عبر إلغاء تثبيت التطبيق.
* **معرّف الإعلانات:** يمكنك إعادة تعيين معرّف الإعلانات أو إيقاف تخصيص الإعلانات من جهازك عبر: **إعدادات أندرويد ← Google ← الإعلانات (Ads)**.
* نظرًا لأن المطور (**Novyra**) لا يجمع أو يخزن حسابات مستخدمين أو بيانات شخصية على خوادم خاصة به، فلا توجد قاعدة بيانات خارجية لدى المطور تحتوي على بياناتك الشخصية.

### 7. خصوصية الأطفال
التطبيق عبارة عن أداة تقنية للشبكات والأمان، وهو غير موجه للأطفال دون سن 13 عامًا (أو السن القانوني المعمول به في بلد الإقامة)، ولا نجمع عن قصد أي بيانات شخصية من الأطفال.

### 8. النقل الدولي للبيانات وحقوق المستخدمين (GDPR / KVKK)
بحكم طبيعة خدمات الـ VPN، عند اختيارك الاتصال بخادم في دولة أخرى، يتم توجيه حركة بياناتك عبر تلك الدولة. للمستخدمين في المنطقة الاقتصادية الأوروبية (GDPR) أو تركيا (KVKK) أو المناطق ذات القوانين المماثلة الحق في التحكم في أذونات الجهاز وإعدادات الإعلانات والتواصل معنا لأي استفسار يتعلق بالخصوصية.

### 9. التعديلات على سياسة الخصوصية والتواصل معنا
قد نقوم بتحديث سياسة الخصوصية هذه عند إضافة ميزات جديدة أو تحديث خدمات الطرف الثالث، وسيتم نشر النسخة المحدثة على هذه الصفحة مع تحديث تاريخ السريان أعلاه.
لأي استفسارات أو طلبات متعلقة بالخصوصية، يرجى التواصل مع **Novyra** عبر البريد الإلكتروني:
📧 **[apps.novyra@gmail.com](mailto:apps.novyra@gmail.com)**

---

## ثانياً: النسخة الإنجليزية (English Version)

### 1. Introduction
This Privacy Policy explains how **Smart Real VPN** (`com.smartreal.vpn`), developed and published by **Novyra** ("we", "us", or "our"), handles information and Android permissions. Smart Real VPN provides an encrypted **OpenVPN** tunnel without requiring user registration or login.

### 2. Android `VpnService` Disclosure
Smart Real VPN relies on Android's official `android.net.VpnService` API as its core functionality to establish an encrypted device-level network tunnel between your device and the VPN server you select.
* **Novyra** does not operate proprietary logging servers to monitor, store, or sell your browsing history or traffic payload.

### 3. Data Stored Locally on Your Device
You do not need to create an account or submit personal details to use Smart Real VPN. The following preferences are stored **exclusively on your device** (`SharedPreferences` and local app cache):
1. Selected server ID and favorite country codes.
2. Selected DNS mode (`Cloudflare`, `AdGuard`, `Quad9`, or `Google DNS`).
3. **Split Tunneling** package selection (stored locally to configure the VPN interface).
4. Compressed local cache of the public server directory (`vpn_gate_servers_v2.cache`).
5. Ephemeral in-memory OpenVPN handshake logs displayed only in the in-app Diagnostics view during your active session.

### 4. Third-Party Services & External Data Processing

#### A. Google AdMob (`com.google.android.gms:play-services-ads`)
The app integrates the **Google Mobile Ads SDK (AdMob)** to display banner ads and optional rewarded ads (used to unlock high-speed VIP server selections). Google Mobile Ads SDK may automatically collect and process:
* Android **Advertising ID (`AD_ID`)** and device identifiers.
* IP address (used for coarse location estimation and fraud prevention).
* Device model, OS version, and app interaction/diagnostic telemetry.
* For details on how Google processes data, please see [Google's Privacy & Terms](https://policies.google.com/privacy).

#### B. VPN Gate Public Relay Directory (`vpngate.net`)
The app fetches public OpenVPN server configurations from the **VPN Gate Academic Public VPN Relay Project** (`https://www.vpngate.net/api/iphone/`), operated by the University of Tsukuba, Japan.
* When you connect to a VPN Gate volunteer server, your encrypted tunnel terminates at that operator's server.
* Under the VPN Gate project's anti-abuse policy, individual VPN Gate server operators may retain connection metadata logs (such as connection timestamps and IP addresses, typically for up to `2 Weeks` as indicated per server) to prevent network abuse. **Novyra** does not control third-party volunteer nodes or have access to their logs.

#### C. Optional DNS Resolvers
Depending on your selection in Settings, DNS queries inside the tunnel are routed to one of the following public resolvers:
* **Cloudflare DNS** (`1.1.1.1` / `1.0.0.1`)
* **AdGuard DNS** (`94.140.14.14` / `94.140.15.15`)
* **Quad9 Security DNS** (`9.9.9.9` / `149.112.112.112`)
* **Google Public DNS** (`8.8.8.8` / `8.8.4.4`)

### 5. Permissions Used by the App
* **`android.net.VpnService`, `FOREGROUND_SERVICE`, `FOREGROUND_SERVICE_SPECIAL_USE` (`vpn`):** Required to establish and maintain the OpenVPN tunnel in the background.
* **`QUERY_ALL_PACKAGES`:** Used **strictly on-device** to list launchable installed apps in the **Split Tunneling** settings screen so you can choose which apps use the VPN tunnel. Your installed app list is never uploaded or transmitted externally.
* **`INTERNET`, `ACCESS_NETWORK_STATE`, `ACCESS_LOCAL_NETWORK`:** Used to fetch server lists, perform live TCP latency checks (`Ping`), and establish VPN connections.
* **`POST_NOTIFICATIONS`:** Used to display the persistent VPN connection notification with quick Disconnect / Pause / Resume actions.
* **`RECEIVE_BOOT_COMPLETED`:** Used to support system Always-On VPN reconnection after device reboot.
* **`READ_EXTERNAL_STORAGE`:** Included by the underlying OpenVPN engine for legacy profile compatibility.

### 6. Data Retention, Deletion & User Controls
* **Local Data Deletion:** You can erase all locally stored preferences and cached server lists at any time via **Android Settings → Apps → Smart Real VPN → Storage → Clear Data**, or by uninstalling the app.
* **Advertising ID Control:** You can reset or delete your Android Advertising ID via **Android Settings → Google → Ads**.

### 7. Children's Privacy
Smart Real VPN is a general-audience network utility and is not directed at children under the age of 13. We do not knowingly collect personal data from children.

### 8. Contact Us
If you have any questions or privacy requests regarding **Smart Real VPN**, please contact **Novyra** at:
📧 **[apps.novyra@gmail.com](mailto:apps.novyra@gmail.com)**
