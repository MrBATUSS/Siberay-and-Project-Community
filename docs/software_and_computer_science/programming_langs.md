# 🚀 Yazılım Dillerini Anlama ve Başlangıç Rehberi

Bu rehber, yazılıma sıfırdan başlamak isteyen ama *"Hangi dille başlamalıyım?"*, *"Bu diller nasıl çalışıyor?"* veya *"Hangi dil ne işe yarar?"* sorularına yanıt arayan kulüp üyelerimiz için hazırlanmıştır.

---

## 🧠 Yazılım Dili Nedir ve Nasıl Çalışır?

Bilgisayarlar temelde sadece **0 ve 1** sayılarını (elektrik var/yok) anlar. Buna **Makine Dili (Machine Code)** denir. Ancak insanların 0 ve 1'lerle karmaşık programlar yazması imkansız gibidir.

Yazılım dilleri, insan dili (İngilizce) ile bilgisayar dili arasındaki bir köprüdür. Yazdığınız kodların bilgisayar tarafından anlaşılabilmesi için iki temel yöntem kullanılır:

1. **Derlenen Diller (Compiled Languages):**
   * **Mantık:** Yazdığınız tüm kodlar bir araç (Derleyici/Compiler) tarafından tek seferde makine diline (0 ve 1'lere) dönüştürülür ve bir çalıştırılabilir dosya (`.exe` vb.) oluşturulur.
   * **Özellikler:** Çok hızlı çalışırlar ama hata ayıklamak biraz daha zor olabilir.
   * **Örnekler:** C, C++, Rust, Go.

2. **Yorumlanan Diller (Interpreted Languages):**
   * **Mantık:** Kodlar bir yorumlayıcı (Interpreter) tarafından satır satır okunur ve anında çalıştırılır.
   * **Özellikler:** Öğrenmesi ve test etmesi çok kolaydır, ancak derlenen dillere göre bir tık daha yavaş çalışabilirler.
   * **Örnekler:** Python, JavaScript, PHP.
  
* **Önerilen Kaynaklar**
  * **[ByteBloodz (YouTube)](https://www.youtube.com/@ByteBloodz/videos)**
---

## 🛠️ Popüler Yazılım Dilleri ve Kullanım Alanları

### 1. 🐍 Python
* **Neden Tercih Edilir?** Sözdizimi (syntax) insan diline çok yakındır. Öğrenmesi en kolay dildir. Devasa bir kütüphane ekosistemine sahiptir.
* **Nasıl Çalışır?** Yorumlanan bir dildir.
* **Nerede Kullanılır?**
  * Yapay Zeka ve Makine Öğrenmesi (AI / ML)
  * Veri Bilimi ve Analizi
  * Web Geliştirme (Django, Flask)
  * Otomasyon ve Scripting
* **Kimler Seçmeli?** Yazılıma **sıfırdan başlayanlar**, yapay zeka ve veriyle ilgilenenler.

* **Önerilen Kaynaklar**
  * **[Btk Akademi](http://btkakademi.gov.tr/portal/course/sifirdan-ileri-seviye-python-programlama-5877)**
  * **[Burak Kocaaslan (Youtube)](https://www.youtube.com/watch?v=702lP_gRkD8&list=PLP6TjrWzAOA21-_OzxJ8CGn7VihdYVBcl)**

---

### 2. 🌐 JavaScript (JS)
* **Neden Tercih Edilir?** İnternet dünyasının (web sitelerinin) ana dilidir. Tarayıcısı olan her cihazda doğrudan çalışır. Hem ön yüz (frontend) hem arka yüz (backend) geliştirilebilir.
* **Nasıl Çalışır?** Yorumlanan (JIT compiled) bir dildir.
* **Nerede Kullanılır?**
  * Etkileşimli Web Siteleri (React, Vue, Angular)
  * Sunucu Tarafı (Node.js)
  * Mobil Uygulamalar (React Native)
* **Kimler Seçmeli?** Web tasarımı, siteler ve kullanıcı arayüzleri geliştirmek isteyenler.

* **Önerilen Kaynaklar**
  * **[Btk Akademi](https://www.btkakademi.gov.tr/portal/course/javascript-8099)**
  * **[JetBrains Academy (İngilizce dökümantasyon)](https://academy.jetbrains.com/course/26697)**
  * **[PROTOTURK](https://www.youtube.com/watch?v=8A7RWDgkXgg&list=PLfAfrKyDRWrGIER-yXLliD_47T_5FY8Qd)** !(data:image/png;base64,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)
---

### 3. ☕ Java
* **Neden Tercih Edilir?** *"Bir kere yaz, her yerde çalıştır"* felsefesine sahiptir. Güvenli, disiplinli ve kurumsal şirketler tarafından çok tercih edilen bir dildir.
* **Nasıl Çalışır?** Kodlar önce *Bytecode*'a dönüştürülür, ardından **JVM** (Java Virtual Machine) adındaki sanal makinede çalıştırılır.
* **Nerede Kullanılır?**
  * Android Mobil Uygulama Geliştirme
  * Büyük Şirketlerin Arka Yüz (Backend) Sistemleri
  * Finans ve Bankacılık Yazılımları
* **Kimler Seçmeli?** Nesne Yönelimli Programlamayı (OOP) katı ve disiplinli kurallarla öğrenmek isteyenler.


* **Önerilen Kaynaklar**
  * **[Yazılım Teknolojileri (YouTube)](https://www.youtube.com/watch?v=TewGWJsyeJY&list=PLzupOkYTW5dTiYvmh9N4NPRrYBgZeeruQ)**
  * **[JetBrains Academy (İngilizce dökümantasyon)](https://academy.jetbrains.com/course/18905)**
---

### 4. 🔷 C# (C-Sharp)
* **Neden Tercih Edilir?** Microsoft tarafından geliştirilmiştir. Çok yönlüdür ve oyun motoru Unity ile doğrudan entegredir.
* **Nasıl Çalışır?** Java'ya benzer; kodlar `.NET` çalışma zamanı (CLR) üzerinde çalışır.
* **Nerede Kullanılır?**
  * Oyun Geliştirme (Unity Game Engine)
  * Windows Masaüstü Uygulamaları
  * Web Backend (ASP.NET Core)
* **Kimler Seçmeli?** **Oyun geliştirmek isteyenler** ve Microsoft ekosisteminde ilerlemek isteyenler.

---

### 5. ⚡ C ve C++
* **Neden Tercih Edilir?** Donanıma ve belleğe (RAM) doğrudan erişim sağlar. İnanılmaz derecede hızlı ve performanslıdır.
* **Nasıl Çalışır?** Doğrudan makine koduna derlenir.
* **Nerede Kullanılır?**
  * Oyun Motorları (Unreal Engine)
  * Gömülü Sistemler ve IoT (Arduino, Sensörler, Robotik)
  * İşletim Sistemleri ve Sürücüler
* **Kimler Seçmeli?** Donanımla, robotikle, microchip'lerle ilgilenenler veya sistem mantığını en derinden anlamak isteyenler.

---

## 🎯 Hiç Bilmeyen Biri Nereden Başlamalı?

Yazılıma başlarken en büyük hata **birden fazla dili aynı anda öğrenmeye çalışmaktır**. Mantık tek bir dilde oturtulduğunda, diğer dillere geçmek sadece birkaç haftalık bir sözdizimi (syntax) alışma sürecinden ibarettir.

### 🧭 Adım Adım Yol Haritası:

1. **Mantığı Kavrayın (Algoritma):**
   * Kod yazmadan önce **Algoritma Mantığı** ve **Akış Şeması (Flowchart)** kavramlarını öğrenin. Problem nasıl küçük parçalara bölünür? (Değişkenler, Koşullar, Döngüler).

2. **İlk Dilinizi Seçin:**
   * **Genel Başlangıç & Yapay Zeka / Otomasyon için:** **Python**
   * **Görsel & Web Tasarımı için:** **JavaScript**
   * **Oyun Geliştirmek için:** **C#**
   * **Robottik & Donanım için:** **C / C++** veya **Python**

3. **Geliştirme Ortamınızı (IDE) Kurun:**
   * Kodlarınızı yazmak için **VS Code (Visual Studio Code)** indirip kurun.

4. **Proje Odaklı İlerleyin:**
   * Sadece video izlemeyin veya kitap okumayın. Küçük de olsa uygulamalar yapın (Örn: Hesap makinesi, Taş-Kağıt-Makas oyunu, To-Do List uygulaması).

---

> 💡 **Unutmayın:** En iyi programlama dili, geliştirmek istediğiniz projeye ve hedefinize en uygun olan dildir!
