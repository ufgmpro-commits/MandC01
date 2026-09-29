# M&C Projesi — Teknik Çerçeve

Bu belge, proje sahibi tarafından belirlenen temel teknik kararları kaydeder. Proje ayrıntıları netleştikçe güncellenecektir.

## Hedef platform

- Geliştirme ortamı: Visual Studio 2022
- Sunucu uygulaması: C#
- Hedef framework: .NET Framework 4.8
- Masaüstü arayüz teknolojisi: Windows Forms
- İşletim sistemi hedefi: Eski Windows 10 kurulumları dahil Windows ortamları

## Temel mimari

M&C, sunucu ve istemci bileşenlerinden oluşacaktır.

### Server

- C# ve Windows Forms ile geliştirilecektir.
- Ana iş mantığını ve sunucu görevlerini yürütecektir.
- Ayrıntılı sorumlulukları proje sahibi tarafından sağlanacak gereksinimlerle belirlenecektir.

### Client

- Temel yaklaşım JavaScript ile web tarayıcısı üzerinden çalışan istemcidir.
- İhtiyaç halinde istemci tarafındaki işletim sistemi entegrasyonları için .NET Framework 4.8 tabanlı DLL geliştirilebilir.
- Gereksinim doğarsa istemci tarafında ayrıca Windows Forms bileşeni veya uygulaması kullanılabilir.

## Mimari ilkeler

- Eski Windows 10 sistemleriyle uyumluluk korunacaktır.
- Tarayıcı tabanlı istemci öncelikli olacaktır.
- Yerel Windows veya .NET yetenekleri yalnızca gereksinimin tarayıcı katmanında karşılanamadığı durumlarda eklenecektir.
- Teknik kararlar, protokoller, desteklenen tarayıcılar ve dağıtım yöntemi gereksinimler netleştikçe bu belgede kayıt altına alınacaktır.

## Açık konular

Aşağıdaki başlıklar proje sahibi tarafından verilecek ayrıntılı bilgilendirmeyle netleştirilecektir:

- M&C ürününün amacı ve ana kullanım senaryoları
- Server ile Client arasındaki iletişim protokolü
- Tek makine, yerel ağ ve internet kullanım modelleri
- Veri saklama ve veritabanı tercihleri
- Kimlik doğrulama ve yetkilendirme
- Hedef tarayıcılar ve WebView gereksinimi
- Kurulum, güncelleme ve çevrimdışı çalışma
- Donanım ve üçüncü taraf sistem entegrasyonları
