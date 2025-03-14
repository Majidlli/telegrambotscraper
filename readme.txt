Telegram üye çekme programı Haluk tarafından yazılmıştır. 
TG: @yesildev 
Zaten bu programa doğrudan sahipseniz kendisi ile iletişiminiz vardır ve ilgili süreçlerde yardımcı olur. 
Şayet dolaylı yoldan bu programı elde ettiyseniz kendisine Telegram üzerinden ulaşabilir veya programı elde ettiğiniz kişilere sorabilirsiniz. 





		***---		KURULUM		---***		


1- Program Python temelli olduğu için python bilgisayarınızda yüklü olmalıdır. 
Python yüklemek için: https://www.python.org/ sitesine gidip Download sekmesinden Download for Windows kısmı Python 3.13.1 (31.01.2025 tarihli sürüm) indirebilirsiniz. 
İndirdiğiniz setup dosyasına çift tıklayarak çalıştırabilir ve kurulum ekranına ulaşabilirsiniz. 

### ÖNEMLİ ###
Python yükleme ekranındayken (https://docs.python.org/3/_images/win_installer.png) Add Python to Path seçeneğini seçerseniz Windows terminalinize entegresi yüklenirken yapılmış olur. 





2- Python yüklü olduğuna göre programımız için gerekli kütüphaneleri yüklememiz gerekiyor. 
Bunun için Windows başlat çubuğuna "cmd" yazarak komut istemini açalım. 
C:\Users\bilgisayarın_adı> şeklinde başlangıç olacaktır. tarafınıza iletilen dosyalar içerisinde requirements.txt dosyasının bulunduğu konuma ulaşmamız gerekecek. 
Eğer bu requirements.txt masaüstünde bulunuyorsa Komut İstemini buraya yönlendirme yapmamız gerekecek. bunun için ' cd Desktop ' yazmamız yeterli olacaktır. 
devamında komut isteminde C:\Users\bilgisayarın_adı\Desktop> yazısını göreceksiniz. 

pip install -r requirements.txt 

kodunu yazdığınız zaman gerekli olan dosyalar yüklenmeye başlayacaktır. Yükleme bitene kadar fare ve klavyeye dokunmamanızı tavsiye ederim. 
tekrar C:\Users\bilgisayarın_adı\Desktop> yazısı gelene kadar bekleyebilirsiniz. 





3- Gerekli kurulumlar yapıldıktan sonra start.exe dosyasını çalıştırabilirsiniz. 
karşınıza yeni bir terminal ve Lisans Doğrulama ekranı gelecektir. 
Tarafınıza iletilen lisans numarasını girerek doğrulaya basalım ve Arayüzümüze erişelim. 
Arayüzümüzde bizden istenilen zorunlu bilgiler şunlardır:

API ID = işlemde kullanılacak hesabın api bilgisi
HASH ID = işlemde kullanılacak hesabın hash bilgisi 
FLOOD TIME = işlem arası bekleme süresi. 10 saniye altına inmemenizle beraber 30 saniye ideal ayardır. Hesabın Telegram Flood hatasına düşmemesi için önemli bir ayar.
SOURCE_GROUP = Üyeleri çekeceğiniz grup, Grubun genel olması, üye olmanız ve üyeleri görebiliyor olmanız yeterli. başına @ koymadan grubun kullanıcı adını yazmanız yeterli ÖRNEK: https://t.me/goatdegencalls için goatdegencalls
TARGET_CHANNEL = Üyeleri ekleyeceğiniz kanal veya grubun kullanıcı adı. Grup için üye olmak yeterliyken Kanal için işlemde kullanılacak hesabın yönetici olması gerekmektedir. ÖRNEK: https://t.me/goatdegencalls için goatdegencalls

API ID ve HASH ID almak için " https://my.telegram.org " sitesini ziyaret edin. Telefon numaranız ile giriş yapmak istediğinizde Telegramın uygulama üzerinden gönderdiği kodu girin ve girişi gerçekleştirin. "API development tools" kısmına tıklayın 
"App title" kısmına herhangi bir başlık atabilirsiniz "Short Name" kısmına "app title" ile aynı olacak şekilde kısaltma yapabilirsiniz "URL" kısmına " www.telegram.org " yazabilirsiniz. "Platform" Desktop seçelim "Description" kısmına herhangi bir şey yazabilirsiniz. Create Application dediğinizde "App api_id" ve "app api_hash" kısımları sizleri karşılayacak 
"app api_id" API ID / "app api_hash" HASH ID 
videolu anlatım için: https://www.youtube.com/watch?v=8naENmP3rg4

AKTİF DEĞİL notu düşülen kısımlar boş bırakılabilir. Bir sonraki gelecek güncellemelerle aktifleşecekler. 

Bilgileri Kaydet derseniz "config.env" diye bir dosyanın oluştuğunu göreceksiniz. bu dosya ayarlarınızı kaydetmeniz ve kayıtlı ayarlarınızla işlemlere devam edebilme olanağı sağlayacaktır. 

İşleme Başla dediğinizde ise öncelikli olarak bilgilerini girdiğiniz hesaba bağlantı sağlanır. İlk kullanımda; açılan komut istemcisinde Telegram sizlerden işlemde kullanılacak hesabın telefon numarasını ister. +905555555555 formatında giriş yapacaksınız. 
Devamında Telegramın hesabınıza gönderdiği doğrulama kodunu gireceksiniz. Böylelikle hesabınız program için aktifleştirilmiş olacak. 

Aktifleşme sonrası session_(API_ID).session diye bir dosya göreceksiniz. Bu dosya sayesinde bir sonraki girişlerinizde telefon doğrulaması yapmanıza gerek kalmayacak. 

Arayüzde işlemleri sırasıyla takip edebilirsiniz. 



4- Arayüzde karşınıza gelen Log kayıtlarında "Scraper Tamamlandı" cümlesini gördükten sonra işleminiz tamamlanmış demektir. Programı kapatabilirsiniz. 



ÖNEMLİ NOTLAR 

Program çalışırken programla beraber açılan Komut İstemini kapatmayın.
Birden fazla program açabilirsiniz ancak birden fazla programla aynı kaynaktan çekme işlemi gerçekleştirmeyin. 
Flood süresine  ve Telegram kurallarına dikkat edelim böylece ban yememeye çalışalım. 
Her bir işlem için programı tekrardan başlatın. 
Gelecek Güncellemeyle programın gerçekleştirdiği bir işlem için birden fazla hesap kullanılabilir olacak.


Sorularınız ve takıldığınız yerler için bana ulaşabilirsiniz. Zaten bu programa sahipseniz bana nasıl ulaşabileceğinizi biliyorsunuz. eğer bilmiyorsanız TG: @yesildev 



 

