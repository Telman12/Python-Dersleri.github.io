# Python Başlanğıc


Herkese selamlar! ilk öncelikle siz burda yazdıklarımı full okudukdan ve uyguladıkdan sonra python'un temelini örnemiş olucaksınız. Belki irelide beyenilirse devamı gelicek full öğreticem neyse
hadi başlayalım.


# Python Nasıl Kurulur


ilk öncelikle https://www.python.org/ bu siteye girelim. Sonra Python yazısının altında downloads yada indirilenler yazıcakdır. mouse ile üzerine gelin ve sizin bilgisayarınız
hangisiyse onu secip indirin. Ve kurulumunu yapın. Bunları yaptıkdan sonra cmd yi acın ve py yada python yazın eyer help fln yazarsa ve echo >>> böyle olursa çalışıyor demekdir.

# NOT: dosyayi calistirmak icin dosyanin dizinine gelip python dosya adi ni yazmaniz yeterli mesela python deneme.py gibi


# Print Komutu ve Kaçış Dizileri


Print Komutu

Print komutu adından da anlaşılacağı gibi ekrana yazı yazdırılmasını sağlar. Şimdi print komutu kullanılarak ekrana birkaç yazı yazdıralım.

print'in yazılış tarzları

print("""deneme""")
print("deneme")
print('deneme')
print('''deneme''')

şimdi yazdıklarımızı deneyip gelin.

Kaçış Dizileri

İlk kaçış dizi olan "\" işaretinden yukarıda verilen örnekler üzerinden açıklık getirilebilir.

kaçış dizi örnekleri

print('Python-Dersleri\'in amacı herkese Python öğretmektir.')
print("Özgür yazılım için \
... bir araya toplandık.")
print("Bilgisayar Mühendisliği\nElektrik Mühendisliği")

şimdi yazdıklarımızı tekrardan deneyip gelin.


# DEĞIŞKENLER



Bir veriyi içerisinde depolayan birime değişken denir. Değişkeni bir kutuya benzetebilirsiniz.Siz ona bir değer verirsiniz. O da verdiğiniz değeri sizin için saklar. Değişken isimleri sayı ile başlayamaz ve program içinde bulunan herhangi bir komut değişken ismi olarak atanamaz.



