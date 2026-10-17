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

---

### 2. 🌐 JavaScript (JS)
* **Neden Tercih Edilir?** İnternet dünyasının (web sitelerinin) ana dilidir. Tarayıcısı olan her cihazda doğrudan çalışır. Hem ön yüz (frontend) hem arka yüz (backend) geliştirilebilir.
* **Nasıl Çalışır?** Yorumlanan (JIT compiled) bir dildir.
* **Nerede Kullanılır?**
  * Etkileşimli Web Siteleri (React, Vue, Angular)
  * Sunucu Tarafı (Node.js)
  * Mobil Uygulamalar (React Native)
* **Kimler Seçmeli?** Web tasarımı, siteler ve kullanıcı arayüzleri geliştirmek isteyenler.

---

### 3. ☕ Java
* **Neden Tercih Edilir?** *"Bir kere yaz, her yerde çalıştır"* felsefesine sahiptir. Güvenli, disiplinli ve kurumsal şirketler tarafından çok tercih edilen bir dildir.
* **Nasıl Çalışır?** Kodlar önce *Bytecode*'a dönüştürülür, ardından **JVM** (Java Virtual Machine) adındaki sanal makinede çalıştırılır.
* **Nerede Kullanılır?**
  * Android Mobil Uygulama Geliştirme
  * Büyük Şirketlerin Arka Yüz (Backend) Sistemleri
  * Finans ve Bankacılık Yazılımları
* **Kimler Seçmeli?** Nesne Yönelimli Programlamayı (OOP) katı ve disiplinli kurallarla öğrenmek isteyenler.

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
