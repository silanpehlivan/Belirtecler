````markdown id="clean_readme_final"
# 🧩 C# Erişim Belirteçleri (Access Modifiers) Uygulaması

Bu proje, C# programlama dilinde kullanılan erişim belirteçlerini (`public`, `private`, `protected`, `internal`, `protected internal`) Windows Forms (WinForms) ortamında örnek bir `Urun` sınıfı üzerinden açıklayan bir uygulamadır.

---

## ⚙️ Özellikler

- 🌍 **public:** Her yerden erişilebilir üyeler
- 🔒 **private:** Sadece tanımlandığı sınıf içinden erişilebilir üyeler
- 🧬 **protected:** Sınıf ve türetilmiş sınıflar tarafından erişilebilir üyeler
- 📦 **internal:** Aynı proje (assembly) içinden erişilebilir üyeler
- 🔐 **protected internal:** Aynı assembly içinden veya türetilmiş sınıflardan erişilebilir üyeler
- 🧪 **Örnek Kullanım:** `Urun` sınıfı üzerinden tüm erişim türleri gösterilmektedir

---

## 🛠️ Teknik Detaylar

- 💻 Dil: C#
- 🪟 Arayüz: Windows Forms (WinForms)
- 🧱 Yapı: Nesne Yönelimli Programlama (OOP)

---

## 🎯 Kazanımlar

- 🔐 Kapsülleme (Encapsulation) mantığını öğrenme
- 🧠 Erişim belirteçlerinin farklarını anlama
- 🖥️ WinForms ile sınıf etkileşimi kurma
- 📁 .NET proje yapısını tanıma

---

## 🚀 Kurulum

1. 📥 Projeyi klonlayın veya indirin:

```bash
git clone https://github.com/kullaniciadi/Belirtecler.git
````

2. 📂 Proje klasörüne girin:

```
Belirtecler-master
```

3. 🧾 `Belirtecler.sln` dosyasını Visual Studio ile açın

4. ▶️ Projeyi çalıştırın

---

## 🖥️ Kullanım

Uygulama çalıştırıldığında `Form1` üzerinde bir `Urun` nesnesi oluşturulur.

Butonlar aracılığıyla:

* 📦 Ürün bilgileri görüntülenir
* 💰 Fiyat güncellenir
* 📊 Stok ve kategori işlemleri yapılır

---

## 🧱 Urun Sınıfı Yapısı

```csharp
public class Urun
{
    public string UrunAdi { get; set; }
    private decimal _fiyat;
    protected int StokMiktari;
    internal string Kategori;
    protected internal string Uretici;

    public Urun(string ad, decimal fiyat, string kategori, int stok, string uretici)
    {
        UrunAdi = ad;
        _fiyat = fiyat;
        Kategori = kategori;
        StokMiktari = stok;
        Uretici = uretici;
    }

    private void FiyatGuncelle(decimal yeniFiyat)
    {
        _fiyat = yeniFiyat;
    }

    public string UrunBilgisiGetir()
    {
        return $"{UrunAdi} - {Kategori}";
    }

    protected void StokGuncelle(int yeniStok)
    {
        StokMiktari = yeniStok;
    }

    public void StokGuncellePublic(int yeniStok)
    {
        StokGuncelle(yeniStok);
    }

    internal void KategoriDegistir(string yeniKategori)
    {
        Kategori = yeniKategori;
    }

    protected internal void UreticiDegistir(string yeniUretici)
    {
        Uretici = yeniUretici;
    }

    public void FiyatGuncellePublic(decimal yeniFiyat)
    {
        FiyatGuncelle(yeniFiyat);
    }
}
```

---

## 📁 Proje Yapısı

```
Belirtecler-master/
├── Belirtecler.csproj
├── Belirtecler.sln
├── Form1.Designer.cs
├── Form1.cs
├── Form1.resx
├── Program.cs
├── LICENSE
└── README.md
```

---

## 🤝 Katkıda Bulunma

Katkılarınızı memnuniyetle karşılıyoruz. Hata bildirimi veya yeni özellik önerileri için issue açabilir veya pull request gönderebilirsiniz.

---

## 👨‍💻 Geliştirici

⭐ **Şilan Pehlivan**

```
