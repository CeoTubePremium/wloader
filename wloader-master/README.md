CeoTube Premium

# wloader

Çin'den herhangi bir arka kapı yükleyicisi kullanmadan Windows 10 PRO Aktivatörü ve
artık bir veya iki hafta geçerli olan herhangi bir crack'e de ihtiyacınız olmayacak. 

Bu komut dosyası cmd için yazılmıştır. Bu komut dosyası
ayrıca tüm bloatware'leri Windows 10'dan kaldırıyor. Betiği ihtiyaçlarınıza göre düzenleyin.


Etkinleştirme kimliği dahil olmak üzere daha ayrıntılı lisans bilgilerini görüntülemek için,
kurulum kimliği ve diğer ayrıntılar - aşağıdaki komutu çalıştırın:
```powershell
slmgr.vbs /dlv
```

### Windows 11 PRO Yükleyiciyi çalıştırın:

Greetings to: [Minionguyjpro](https://gist.github.com/Minionguyjpro/d913b3931e844ad8ad9a758a4aca4b63) - Author

```powershell
sc config LicenseManager start= auto & net start LicenseManager
sc config wuauserv start= auto & net start wuauserv
changepk.exe /productkey VK7JG-NPHTM-C97JM-9MPGT-3V66T
exit
```

### Aşağıya kopyalayıp yapıştırarak Windows 10/11'i PRO'ya yükseltin:

```powershell
slmgr /ipk W269N-WFGWX-YVC9B-4J6C9-T83GX
slmgr /skms kms8.msguides.com
slmgr /ato
```

### Windows 10 Enterprise 10.0.19043'ü etkinleştirin N/A Build 19043, tam örnek 

```powershell
slmgr.vbs /ipk DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
slmgr /skms kms8.msguides.com
slmgr.vbs /ato
```
### Lisans Bitiş Tarihini Görüntüle

```powershell
slmgr.vbs /xpr
```
### Aktivasyon Anahtarını Kaldır

```powershell
slmgr.vbs /upk
```
### Ürün Anahtarını Kaldırma

 ```powershell
slmgr.vbs /cpky
```

### Lisans Anahtarınızı Belirleyin

```powershell
slmgr.vbs /ipk #####-#####-#####-#####-#####
```

### `slmgr`yi Uzaktan Kumandayla Yapılandırın

```powershell
slmgr.vbs computername username password /option
```


### Windows 10 Keys

```
Home:                TX9XD-98N7V-6WMQ6-BX7FG-H8Q99
Home N:              3KHY7-WNT83-DGQKR-F7HPR-844BM
Professional:        W269N-WFGWX-YVC9B-4J6C9-T83GX
rofessional N:      MH37W-N47XK-V7XM9-C7227-GCQG9
Education:           NW6C2-QMPVW-D7KKK-3GKT6-VCFB2
Education N:         2WH4N-8QGBV-H22JP-CT43Q-MDWWJ
Enterprise:          NPPR9-FWDCX-D2C8J-H872K-2YT43
Enterprise N:        DPH2V-TTNVB-4X9Q3-TJR4H-KHJW4
Enterprise LSTB:     WNMTR-4C88C-JK8YV-HQ7T2-76DF9
Enterprise LSTB N:   2F77B-TNFGY-69QQF-B8YKP-D69TJ
```

### KMS Sunucuları

* Add keys via 

```powershell
slmgr /skms <server>
```

* Bazı Kullanılabilir Sunucular

```powershell
kms.digiboy.ir
kms.cangshui.net
hq1.chinancce.com
54.223.212.31
kms.cnlic.com
kms.chinancce.com
kms.ddns.net
franklv.ddns.net
k.zpale.com
m.zpale.com
mvg.zpale.com
kms.shuax.com
kensol263.imwork.net:1688
xykz.f3322.org
kms789.com
dimanyakms.sytes.net:1688
kms.03k.org:1688
```

### SLMGR Komutları

```powershell
slmgr.exe -ato                                    Windows lisansını ve ürün anahtarını Microsoft sunucusunda etkinleştirin.
slmgr.exe -atp                                    Onay_Kimliği Kullanıcı tarafından sağlanan Onay Kimliği ile Windows'u etkinleştirin.
slmgr.exe -ckms                                   Varsayılan olarak kullanılan KMS sunucusunun adını ve varsayılana bağlantı noktasını temizleyin.
slmgr.exe -cpky                                   Ürün anahtarını kayıt defterinden temizleyin (ifşa saldırılarını önler).
slmgr.exe -dli                                    Aktivasyon durumu ve kısmi ürün anahtarı ile mevcut lisans bilgilerini görüntüleyin.
slmgr.exe -dlv                                    Ayrıntılı, -dli'ye benzer, ancak daha fazla bilgi içerir.
slmgr.exe -dti                                    Çevrimdışı etkinleştirme için Kurulum Kimliğini görüntüleyin.
slmgr.exe -ipk                                    Anahtar xxxxx-xxxxx-xxxx-xxxxx-xxxxx olarak sağlanan yeni bir ürün anahtarını girin.
slmgr.exe -ilc                                    License_file Kurulum lisansı.
slmgr.exe -rilc                                   Sistem lisans dosyalarını yeniden yükleyin.
slmgr.exe -rearm                                  Makinenin değerlendirme süresini/lisans durumunu ve aktivasyon durumunu sıfırlayın.
slmgr.exe -skms activationservername:port         Toplu Lisanslama KMS sunucusunu ve/veya KMS aktivasyonu için kullanılan bağlantı noktasını ayarlayın (Windows sürümünüz tarafından destekleniyorsa).
slmgr.exe -skhc                                   KMS ana bilgisayar önbelleğini etkinleştir (varsayılan), bu, çalışan bir KMS ana bilgisayarının ilk keşfinden sonra DNS önceliği ve ağırlığının kullanımını engeller.
slmgr.exe -ckhc                                   KMS ana bilgisayar önbelleğini devre dışı bırakın. Bu ayar, istemciye, KMS aktivasyonunu her denediğinde DNS otomatik keşfini kullanma talimatı verir.                          
slmgr.exe -sai interval                           Etkinleştirilmemiş istemcilerin KMS bağlantısını denemesi için dakika cinsinden aralığı ayarlar. Aktivasyon aralığı 15 - 30 gün arasında olmalıdır.
slmgr.exe -sri interval                           Etkinleştirilmiş istemcilerin KMS bağlantısını denemesi için yenileme aralığını dakika cinsinden ayarlar. Yenileme aralığı arasında olmalıdır
slmgr.exe -spri                                   KMS önceliğini normal (varsayılan) olarak ayarla
slmgr.exe -cpri                                   KMS önceliğini düşük olarak ayarlayın.
slmgr.exe -sprt port                              KMS ana bilgisayarının istemci etkinleştirme isteklerini dinlediği bağlantı noktasını ayarlar. Varsayılan TCP bağlantı noktası 1688'dir.
slmgr.exe -sdns                                   KMS ana bilgisayarı tarafından DNS yayınlamayı etkinleştir (varsayılan).
slmgr.exe -cdns                                   KMS ana bilgisayarı tarafından DNS yayınlamayı devre dışı bırakın.
slmgr.exe -upk                                    Geçerli kurulu ürün anahtarını kaldırın ve lisans durumunu deneme durumuna geri döndürün.
slmgr.exe -xpr                                    Geçerli lisansın sona erme tarihini gösterin (kalıcı olarak etkinleştirilmemişse). Belirteç tabanlı aktivasyon:
slmgr.exe -lil                                    Yüklü belirteç tabanlı etkinleştirme verme lisanslarını listeleyin. 
slmgr.exe -ril ILID ILvID                         Yüklü bir belirteç tabanlı etkinleştirme verme lisansını kaldırın. 
slmgr.exe -stao                                   Otomatik KMS aktivasyonunu devre dışı bırakarak Yalnızca Belirteç Tabanlı Aktivasyon bayrağını ayarlayın.
slmgr.exe -ctao                                   Otomatik KMS aktivasyonunu etkinleştiren Yalnızca Belirteç Tabanlı Aktivasyon bayrağını (varsayılan) temizleyin.
slmgr.exe -ltc                                    Yüklü yazılımı etkinleştirebilecek geçerli belirteç tabanlı etkinleştirme sertifikalarını listeleyin
slmgr.exe -fta Certificate Thumbprint             Tanımlanan sertifikayı kullanarak belirteç tabanlı etkinleştirmeyi zorunlu kılın. 
```

### Gerçek Zamanlı Korumayı / Windows Defender / Windows Otomatik Taramalarını Devre Dışı Bırak

* Print current settings

```powershell
Get-MpPreference
```

* Copy and paste for disable all protection at once

```powershell
Set-MpPreference -DisableArchiveScanning      $true                
Set-MpPreference -DisableAutoExclusions       $true                   
Set-MpPreference -DisableBehaviorMonitoring   $true              
Set-MpPreference -DisableBlockAtFirstSeen     $true                     
Set-MpPreference -DisableRealtimeMonitoring   $true
Set-MpPreference -DisableScanningNetworkFiles $true                  
Set-MpPreference -DisableScriptScanning       $true                
Set-MpPreference -DisableArchiveScanning      $true
Set-MpPreference -ScanParameters              0
```

### WSL2'yi yükleyin ("Gentoo")

```powershell
Enable-WindowsOptionalFeature -NoRestart -Online -FeatureName Microsoft-Windows-Subsystem-Linux
Enable-WindowsOptionalFeature -NoRestart -Online -FeatureName VirtualMachinePlatform
wsl --set-default-version 2
wsl --import gentoo C:\Users\salfter\gentoo\ C:\Users\salfter\Downloads\stage3-amd64-nomultilib-20200624T214505Z.tar --version 2
```

### Kaynaklar

* https://www.reneelab.com/win10-activation-crack-free.html
* https://docs.microsoft.com/sv-se/windows-server/get-started/kmsclientkeys
* https://gist.github.com/Minionguyjpro/d913b3931e844ad8ad9a758a4aca4b63

