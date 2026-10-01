# 👋 Merhaba, Ben Alphan Kılıçaslan

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&pause=1000&color=61AFEF&center=true&vCenter=true&width=620&lines=Bilgisayar+Programc%C4%B1s%C4%B1+%26+Yaz%C4%B1l%C4%B1m+Geli%C5%9Ftirici;Masa%C3%BCst%C3%BC%2C+Sistem+Programlama+%26+Yapay+Zeka;A%C4%9F+T%C3%BCnelleme%2C+Ses+%C4%B0%C5%9Fleme+%26+Telemetri;Finansal+Sim%C3%BClasyon+%26+Vergi+Algoritmalar%C4%B1" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://linkedin.com/in/alphankilicaslan"><img src="https://img.shields.io/badge/LinkedIn-Alphan%20K%C4%B1l%C4%B1%C3%A7aslan-0A66C2?style=for-the-badge&logo=linkedin" alt="LinkedIn" /></a>
  <a href="mailto:alphankilicaslan@gmail.com"><img src="https://img.shields.io/badge/Email-alphankilicaslan%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" /></a>
  <img src="https://img.shields.io/badge/Unvan-Bilgisayar%20Programc%C4%B1s%C4%B1-2ea44f?style=for-the-badge" alt="Unvan" />
</p>

---

## 👨‍💻 Programcılık Vizyonum & Yaklaşımım

Ben pratik, sahada çalışan, donanımın ve işletim sisteminin dilinden anlayan bir **Bilgisayar Programcısıyım**.

Geliştirdiğim projelerde teorik yaklaşımlardan ziyade; **doğrudan performansa odaklanan, düşük seviyeli API'leri (Win32, ASIO, WMI, Donanım sürücüleri) kullanan, otonom yapay zeka aracı modelleri geliştiren ve gerçek hayat problemlerine çözüm üreten** yazılımlar inşa ediyorum.

Projelerimin büyük çoğunluğu tescilli yazılımlar ve fikri mülkiyet (IP) korumalı masaüstü sistemleri olduğu için kaynak kodları kapalı tutulmaktadır. Aşağıda bu sistemlerin **derinlemesine çalışma mantığı, özellikleri ve mimari yapıları** yer almaktadır.

---

## 🛠️ Yetkinlikler & Teknoloji Yığını

<p align="center">
  <img src="https://skillicons.dev/icons?i=cs,dotnet,python,cpp,ts,js,react,html,css,postgres,redis,sqlite,docker,git,github,windows" />
</p>

* **Diller & Ortamlar:** C# (.NET Core / WPF), Python, C/C++, TypeScript, JavaScript, Lua.
* **Masaüstü & Sistem Programlama:** Windows Presentation Foundation (WPF), Win32 API, WebView2 (Modern Web Entegrasyonu), FFmpeg Interop, NAudio / ASIO.
* **Ağ & Donanım Entegrasyonu:** Cloudflare WARP & WireGuard Tünelleme, Native Wi-Fi API, Donanım Telemetrisi (RAM SPD, WMI, Sürücü Analizi), Sanal Ses Kabloları (VBCable).
* **Yapay Zeka & Agentic Sistemler:** Yerel Model Çalıştırma (Quantized / Local LLM), Çoklu Model Orkestrasyonu, Vektör RAG Bilgi Bankası, Gerçek Zamanlı Ses Köprüsü (VoiceBridge), 3D Semantik Çizge Görselleştirme.
* **Finansal Modelleme:** GVK 103 Vergi Matrah Simülasyonu, KDV Mahsuplaşma Algoritmaları, Dinamik Nakit Akış Tahmini.

---

## 🌟 Öne Çıkan Projeler & Kapsamlı Sistem İncelemeleri

---

### 🌐 1. AlpNet & AlpNet Pulse — Gelişmiş Ağ Tünelleme, Gerçek Zamanlı Ses Çevirisi & Donanım Telemetrisi

<p align="center">
  <img src="https://img.shields.io/badge/Proje-AlpNet%20Pulse-0078D7?style=flat-square&logo=windows" />
  <img src="https://img.shields.io/badge/Altyap%C4%B1-C%23%20WPF%20%2B%20Python%20%2B%20FFmpeg-512BD4?style=flat-square" />
  <img src="https://img.shields.io/badge/A%C4%9F-Cloudflare%20WARP%20%2F%20WireGuard-FF6600?style=flat-square" />
  <img src="https://img.shields.io/badge/Ses-ASIO%20%2F%20Surround%20Stereo%20Engine-brightgreen?style=flat-square" />
</p>

**AlpNet Pulse**, oyuncular, canlı yayıncılar ve ileri düzey bilgisayar kullanıcıları için geliştirilmiş çok fonksiyonlu bir sistem merkezidir. Yalnızca standart bir teleometri aracı değil; ağ tünelleme, anlık sesli çeviri, anlık oyun klibi yakalama ve donanım kontrolünü tek çatı altında birleştiren entegre bir masaüstü yazılımıdır.

