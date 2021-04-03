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
25
Bu kullanım çok mantıklı olmayabilir. İleri ki yazılarda kullanıcı ile etkileşime geçildiği zaman bu dönüşümlerin ne kadar önemli olduğundan bahsedeceğiz.







