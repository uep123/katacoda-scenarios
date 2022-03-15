
# Dosya ve Dizin izinlerini ogrenme

> ls -l: bu komut ile bulundugumuz dizindeki dosyaların izinlerini öğrenebiliriz.

> stat -c "%a %n" *: bu komut ile de mevcut dizindeki dosyaların izinlerini öğrenebiliriz.

* r-: okuma yetkisi (read)
* w-: yazma yetkisi (write)
* x-: calistirma yetkisi (execute)

>Dizinde listeme yaptığımızda bir sey gozunuze carpmis olabilir, bazilari "-r" ile baslarken bazilari "r" diye basliyor bunun sebebi "-r" başlayanların dosya "r" ile başlayanların dizin olmasıdır.

* 4 : okuma yetkisi (read)
* 2: yazma yetkisi (write)
* 1: calistirma yetkisi (execute)

>ilk rakam dosyanın sahibinin izinlerini, ikinci rakam dosyanın sahibiyle aynı grupta bulunan kullanıcılarının yetkilerini, üçüncü rakam diger kullanicilarin yetkilerini ifade eder

# Dosya ve Dizin izin verme

* u: dosya sahibini
* g: dosya sahibinin grubunu
* o: diger kullanıcılari
* a: tum haklari
* +: yetki ekleme
* =: yetki eşitleme
* -: yetki cikarma
* r: okuma yetkisi
* w: yazma yetkisi
* x: calistirma yetkisi

>chmod o+r <"dosya">: Diger kullanicalara yazma yetkisi veya chmod o=r <"dosya"> şeklinde kullanılabilir

>chmod ugo+rw <"dosya">: Dosya sahibine, dosya sahibinin grubuna ve diger kullanicalara yazma ve okuma izni verir

>chmod 644 <"dosya">: Dosya sahibi 4+2=6 okuma yazma izni, dosya sahibi ile aynı grup 4=4 sadece okuma izini verir, diger kullanicilar 4=4 sadece okuma izni verir

>chmod 755 <"dosya">: Dosya sahibi 4+2+1=7 okuma,yazma ve calistirma izni, dosya sahibi ile aynı grup 4+1 sadece okuma, calistirma izini verir, diger kullanicilar 4+1 okuma, calistirma izni verir

# Dosya ve Dizin sahibini degistirmek

* chown <"kullanici"> <"dosya_dizin">: Dosya sahibini degistirmek icin
* chown -R <"kullanici"> <"dosya_dizin">: Degisligi tum dizin ve dosyalarda yapmak icin "-R" parametresi kullanilir
* chown -R <"kullanici">:<"grup"> <"dosya_dizin">: Dosya sahibini ve grubunu degistirmek icin kullanilir
* chgrp <"grup"> <"dosya_dizin">: dosya grubunu degistirmek icin kullanilir