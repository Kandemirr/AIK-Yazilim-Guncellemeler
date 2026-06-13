# Müfredat Güncelleme Kanalı

`mufredat-manifest.json`, Ders Dağıtım Programının açılışta denetlediği güncel
paketi gösterir. Paketler GitHub Releases altında yayımlanır.

## Güvenlik ve veri koruma

- Paket yalnız HTTPS üzerinden indirilir.
- İndirilen dosyanın SHA-256 özeti manifestteki değerle aynı olmalıdır.
- Paket boyutu 10 MB ile sınırlıdır.
- Kullanıcının oluşturduğu özel müfredatlar ve kullanıcı dersleri değiştirilmez.
- Yeni sürüm eski sürümün üzerine sessizce yazılmaz; paket sürümü karşılaştırılır.

## Yeni yıl paketi

1. MEB'in resmî haftalık ders çizelgeleri incelenir.
2. Her profil için ders adı, sınıf seviyesi, zorunlu/seçmeli durumu, haftalık saat,
   saat seçenekleri ve varsayılan dağıtım biçimi pakete yazılır.
3. Paket yeni bir sürüm etiketiyle GitHub Releases bölümüne yüklenir.
4. Paket SHA-256 özeti alınır ve `mufredat-manifest.json` güncellenir.

Uygulama kodunun veya kurulum EXE'sinin değiştirilmesi gerekmez.