Eğer herhangi bir programlama dili ile ilgilendiyseniz değişkenler ile bol bol uğraşmış olmanız gerekir. Diğer programlama dillerinde(C,C++,C#) bir değişken tanımlanırken değişkenin adı yazılmadan önce türü yazılır.


int tamSayi=10;
char karakter = 'a';
cumle = "Bu bir cümledir."
float ondalikSayi = 2.5

Python programlama dilinde bu kural geçerli değildir. Değişken tanımlarken adını ve değerini yazmak yeterlidir.Eğer Python gibi yorumlayıcı web programlama dili olan PHP ile ilgilendiyseniz bu tanımla yolu size çok tanıdık gelecektir. Yukarı da verilen değişkenleri Python'da tanımlayalım.

tamSayi = 10 #integer
karakter = 'a' #char
cumle = "Bu bir cümledir." #string
ondalikSayi = 2.5 #float

ad="Telman"
soyad="Allahverdiyev"
adSoyad = ad + soyad
print(adSoyad)

>>>TelmanAllahverdiyev

sayi=3.6
bol=sayi/2
print(bol)

>>>1.8


# Dönüştürme İşlemleri


Bazı durumlarda değişkenler üzerinde tür dönüşümü yapmak zorunda kalabilirsiniz. Program yazdıkça farkına varacaksınız ki; En çok dönüştürme işlemi 'string' ve 'integer' ifadeler arasında yapılmaktadır. Tür Dönüşümü İçin Kullanılan Fonksiyonlar:

Float() => Herhangi bir sayı veya sayı değerli karakter dizisini noktalı sayıya çevirir.
int() => Herhangi bir sayıyı veya sayı değerli karakter dizisini tam sayıya dönüştürür.
str() => Herhangi bir sayıyı karakter dizisine dönüştürür.

Birkac örnek:

a = 2
print float(a)

>>>2.0

a=10
b="15"
print(a+b)
>>>Traceback (most recent call last):
  File "deneme.py", line 3, in <module>
    print(a+b)
TypeError: unsupported operand type(s) for +: 'int' and 'str'
  
Bu şekilde bir kullanım yapılırsa görüldüğü gibi Python integer ve string türünü toplayamadığı için hata döndürdü.Bu yüzden bunu şu şekilde yapabiliriz.

a=10
b="15"
print(a+int(b))

>>>25

Bu kullanım çok mantıklı olmayabilir. İleri ki yazılarda kullanıcı ile etkileşime geçildiği zaman bu dönüşümlerin ne kadar önemli olduğundan bahsedeceğiz.

# Kullanıcıdan Veri Almak

Bugüne kadar yaptığımız bütün örneklerde her zaman tek taraflı işlemler yaptık.Yani kullanıcı programa hiç müdahalede bulunamadı. Bu yazımızda kullanıcının Python ile nasıl etkileşime geçeceğinden bahsedeceğiz.
Python da kullanıcı ile etkileşime geçebilmek için input() fonksiyonu kullanılır. Şimdi bu fonksiyonları ve aralarındaki temel farkları inceleyelim.

input() Fonksiyonu
input() fonksiyonu klavye aracılığı ile kullanıcıdan veri alınmasını sağlar. Daha iyi anlayabilmeniz için basit bir örnek ile açıklayalım.
 
ad = input("Lütfen adınızı giriniz:")
print(ad)

Yukarıdaki programda ilk satırdaki kodun ne işe yaradığından ve kaydedilen bir Python dosyasının çalıştırılmasından yazının başında bahsetmiştik. Gelelim şuan bizi ilgilendiren kodlara; Gördüğünüz gibi input() fonksiyonu içinde "Lütfen adınızı giriniz:" açıklaması yapılarak programın kullanıcıdan ne beklediği belirtilmiştir. Bu açıklamayı yapmak zorunda değilsiniz. Ama kullanıcının programın kendisinden ne beklediğini anlayabilmesi için yazmanız daha faydalı olacaktır. Burada input() fonksiyonunun anlaşılabilmesi için basit bir örnek yapılmıştır.Şimdi ise kullanıcının girdiği iki sayıyı topladıktan sonra ekrana yazdıran programı yazmaya çalışalım.



print("İki Sayıyı Toplayan Program")
sayi1 = input("Birinci Sayıyı Giriniz:")
sayi2 = input("İkinci Sayıyı Giriniz:");
 
toplam = sayi1+sayi2
print(toplam)

Bu programı çalıştırdıktan sonra 10 ve 15 değerlerini girerseniz şu şekilde bir çıktı ile karşılaşacaksınız.

İki Sayıyı Toplayan Program
Birinci Sayıyı Giriniz:10
İkinci Sayıyı Giriniz:15
1015

Gördüğünüz gibi biz programın iki sayıyı toplamasını isterken;program iki sayıyı yan yana ekleyerek ekrana yazdı. Buradan da anlayacağınız gibi raw_input() kullanıcı tarafından girilen bütün değerleri karakter dizisi olarak alır. Yani Python için girilen iki değer sayı değildir.Bu yüzden de iki karakter dizisini uç uca eklemiş oldu. Programın kod yapısını şu şekilde değiştirelim.

print("İki Sayıyı Toplayan Program")
sayi1 = input("Birinci Sayıyı Giriniz:")
sayi2 = input("İkinci Sayıyı Giriniz:");
 
toplam = int(sayi1)+int(sayi2)
print(toplam)

Aynı değerleri bu program için girdiğinizde aşağıdaki gibi bir sonuçla karşılaşacaksınız.

İki Sayıyı Toplayan Program
Birinci Sayıyı Giriniz:10
İkinci Sayıyı Giriniz:15

>>>25

Peki neden bu şekilde oldu? Eğer bu sorunun cevabı hakkında pek bir fikriniz yoksa;Değişkenler başlıklı yazıyı okumalısınız. Burada programın elinde bulunan karakter dizilerini sayıya çevirmesi için int() fonksiyonundan yararlandık.



