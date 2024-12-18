# Development-Applications

## Proje Açıklaması
Bu proje, *Trendyol* için geliştirilen örnek bir Java uygulamasıdır. Kıyafetlerin, renklerin ve modellerin sınıflandırılması için temel bir sınıf yapısı içerir. *Nesne Yönelimli Programlama (OOP)* prensipleri kullanılmıştır.

---

## Kullanılan Teknolojiler
- *Java*: Geliştirme dili
- *Maven*: (İsteğe bağlı) Proje bağımlılık yönetimi

---

## Kod Dosyaları

### *1. Clothing.java*
```java
package com.trendyol;

public class Clothing {
    private String name;
    private Color color;
    private Model model;

    public Clothing(String name, Color color, Model model) {
        this.name = name;
        this.color = color;
        this.model = model;
    }

    public void displayClothingInfo() {
        System.out.println("Kıyafet Adı: " + name);
        System.out.println("Renk: " + color.getColorName());
        System.out.println("Model: " + model.getModelName());
    }
}



Main.java

package com.trendyol;

public class Main {
    public static void main(String[] args) {
        // Kıyafet nesneleri oluşturuluyor
        Clothing tshirt = new Clothing("T-Shirt", "Kırmızı", "Yaz Koleksiyonu");
        Clothing coat = new Clothing("Kaban", "Mavi", "Kış Koleksiyonu");
        Clothing jeans = new Clothing("Kot Pantolon", "Siyah", "Günlük Giyim");

        // Bilgileri ekrana yazdırma
        System.out.println("------ Kıyafet Bilgileri ------");
        tshirt.displayClothingInfo();
        System.out.println("------------------------------");
        coat.displayClothingInfo();
        System.out.println("------------------------------");
        jeans.displayClothingInfo();
    }
}


Örnek çıktı:

----- Kıyafet Bilgileri ------
Kıyafet Adı: T-Shirt
Renk: Kırmızı
Model: Yaz Koleksiyonu
------------------------------
Kıyafet Adı: Kaban
Renk: Mavi
Model: Kış Koleksiyonu
------------------------------
Kıyafet Adı: Kot Pantolon
Renk: Siyah
Model: Günlük Giyim

Projeye katkıda bulunmak isteyenler pull request gönderebilir.