```mermaid
flowchart TD
    subgraph AlpNet_Core["AlpNet Pulse Çekirdeği (C# WPF & Sistem Katmanı)"]
        UI[WPF Modern Arayüz & Bildirim Alanı]
        Hotkeys[Global Kısayol Tuş Dinleyicisi]
        Settings[PulseAppSettings & Replay Yapılandırması]
    end

    subgraph Network_Engine["Ağ & Tünelleme Katmanı"]
        Warp[WarpManager - Cloudflare WARP & WireGuard]
        WiFi[NativeWifi - Wi-Fi Sinyal & Ağ Analitiği]
        Split[SplitWire - Uygulama Bazlı Trafik Yönlendirme]
    end

    subgraph Audio_Translation["Ses & Anlık Çeviri Hattı"]
        AudioIn[Mikrofon & Sistem Sesi Girişi]
        Surround[SurroundToStereo Dönüştürücü]
        VoiceTrans[Canlı Sesli Çeviri Modülü - Python STT/TTS]
        AudioOut[VBCable / Kulaklık Çıkışı]
        AudioIn --> Surround --> VoiceTrans --> AudioOut
    end

    subgraph Hardware_Media["Donanım Telemetrisi & Medya"]
        Hardware[RAM SPD & Disk Bilgi Teşhis Kütüphanesi]
        FFmpeg[FFmpegManager - Düşük Gecikmeli Replay / Klip Kaydı]
        Player[Entegre Video Oynatıcı Penceresi]
        Discord[Discord Rich Presence Entegrasyonu]
    end

    UI --> Network_Engine
    UI --> Audio_Translation
    UI --> Hardware_Media
    Hotkeys --> FFmpeg
    FFmpeg --> Player
```

#### 🔍 AlpNet Pulse'ın Çözdüğü Problemler ve Özellikleri:
1. **Akıllı Ağ Yönlendirme & WARP Tünelleme (WarpManager & SplitWire):**
   * İnternet trafiğini optimize eden, sansür ve rota gecikmelerini aşmak için Cloudflare WARP ve WireGuard tünellerini masaüstünden tek tıkla başlatan ve yöneten tünelleme entegrasyonu.
   * `NativeWifi` modülüyle çevre Wi-Fi ağlarını donanım seviyesinde tarama ve sinyal kalitesini haritalandırma.
2. **Canlı İki Yönlü Ses İşleme & Anlık Çeviri (VoiceTranslation Pipeline):**
   * Oyun veya görüşmeler sırasında gelen yabancı sesleri mikrofon/kulaklık düzeyinde yakalayan, düşük gecikmeli Python çeviri motoruna ileten ve çeviriyi kullanıcıya doğrudan nöral sesle dinleten tam entegre ses köprüsü.
   * Çok kanallı surround sesleri bozulma olmadan stereo kulaklıklara indirgeyen `SurroundToStereoProvider` ses matrisi.
3. **Sistem Kaynaklarını Yormayan Arka Plan Replay / Klip Motoru (FFmpegManager):**
   * GPU hızlandırmalı FFmpeg motoru sayesinde oyunda veya ekranda yaşanan son saniyeleri (Instant Replay) sistem performansını düşürmeden RAM/Disk tamponunda tutma ve global kısayol tuşuyla anında klip olarak kaydetme.
   * Kaydedilen klipleri doğrudan uygulama içindeki özel video oynatıcıda (`VideoPlayerWindow`) inceleme imkanı.
4. **Düşük Seviyeli Donanım Teşhis Kütüphanesi:**
   * WMI, RAM SPD (Timing & Bellek çipi üretici bilgileri) ve Disk denetleyicisi seviyesinde donanım okuma.
5. **Güvenlik, Lisanslama & Obfuscation:**
   * Donanım parmak izine (HWID) kilitli lisans doğrulama sistemi (`AlpNet.Keygen`), MSI yükleyicisi ve `Obfuscar` ile tersine mühendisliğe karşı korunan binary mimarisi.

---

### 💰 2. AlpFinans — Gelir/Gider Analitiği, GVK 103 Vergi Simülatörü & Net Kâr Hesaplayıcı

<p align="center">
  <img src="https://img.shields.io/badge/Proje-AlpFinans-2ea44f?style=flat-square&logo=cashapp" />
  <img src="https://img.shields.io/badge/Altyap%C4%B1-C%23%20WPF%20%2B%20Python%20Backend-0078D7?style=flat-square" />
  <img src="https://img.shields.io/badge/Mevzuat-GVK%20103%20%2B%20Gen%C3%A7%20Giri%C5%9Fimci%20%C4%B0stisnas%C4%B1-gold?style=flat-square" />
  <img src="https://img.shields.io/badge/G%C3%BCvenlik-100%25%20Yerel%20Veri%20Gizlili%C4%9Fi-critical?style=flat-square" />
