# Yapay Zeka & Makine Öğrenimi 🤖

## Başlangıç:
Çoğu insan yapay zeka ile makine öğreniminin aynı şey olduğunu sanır lakin aslında bunlar birer iç içe geçmiş kavramlardır. Yapay zeka ise bunların bütünüdür.

Öncelikle Yapay Zeka(Artiffical intelligence)'nın ne olduğuna bir bakalım

- **Yapay Zeka:** İnsan zekasını, karar verme mekanizmalarını ve öğrenme yeteneğini bilgisayar ortamında taklit eden tüm sistemlerin genel adıdır.(Şemsiye kavram)


- **Makine Öğrenimi (Machine Learning ML):** Yapay zekanın alt dalıdır. Kabaca **programlanmadan, veriden öğrenerek tahminler yapan veya kararlar alan algoritmalar bütünüdür.** 

Peki.. ne demek **programlanmadan ?** Kabaca şöyle anlatabilirim..

## ⚡ Geleneksel Programlama vs. Makine Öğrenimi
Eğer bilgisayara tam anlamıyla her şeyi programlayacak olsanız (ki bunu yapmanız mümkün olmaz) milyarlarca olasığı hesap etmeniz gerekirdi. Örneğin diyelim ki bir spam e-posta aracınız olsun. İşte size basit bir spam e-posta örneği:
```
Konu: Bedava hediye kazandınız!

Tebrikler! Bedava iPhone kazandınız. Hemen tıkla ve bilgilerini gir: sahte-link.com

Bu fırsat kaçmaz, tıkla kazan!

Saygılar,
Ödül Ekibi
```

Bu maili "spam" olarak işaretlemek isteseydiniz maildeki genel bağlama bakmanız gerekirdi. Burada biz "bedava" kelimesini hedef alalım. Diyelim ki "bedava" kelimesi bir mailde geçiyorsa o mail spamdir. Bunu yapmak için geleneksel yazılımda şu algoritmayı uygulamanız gerekirdi:

```
Eğer => Mailde varsa => "Bedava":
    işaretle => spam
değilse:
    işaretle => güvenli
```

Artık bir maili spam olarak işaretleyebiliyor olursunuz. Ama bu mekanizmayı atlatmak çok kolay olurdu! Eğer maili size b.e.d.a.v.a şeklinde gönderirsem mekanizmanızı çok rahat atlatmış olacağım. Siz kodunuzu buna göre güncelleyeceksiniz, bu sefer ben b-e-d-a-v-a yazıp yine mekanizmanızı atlatacağım. Özetle bunun bir sonu yok! Her olasılığı tek tek koda dökmeniz imkansızdır.

İşte Makine Öğrenimi (ML) tam burada devreye girer. Biz kuralları elle teker teker yazmak yerine, sisteme binlerce e-posta veririz. Algoritma e-postaların içindeki kalıpları (bunlara ileride **"desenler / patterns"** diyeceğiz) kendisi inceleyerek spam olma kurallarını kendisi keşfeder.

Makinenin veriler ve algoritmalar vasıtasıyla kendi kendine öğrenme sürecine **Machine Learning (ML)**, bu öğrenme sonucunda ortaya çıkan kurallar bütününe ise **Model** adını veriyoruz.

```mermaid
flowchart LR
    subgraph Traditional["Geleneksel Programlama"]
        direction LR
        D1[Veri] --> R1[Kurallar] --> C1[Bilgisayar] --> O1[Sonuç]
    end

    subgraph ML["Makine Öğrenimi"]
        direction LR
        D2[Veri] --> R2[Sonuçlar] --> C2[Bilgisayar] --> M2[MODEL]
    end
```

