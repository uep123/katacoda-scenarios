# Dosya Kopyalama

>cp <"kaynak_dosya"> <"hedef_dizin">: cp komutu ile dosya ve dizin kopyalabiliriz, birden fazla dosya/dizin kopyalama imkanida vardir "cp <"kaynak_dosya"> <"kaynak_dosya"> <"hedef_dizin">" şeklinde yapabiliriz.

# Dizin Olusturma

>mkdir <"istedigimiz_dizin_ismi">: yeni bir dizin olusturmak icin kullanilan komuttur.

# Dosya Tasima

>mv <"kaynak_dosya"> <"hedef_dizin">: Komutu kullanim olarak "cp" komutu ile aynı hiyerarsik temellere sahiptir yani ayni anda birden fazla dosya tasinabilir, ekstra olarak "-i" komutu ile taşıyacagımız dosyanın hedef dizinde ayni ada sahip baska bir dosya olup olmadığını kontrol ettirebiliriz, ayni ada sahip dosya var ise bizden dosyanın üzerine yazılıp yazılmamasi için onay ister.

# Dosya ve Dizin Silme

>rm <"hedef_dosya">: Dosyaları silmek için bu komutu kullaniriz, birden fazla dosyayi ayni anda silme imkanı verir, "-f" parametresi ile dosyayi silmeye zorlayabilir "-rf" parametresi ile dizin silme işlemi yapabiliriz.

>rmdir <"hedef_dizin">: Hedef dizini silmek icin bu komut kullanılır.

# Sembolik link olusturma

>bir dosyayi farklı yerlere kopyalamak yerine bir dosyanın birden fazla yerde link olusturup depolama alnimizda tasarruf saglayabiliriz.

* ln -s /path/to/file /path/to/symlink: kullanımı bu şekildedir.