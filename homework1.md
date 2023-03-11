**1)Python'da Veri Tiplerini araştırınız, her bir veri tipi için kendi cümlelerinizle açıklamalar yazınız.**

**Text Type:** str olarak gösterilir. Tırnak içinde yazılmalıdır.
```python
x="elma"
y="56"
```

**Numeric Types:** int, float ve complex sayısal veri tipleridir. int tam sayılar, float ondalık sayılar ve complex karmaşık sayıları ifade eder.
```python
x=5    #int
y=5.6  #float
z=1+1j  #complex
```
**Sequence Types:** list[], ve tuple() bu gruba giren veri tipleridir. tuple ve list birden çok ögeyi tek bir değişkende saklama imkanı verir. list'ler mutabledır yani elemanlarını değiştirebilir, silebilir ve eleman ekleyebiliriz. Ama tuple'lar immutabledır, elemanlarını değiştiremeyiz.  
```python
xliste=[5,6,"cherry","apple"]
ytuple=(5,6,"cherry","apple")
```
**set:** list ve tuple'lar gibi birden çok ögeyi tek bir değişkende saklama imkanı verir. Ama list ve tuple'ların aksine yinelenen elemanlara izin vermez ve sıralı değillerdir. Ayrıca immutabledır.
```python
thisset={"apple","banana","cherry"}
```
**dict:** dictionarydir. Veri tiplerini key ve value şeklinde tutmamıza yarar. Böylece bir mapping işlemi yapmış oluruz. Duplicate değerlere izin vermez ve mutabledır.
```python
thisdict={"brand":"Ford","model":"Mustang","year":"1964"} 
print(thisdict) #{'brand': 'Ford', 'model': 'Mustang', 'year': '1964'}
print(type(thisdict)) #<class 'dict'>
print(thisdict["model"]) #Mustang
```
**bool:** boolean veri tipidir. True ve False olarak iki değer alır.
```python
x=True
y=False
```

**2)Kodlama.io sitesinde değişken olarak kullanıldığını düşündüğünüz verileri, veri tipleriyle birlikte örneklendiriniz.**

String: Kurslarım, Tüm Kurslar, Kariyer, Sık Sorulan Sorular, kurs başlıkları..

int: Kursları tamamlama yüzdesi

liste: Kurslarıma tıklayınca gösterilen kurslar

**3)Kodlama.io sitesinde şart blokları kullanıldığını düşündüğünüz kısımları örneklendiriniz ve Python dilinde bu örnekleri koda dökünüz.**

Tüm kurslar altında kurs bul arama çubuğunda:
```python
metin=input() #java
kurslar=["2022 Yazılım Geliştirici Yetiştirme Kampı-JAVA","2023 Yazılım Geliştirici Yetiştirme Kampı-Python&Seleniun","Yazılım Geliştirici Yetiştirme Kampı-JAVA+REACT","Yazılım Geliştirici Yetiştirme Kampı(JavaScript)"]
if(metin=="java"):
    print("2022 Yazılım Geliştirici Yetiştirme Kampı-JAVA")
    print("Yazılım Geliştirici Yetiştirme Kampı-JAVA+REACT")
else:
    print(" ")
```

Tüm kurslar altında eğitmen adına göre seçim:
```python
egitmen1="Engin Demiroğ"
egitmen2="Halit Enes Kalaycı"
girdi=input("Eğitmeni seçiniz: ")
if(girdi==egitmen1):
    print("2022 Yazılım Geliştirici Yetiştirme Kampı-JAVA")
    print("Yazılım Geliştirici Yetiştirme Kampı-JAVA+REACT")
elif(girdi==egitmen2):
    print("2023 Yazılım Geliştirici Yetiştirme Kampı-Python&Seleniun")
else:
    print(" ")
```

Siteye giriş:
```python
email="abcd@gmail.com"
password="abcd"
input1=input("mail giriniz: ")
input2=input("parola giriniz: ")
if(input1==email and input2==password):
    print("succesful")
else:
    print("Your email or password is in correct")
```
