<div align="center">

# C# Erişim Belirteçleri

**Nesne yönelimli programlama ve kapsülleme**

![C#](https://img.shields.io/badge/C%23-2563eb?style=flat-square)
![Windows Forms](https://img.shields.io/badge/Windows%20Forms-0891b2?style=flat-square)
[![MIT License](https://img.shields.io/badge/License-MIT-16a34a?style=flat-square)](LICENSE)

C# erişim belirteçlerinin davranışını bir ürün sınıfı ve masaüstü arayüzü üzerinden gösteren eğitim uygulaması.

</div>

---

## Öne Çıkanlar

- public, private, protected ve internal kapsamları
- Ürün bilgileri üzerinden sınıf etkileşimi
- WinForms ile temel nesne yönelimli programlama

## Teknolojiler

C# · Windows Forms

## Teknik yaklaşım

Ürün sınıfındaki alan ve metotlar farklı erişim kapsamlarıyla tanımlanır; form olayları public metotlar üzerinden nesnenin durumunu değiştirir. Kapsülleme ile arayüz olaylarının ilişkisini gösterir.

## Kodu incelemeye başlayın

- [Form1.cs](Form1.cs)
- [Program.cs](Program.cs)

## Kapsam ve sınırlar

Erişim belirteçleri kod düzeyinde kapsülleme sağlar; kullanıcı yetkilendirmesi veya güvenlik sınırı oluşturmaz.

<details>
<summary><strong>Kurulum, kullanım ve teknik ayrıntılar</strong></summary>

Bu proje, C# programlama dilinde kullanılan erişim belirteçlerini (`public`, `private`, `protected`, `internal`, `protected internal`) Windows Forms (WinForms) ortamında örnek bir `Urun` sınıfı üzerinden açıklayan bir uygulamadır.

---

## Özellikler

- **public:** Her yerden erişilebilir üyeler
- **private:** Sadece tanımlandığı sınıf içinden erişilebilir üyeler
- **protected:** Sınıf ve türetilmiş sınıflar tarafından erişilebilir üyeler
- **internal:** Aynı proje (assembly) içinden erişilebilir üyeler
- **protected internal:** Aynı assembly içinden veya türetilmiş sınıflardan erişilebilir üyeler
- **Örnek Kullanım:** `Urun` sınıfı üzerinden erişim belirteçlerinin davranışı gösterilmektedir

---

## Teknik Detaylar

- Dil: C#
- Arayüz: Windows Forms (WinForms)
- Yapı: Nesne Yönelimli Programlama (OOP)

---

## Kazanımlar

- Kapsülleme (Encapsulation) mantığını öğrenme
- Erişim belirteçlerinin kullanım farklarını anlama
- WinForms ile sınıf etkileşimi kurma
- .NET proje yapısını tanıma

---

## Kurulum

1.  Projeyi klonlayın veya ZIP olarak indirin  
2.  Proje klasörüne girin  
3.  Visual Studio ile `.sln` dosyasını açın  
4.  Projeyi derleyip çalıştırın  

---

## Kullanım

Uygulama çalıştırıldığında `Form1` üzerinden bir `Urun` nesnesi oluşturulur.

Kullanıcı:
- Ürün bilgilerini görüntüleyebilir  
- Fiyat bilgilerini güncelleyebilir  
- Stok ve kategori işlemlerini yapabilir  

---

## Proje Yapısı

- Belirtecler.csproj  
- Belirtecler.sln  
- Form1 tasarım ve kod dosyaları  
- Program.cs  
- LICENSE  
- README.md  

---

## Katkıda Bulunma

Katkılarınız memnuniyetle karşılanır. Hata bildirimi veya yeni özellik önerileri için issue açabilir veya pull request gönderebilirsiniz.

---


</details>

---

<div align="center">

**© 2024 Şilan PEHLİVAN**

Bu proje MIT lisansı kapsamında sunulmaktadır. Kullanım ve dağıtım koşulları: [LICENSE](LICENSE).

</div>