## 📐 Kavram Hiyerarşisi
```mermaid
flowchart TB
    %% Kutu stillerini (renkler, kenarlıklar, yazı tipleri) tanımlıyoruz
    classDef aiStyle fill:#3b5998,stroke:#1d2c4d,stroke-width:3px,color:#ffffff,font-weight:bold,font-size:16px;
    classDef mlStyle fill:#f37021,stroke:#a34814,stroke-width:3px,color:#ffffff,font-weight:bold,font-size:16px;
    classDef dlStyle fill:#ea1c4e,stroke:#9e1334,stroke-width:3px,color:#ffffff,font-weight:bold,font-size:16px;
    classDef nnStyle fill:#00b4b4,stroke:#006666,stroke-width:3px,color:#ffffff,font-weight:bold,font-size:16px;
    
    %% Bağlantı çizgilerini ve genel arka planı belirginleştiriyoruz
    %% linkStyle 0,1,2,3 diyerek okların rengini koyu gri yapıyoruz
    
    subgraph AI["AI - Artificial Intelligence"]
        direction TB
        subgraph ML["ML - Machine Learning"]
            direction TB
            subgraph DL["DL - Deep Learning"]
                direction TB
                NN["NN - Neural Networks"]
            end
        end
    end

    %% Tanımladığımız stilleri kutulara uyguluyoruz
    class AI aiStyle;
    class ML mlStyle;
    class DL dlStyle;
    class NN nnStyle;
    
    %% Arka planı ve çizgileri netleştirmek için stil atamaları
    style AI fill:#3b5998,stroke:#2c4373,stroke-width:4px,color:#fff
    style ML fill:#f37021,stroke:#c25715,stroke-width:4px,color:#fff
    style DL fill:#ea1c4e,stroke:#b8143b,stroke-width:4px,color:#fff
    style NN fill:#00b4b4,stroke:#008080,stroke-width:4px,color:#fff
```
## 🔄 Makine Öğrenimi Öğrenme Yöntemleri
Makine öğrenimi algoritmaları veriyi işleme ve öğrenme biçimlerine göre 4 temel kategoriye ayrılır:
```mermaid
flowchart TD
    %% Ana başlık kutusunun stili
    Root["MAKİNE ÖĞRENİMİ YÖNTEMLERİ"]
    classDef rootStyle fill:#2C3E50,stroke:#1A252F,stroke-width:3px,color:#FFFFFF,font-weight:bold,font-size:16px;
    class Root rootStyle;

    %% Alt dalların (Yöntemlerin) stilleri
    classDef methodStyle fill:#3498DB,stroke:#21618C,stroke-width:2px,color:#FFFFFF;
    
    %% Düğümleri (Kutuları) oluşturuyoruz (Alt satıra geçmek için <br/> kullanıyoruz)
    Supervised["Denetimli<br/>(Supervised Learning)"]
    Unsupervised["Denetimsiz<br/>(Unsupervised Learning)"]
    SemiSupervised["Yarı-Denetimli<br/>(Semi-Supervised Learning)"]
    Reinforcement["Pekiştirmeli<br/>(Reinforcement Learning)"]

    %% Ağaç hiyerarşisini (Bağlantıları) kuruyoruz
    Root --> Supervised
    Root --> Unsupervised
    Root --> SemiSupervised
    Root --> Reinforcement

    %% Stilleri alt dallara uyguluyoruz
    class Supervised,Unsupervised,SemiSupervised,Reinforcement methodStyle;
    
    %% Bağlantı çizgilerini (Okları) belirgin ve koyu renk yapıyoruz
    linkStyle default stroke:#7F8C8D,stroke-width:2px;
```

## 🟢 1. Denetimli Öğrenme (Supervised Learning)

Sisteme **hem girdiler (X) hem de doğru yanıtlar/etiketler (Y)** verilir. Model, girdiden doğru yanıtı bulmayı öğrenir.

- **Öğretmen Mantığı:** Bir öğrenciye **çözümlü soru bankası verip arkasındaki cevap anahtarıyla birlikte çalıştırmak** gibidir.

**Temel Alt Alanlar:**

* **Sınıflandırma (Classification):** Veriyi kategorilere ayırır (E-posta Spam mi Değil mi?, Kedi mi Köpek mi?).

* **Regresyon (Regression):** Sürekli sayısal bir değer tahmin eder (Ev fiyatı tahmini, Hava sıcaklığı tahmini).
```mermaid
flowchart LR
    %% Girdi Kutularını Tanımlıyoruz
    Text["📄 E-posta Metni"]
    Label["🏷️ Etiket: Spam"]

    %% Model ve Çıktı Kutuları
    Model["⚙️ Model Eğitimi"]
    Output["🎯 Tahmin: Spam (%98)"]

    %% Stil Tanımlamaları (Renkler ve Belirgin Kenarlıklar)
    classDef inputStyle fill:#E8F8F5,stroke:#1ABC9C,stroke-width:2px,color:#0E6251,font-weight:bold;
    classDef modelStyle fill:#FEF9E7,stroke:#F1C40F,stroke-width:3px,color:#7D6608,font-weight:bold;
    classDef outputStyle fill:#FDEDEC,stroke:#E74C3C,stroke-width:3px,color:#78281F,font-weight:bold;

    %% Stilleri Uyguluyoruz
    class Text,Label inputStyle;
    class Model modelStyle;
    class Output outputStyle;

    %% Akış Bağlantıları
    Text --> Model
    Label --> Model
    Model ===> Output

    %% Bağlantı Çizgilerinin Rengi ve Kalınlığı
    linkStyle 0,1 stroke:#7F8C8D,stroke-width:2px;
    %% Modelden Çıktıya giden ok daha kalın (===>) ve vurgulu
    linkStyle 2 stroke:#E74C3C,stroke-width:3px;
```