</p>

**AlpFinans**, şahıs şirketleri, serbest çalışan programcılar ve KOBİ'ler için geliştirilmiş; yalnızca geçmiş harcamaları tutmakla kalmayıp Türkiye Vergi Mevzuatına göre **gelecekteki vergi yükünü ve gerçek net kârı kuruşu kuruşuna hesaplayan** gelişmiş bir finansal karar destek sistemidir.

```mermaid
flowchart LR
    subgraph Girdiler["Kullanıcı Girdileri"]
        Brut[Brüt Gelir Faturaları]
        Gider[Şirket Giderleri & Harcamalar]
        Genc[Genç Girişimci Muafiyeti Durumu]
    end

    subgraph Hesaplama["AlpFinans Simülasyon Motoru"]
        KDV[KDV Dengesi: Gelir KDV - Gider KDV]
        Matrah[Vergi Matrahı Hesabı]
        GVK[GVK 103 Dilimleri: %15, %20, %27, %35, %40]
        Kalkan[Vergi Kalkanı Avantaj Analizi]
        NetHesap[Cebe Kalan Net Nakit Formülü]

        Brut & Gider --> KDV
        Brut & Gider & Genc --> Matrah
        Matrah --> GVK
        Gider --> Kalkan
        GVK & KDV & Brut --> NetHesap
    end

    subgraph Ciktilar["Stratejik Karar Çıktıları"]
        R1[Ödenecek Net KDV]
        R2[Dönem Gelir Vergisi Yükü]
        R3[Giderin Sağladığı Vergi Avantajı]
        R4[Cebe Kalan Net Harcanabilir Nakit]
    end

    KDV --> R1
    GVK --> R2
    Kalkan --> R3
    NetHesap --> R4
```

#### 🔍 AlpFinans'ın Çözdüğü Problemler ve Özellikleri:
1. **"Ay Sonunda Cebime Ne Kalacak?" Sorusuna Kesin Yanıt:**
   * Birçok yazılımcı ve işletme brüt ciro ile eline geçen parayı karıştırır. AlpFinans; KDV'yi, gelir vergisi dilimlerini ve işletme giderlerini birbirinden ayrıştırarak kullanıcının şahsi cebine kalan net harcanabilir tutarı net olarak raporlar.
2. **Gerçek Zamanlı GVK 103 Gelir Vergisi Dilim Simülatörü:**
   * Kazanç arttıkça %15'ten başlayıp %20, %27, %35 ve %40 dilimlerine geçen kademeli gelir vergisi baremlerini anlık simüle eder. Fatura kesilmeden önce vergi dilimi atlamasının maliyetini gösterir.
3. **Genç Girişimci İstisnası Desteği:**
   * Mevzuatta yer alan genç girişimci matrah muafiyetini (230.000 TL) tek tıkla hesaba katarak yeni girişimcilerin gerçek nakit akışını planlamasını sağlar.
4. **Vergi Kalkanı (Tax Shield) Analitiği:**
   * Yapılan bir giderin (örneğin donanım, ofis ya da yazılım aboneliği) şirkete sağladığı KDV mahsubu ve gelir vergisi indirim avantajını hesaplayarak harcamanın gerçek maliyetini ortaya koyar.
5. **Sıfır Bulut Bağımlılığı & %100 Finansal Gizlilik:**
   * Şirketin ve geliştiricinin hassas finansal tabloları kesinlikle üçüncü taraf bulut veritabanlarına gönderilmez; tamamen yerel cihazda şifreli veri tabanında tutulur.

---

### 🧠 3. AlphaGravity — Otonom Kurumsal Yapay Zeka & 3D Bilgi Zekası Platformu

<p align="center">
  <img src="https://img.shields.io/badge/Proje-AlphaGravity-critical?style=flat-square&logo=openai" />
  <img src="https://img.shields.io/badge/Aray%C3%BCz-Modern%20Dark%20WPF%20%2B%20WebView2-blue?style=flat-square" />
  <img src="https://img.shields.io/badge/G%C3%B6rselle%C5%9Ftirme-3D%20Three.js%20%2F%20WebGL%20Grafi%C4%9Fi-green?style=flat-square" />
  <img src="https://img.shields.io/badge/Ses-VoiceBridge%20Real--Time%20Loop-orange?style=flat-square" />
</p>

**AlphaGravity**, işletmelerin ve bağımsız araştırmacıların hassas verilerini dış dünyadan tamamen izole ederek işleyen, yerel LLM inference motorunu, iki yönlü sesli asistanı ve 3 boyutlu interaktif bilgi haritasını bir araya getiren amiral gemisi masaüstü yapay zeka istasyonudur.

