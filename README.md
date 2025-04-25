# Üretim Hattı Çizelgeleme Optimizasyonu

![Java](https://img.shields.io/badge/Java-17-blue)
![Dinamik Programlama](https://img.shields.io/badge/Algorithm-Dynamic_Programming-green)

Bu proje, farklı makinelerde çalıştırılabilen işlerin en optimal şekilde çizelgelenmesi için dinamik programlama tabanlı bir çözüm sunar.

## Problem Tanımı

Bir üretim hattında:
- `n` adet sıralı iş tamamlanmalıdır
- `m` adet farklı makine kullanılabilir
- Her işin her makinedeki işlem süresi farklıdır
- Makineler arası geçişlerin ek maliyetleri vardır

**Amaç:** Toplam üretim süresini (işlem + geçiş süreleri) minimize etmek

## Teknolojiler

- Java 17
- Dinamik Programlama Algoritması

## Proje Yapısı
src/
├── main/
│ └── java/
│ └── UretimHattiCizelgeleme.java
test/
├── java/
│ └── UretimHattiCizelgelemeTest.java
README.md


## Kullanım

1. Ana sınıfı çalıştırın:

```java
public class Main {
    public static void main(String[] args) {
        int[][] isler = {{5,7,3}, {2,6,1}, {4,3,2}};
        int[][] gecisMaliyetleri = {{0,2,1}, {1,0,3}, {2,1,0}};
        
        int sonuc = UretimHattiCizelgeleme.minimumUretimSuresiHesapla(isler, gecisMaliyetleri);
        System.out.println("Minimum toplam süre: " + sonuc);
    }
}
Algoritma Analizi
Karmaşıklık	Değer
Zaman	O(n*m²)
Uzay	O(n*m)
n = İş sayısı
m = Makine sayısı

Örnek Çalışma
Girdi:

İşler:
[5, 7, 3]
[2, 6, 1] 
[4, 3, 2]

Geçiş Maliyetleri:
[0, 2, 1]
[1, 0, 3]
[2, 1, 0]
Çıktı:

Minimum toplam süre: 7
Lisans
Bu proje MIT lisansı altında lisanslanmıştır.

Katkıda Bulunma
Projeyi fork'layın

Yeni özellik dalı oluşturun

Değişikliklerinizi commit edin

Dala push yapın

Pull Request oluşturun