## 🔵 2. Denetimsiz Öğrenme (Unsupervised Learning)
Veri setinde **hiçbir etiket veya yanıt yoktur.** Algoritma, **verinin** içindeki gizli **desenleri, benzerlikleri ve grupları kendisi keşfeder**.

- **Kaşif Mantığı:** Bilmediğiniz bir gezegendeki taşları renklerine ve boyutlarına göre kendi kafanızda gruplamak gibidir.

**Temel Alt Alanlar:**
* Kümeleme (Clustering): Benzer verileri gruplar (Müşteri segmentasyonu, haberleri konularına göre ayırma).

* Boyut İndirgeme (Dimensionality Reduction): Karmaşık verileri basitleştirir (Görsel sıkıştırma).
```mermaid
flowchart LR
    %% Kutuları Tanımlıyoruz
    Input["📥 Karışık E-postalar<br/>(Etiketsiz)"]
    Model["⚙️ Model"]
    Group1["📢 Grup 1: Reklamlar"]
    Group2["💼 Grup 2: İş Mailleri"]

    %% Akış Bağlantıları (Modelden iki farklı gruba ayrım)
    Input ==> Model
    Model ==> Group1
    Model ==> Group2

    %% Renk ve Stil Tanımlamaları (classDef)
    classDef inputStyle fill:#E8F8F5,stroke:#1ABC9C,stroke-width:2px,color:#0E6251,font-weight:bold;
    classDef modelStyle fill:#FEF9E7,stroke:#F1C40F,stroke-width:3px,color:#7D6608,font-weight:bold;
    classDef group1Style fill:#FDEDEC,stroke:#E74C3C,stroke-width:2px,color:#78281F,font-weight:bold;
    classDef group2Style fill:#EBF5FB,stroke:#2980B9,stroke-width:2px,color:#154360,font-weight:bold;

    %% Stilleri kutulara uyguluyoruz
    class Input inputStyle;
    class Model modelStyle;
    class Group1 group1Style;
    class Group2 group2Style;

    %% Bağlantı çizgilerini (Okları) belirgin yapıyoruz
    linkStyle default stroke:#7F8C8D,stroke-width:2.5px;
```
## 🟡 3. Yarı-Denetimli Öğrenme (Semi-Supervised Learning)
Elimizde çok az miktarda etiketli veri ve devasa miktarda etiketsiz veri olduğunda kullanılır.

- **Örnek:** Fotoğraf arşivinizdeki 10.000 fotoğraftan sadece 50 tanesine kimin olduğunu yazarsınız, model kalan 9.950 fotoğrafı bu 50 fotoğraftan yola çıkarak kendisi eşleştirir.
## 🔴 4. Pekiştirmeli Öğrenme (Reinforcement Learning)
**Model (Ajan / Agent)**, bir çevre içinde **deneme-yanılma** yoluyla öğrenir. Doğru hamle yaptığında **Ödül (Reward)**, yanlış yaptığında **Ceza (Penalty)** alır. Amacı **toplam ödülü en yüksek düzeye çıkarmak**tır.

- **Oyun Mantığı:** Bir oyunda yüksek skor yapmayı deneme-yanılma ile öğrenen yapay zeka.

- **Kullanım Alanları:** Otonom araçlar (Tesla), Satranç/Go oynayan yapay zekalar (AlphaGo), Robotik kol hareketleri.
```mermaid
flowchart TD
    %% Düğümleri (Kutuları) Tanımlıyoruz
    Ajan1["🤖 Ajan (AI)"]
    Cevre["🌍 Çevre<br/><i>(Örn: Oyun Alanı / Yol)</i>"]
    Ajan2["🤖 Ajan (AI)"]

    %% Akış Bağlantıları ve Etiketler
    Ajan1 -->|"Eylem (Action)"| Cevre
    Cevre -->|"Ödül / Durum Bilgisi"| Ajan2

    %% Renk ve Stil Tanımlamaları
    classDef ajanStyle fill:#EBF5FB,stroke:#2980B9,stroke-width:3px,color:#154360,font-weight:bold,font-size:16px;
    classDef cevreStyle fill:#F4F6F7,stroke:#7F8C8D,stroke-width:3px,color:#2C3E50,font-weight:bold,font-size:16px;

    %% Stilleri Uyguluyoruz
    class Ajan1,Ajan2 ajanStyle;
    class Cevre cevreStyle;

    %% Bağlantı Çizgilerini (Okları) Belirginleştiriyoruz
    linkStyle default stroke:#34495E,stroke-width:2.5px;
```