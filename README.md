````markdown
# 🧩 C# Erişim Belirteçleri (Access Modifiers) Uygulaması

Bu proje, C# programlama dilindeki temel erişim belirteçlerinin (`public`, `private`, `protected`, `internal`, `protected internal`) kullanımını ve farklı senaryolardaki davranışlarını gösteren bir Windows Forms uygulamasıdır.

---

## ⚙️ Özellikler

- 🌍 **public:** Her yerden erişilebilir üyeler.
- 🔒 **private:** Yalnızca tanımlandığı sınıf içinden erişilebilir üyeler.
- 🧬 **protected:** Tanımlandığı sınıf ve ondan türetilen sınıflar içinden erişilebilir üyeler.
- 📦 **internal:** Yalnızca aynı derleme (assembly) içinden erişilebilir üyeler.
- 🔐 **protected internal:** Aynı derleme içinden veya türetilmiş sınıflar üzerinden erişilebilir üyeler.
- 🧪 **Örnek Uygulama:** `Urun` sınıfı üzerinden erişim belirteçlerinin davranışlarını gösterir.

---

## 🛠️ Teknik Detaylar

- 💻 **Dil:** C#
- 🪟 **Arayüz:** Windows Forms (WinForms)
- 🧱 **Mimari:** Sınıf yapıları ve nesne yönelimli programlama (OOP)

---

## 🎯 Kazanımlar

- 🔐 **Kapsülleme (Encapsulation):** Veri gizliliği ve erişim kontrolü
- 🖥️ **UI & Logic Senkronizasyonu:** Form üzerinden sınıflarla etkileşim
- 📁 **Proje Yönetimi:** `.sln` ve `.csproj` yapısının kullanımı

---

## 🚀 Kurulum

Projeyi yerel makinenizde çalıştırmak için:

1. 📥 Depoyu klonlayın veya ZIP olarak indirin:

```bash
git clone https://github.com/kullaniciadi/Belirtecler.git
````

2. 📂 `Belirtecler-master` klasörüne gidin.

3. 🧾 `Belirtecler.sln` dosyasını Visual Studio ile açın.

4. ▶️ Projeyi derleyip çalıştırın.

---

## 🖥️ Kullanım

Uygulama, `Form1` üzerinde bir `Urun` nesnesi oluşturur ve erişim belirteçlerinin nasıl çalıştığını gösterir.

Form üzerindeki butonlarla:

* 📦 Ürün bilgileri görüntülenir
* 💰 Fiyat güncellenir
* 📊 Stok ve kategori bilgileri düzenlenir

---

## 🧱 Urun Sınıfı Yapısı

```csharp
public class Urun
{
    public string UrunAdi { get; set; }   // 🌍 Public özellik
    private decimal _fiyat;               // 🔒 Private özellik
    protected int StokMiktari;           // 🧬 Protected özellik
    internal string Kategori;            // 📦 Internal özellik
    protected internal string Uretici;   // 🔐 Protected Internal özellik

    public Urun(string ad, decimal fiyat, string kategori, int stok, string uretici)
    {
        // constructor
    }

    private void FiyatGuncelle(decimal yeniFiyat) { }

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
        _fiyat = yeniFiyat;
    }
}
```

---

## 📁 Proje Yapısı

```
Belirtecler-master/
├── 📄 Belirtecler.csproj
├── 📄 Belirtecler.sln
├── 🪟 Form1.Designer.cs
├── 🪟 Form1.cs
├── 🧾 Form1.resx
├── 📜 LICENSE
├── 🚀 Program.cs
└── 📘 README.md
```

---

## 🤝 Katkıda Bulunma

Katkılarınız memnuniyetle karşılanır. Herhangi bir hata bulursanız veya yeni özellik eklemek isterseniz issue açabilir veya pull request gönderebilirsiniz.

---

## 👨‍💻 Geliştirici

⭐ **Şilan Pehlivan**

```
```