```mermaid
flowchart TB
    subgraph Presentation["Modern Masaüstü Sunum Katmanı"]
        WPF_App[C# WPF Native Uygulama Kabuğu]
        WebView[WebView2 Donanım Hızlandırmalı Render Motoru]
        ThreeJS["3 Boyutlu Dinamik Semantik Çizge (Three.js / WebGL)"]
        WPF_App --> WebView --> ThreeJS
    end

    subgraph Audio_Pipeline["VoiceBridge Çift Yönlü Ses Katmanı"]
        Mic[Mikrofon Girişi & VAD Filtresi]
        SpeechRec[Gerçek Zamanlı Konuşma Algılama]
        NeuralTTS[Düşük Gecikmeli Nöral Ses Sentezi]
        Mic --> SpeechRec
    end

    subgraph Intelligent_Core["AlphaGravity Orkestrasyon Çekirdeği"]
        ModelRouter{Akıllı Model Yönlendirici}
        Local_Inference["Yerel Model Motoru (Scratch / Quantized Engine - Tamamen Çevrimdışı)"]
        Cloud_Gateway["Şifreli API Kasası (Vault Korumalı Dış Modeller)"]
        ModelRouter -->|Hassas & Gizli Veri| Local_Inference
        ModelRouter -->|Geniş Kapsamlı Araştırma| Cloud_Gateway
    end

    subgraph Knowledge_Base["Kurumsal Bilgi Bankası & Vektör RAG"]
        FileIngest[Doküman Yükleyici .MD, .TXT, .PDF]
        VectorEngine[Anlamsal Parçalama & Bellek-İçi Vektör İndeksi]
        FileIngest --> VectorEngine
    end

    subgraph Reliability["Güvenilirlik & Analitik"]
        Checkpoints[Tek Tıkla Deterministik Geri Yükleme & Snapshot]
        Reports[Öğrenme ve Çıkarım Doğruluk Raporları]
    end

    Presentation <--> Intelligent_Core
    SpeechRec --> Intelligent_Core
    Intelligent_Core --> NeuralTTS
    Intelligent_Core <--> Knowledge_Base
    Intelligent_Core --> Reliability
    Knowledge_Base -.->|Anlamsal Düğüm İlişkileri| ThreeJS
```

#### 🔬 AlphaGravity'nin Öne Çıkan Mimari Yetenekleri:
1. **Dinamik 3D Semantik Bilgi Çizgesi (3D Neural Topology):**
   * Yapay zekanın öğrendiği kavramlar ve dökümanlar arasındaki anlamsal ilişkiler, WebGL ve Three.js tabanlı canlı bir 3 boyutlu grafikte fizik motoruyla canlandırılır. Kullanıcı düğümler arasında gezinebilir, kavram kümelerini görsel olarak keşfedebilir.
2. **VoiceBridge — Gerçek Zamanlı Ses Köprüsü:**
   * Tuşlara basmadan, konuşma bittiği anı algılayan VAD (Voice Activity Detection) algoritmalarıyla yapay zekaya sesli girdi sağlayan ve yanıtı anlık nöral ses senteziyle geri seslendiren düşük gecikmeli döngü.
3. **İzole / Çevrimdışı Çalışma (Air-Gapped Modu):**
   * Gizli şirket verilerinin internete sızmasını engellemek amacıyla tamamen yerel donanımda çalışan modeller ile sıfır veri sızıntısı garantisi.
4. **Kriptografik Güvenlik Kasası (Local Secret Vault):**
   * Harici servis anahtarları işletim sisteminin kriptografik API'leri kullanılarak şifrelenir; telemetri veya log kaydı dışarı aktarılmaz.
5. **Kararlı Kontrol Noktaları (Checkpoint & Rollback Mimarisi):**
   * Bilgi tabanı üzerinde yapılan tüm güncellemeler ve model hafızası anlık olarak snapshot'lanabilir; tek tıkla eski kararlı duruma (`GERI_YUKLE_CHECKPOINT`) dönülebilir.

---

## 📊 GitHub İstatistikleri & Süreklilik

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=alphankilicaslan&show_icons=true&theme=tokyonight&count_private=true&hide_border=true" alt="Alphan Kılıçaslan GitHub Stats" />
  <br/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=alphankilicaslan&theme=tokyonight&hide_border=true" alt="Alphan Kılıçaslan GitHub Streak" />
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=alphankilicaslan&layout=compact&theme=tokyonight&count_private=true&hide_border=true" alt="En Çok Kullanılan Diller" />
</p>

---

<p align="center">
  <i>"Bir bilgisayar programcısının asıl gücü; teoride kalmayıp çalışan, hızlı ve gerçek problemleri çözen sistemler inşa edebilmesidir."</i>
</p>
