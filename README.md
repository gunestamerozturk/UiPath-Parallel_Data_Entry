# 🔄 UiPath Parallel Data Entry – Web ve Masaüstü Uygulamasına Eşzamanlı Veri Kaydı

Bu proje, Excel tablosundaki müşteri verilerini aynı anda hem bir **web uygulamasına** hem de bir **masaüstü uygulamasına** kaydeden bir **UiPath Studio** otomasyonudur. Uygulama, paralel çalışma mantığını öğretmek amacıyla geliştirilmiş olup, Udemy üzerinde alınan Complete UiPath RPA Developer Course: Build 7 Robots
isimli kursun pratik etkinliğidir.

Web tarafında veri girişleri, eğitmene ait olan **https://www.theautomationchallenge.com/crm** adresine yapılmaktadır. Masaüstü tarafı ise eğitmenin kurs için hazırladığı basit bir data entry uygulamasıdır.

Bu proje sayesinde UiPath’te **paralel iş akışları**, **workflow yönetimi** ve **eşzamanlı süreç yürütme** adımları pratik edilmiştir.

---

## 🚀 Projenin Amacı

Bu uygulamanın amacı, bir veri kaynağından (Excel) alınan bilgilerin **eşzamanlı olarak iki farklı platforma** (web ve masaüstü) işlenmesini sağlayarak UiPath'in paralel çalışma yeteneklerini öğrenmektir.

Robotun temel hedefleri:

- Excel dosyasından müşteri verilerini okumak  
- Verileri web CRM uygulamasına kaydetmek  
- Verileri masaüstü veri giriş uygulamasına kaydetmek  
- İki iş akışını **aynı anda paralel olarak çalıştırmak**

---

## 🖥️💻 Kullanılan Uygulamalar

- **Web CRM Uygulaması:**  
  https://www.theautomationchallenge.com/crm

- **Masaüstü Veri Giriş Uygulaması:**  
  Kurs eğitmeni tarafından oluşturulmuş, gerçek veri tabanı bağlantısı bulunmayan basit bir demo uygulaması

---

## 🧩 Proje Yapısı

Proje üç ana workflow’dan oluşur:

- **Main.xaml**  
  - Run Both Workflows (Simultaneous) kullanılarak iki sürecin paralel yürütülmesi sağlanır.

- **WebDataCapturing.xaml**  
  - Web CRM sayfasını açar  
  - Form alanlarını doldurur  
  - Veriyi gönderir  

- **DesktopDataCapturing.xaml**  
  - Masaüstü data entry uygulamasını başlatır  
  - Form alanlarını doldurur  
  - Veriyi gönderir  

---

## ⚙️ Uygulama Nasıl Çalışır?

1. Excel dosyasındaki müşteri bilgileri okunur.  
2. Main workflow, **Run Both Workflows (Simultaneous)** aktivitesini kullanarak hem web hem masaüstü iş akışlarını aynı anda çağırır.  
3. WebDataCapturing ve DesktopDataCapturing workflow’ları kendi süreçlerini paralel olarak yürütür.  
4. Her iki uygulama da ilgili müşteri verilerini işler ve kayıt işlemi tamamlanır.

Bu yapı sayesinde UiPath’te **eşzamanlı süreç yönetimi**, **aynı veri kaynağını iki farklı platformda işleme** ve **workflow bölme** prensipleri uygulanır.

---

## 🧠 Kullanılan UiPath Aktiviteleri

- Read Range  
- Parallel 
- Use Application Browser  
- Type Into  
- Click  
- Workflow Invocation aktiviteleri  

---

## 📊 Proje Akış Özeti

- Excel’den müşteri verilerini oku  
- WebDataCapturing workflow → CRM sitesine kaydet  
- DesktopDataCapturing workflow → Masaüstü uygulamasına kaydet  
- Her iki workflow **eşzamanlı olarak çalışır**  
- Kayıt tamamlanır  

---

## 🎯 Kazanımlar

Bu proje ile:

- Paralel workflow çalıştırma  
- Web otomasyonu  
- Masaüstü uygulama otomasyonu  
- Form doldurma  
- Tablodan veri okuma  
- Workflow mimarisi tasarlama  

gibi temel UiPath yetkinliklerinde pratik yapılmıştır.

