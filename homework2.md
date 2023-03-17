***Ödev Tanımı:***
Bir öğrenci kayıt sistemi yazdığımızı düşünelim. Sistemimizdeki öğrencileri bir listede sadece ad soyad olacak şekilde tutalım.
Bu öğrenci kayıt sistemine;
- Aldığı isim soy isim ile listeye öğrenci ekleyen
- Aldığı isim soy isim ile eşleşen değeri listeden kaldıran
- Listeye birden fazla öğrenci eklemeyi mümkün kılan
- Listedeki tüm öğrencileri tek tek ekrana yazdıran
- Öğrencinin listedeki index numarası öğrenci numarası olarak kabul edildiğini düşünerek öğrencinin numarasını öğrenmeyi mümkün kılan
- Listeden birden fazla öğrenci silmeyi mümkün kılan (döngü kullanınız)
fonksiyonları geliştiriniz ve her bir fonksiyonu en az bir kere çağırarak konsolda test ediniz.

Ödevde kullanacağınız döngülerin bir tanesi for bir tanesi while döngüsü olması istenmektedir.


```python
students=["X Kişisi", "Y Kişisi", "Z Kişisi"]
def addStudent(name,surname):
    student=name+" "+surname
    students=students.append(student)
```

```python       
def removeStudent(nameAndSurname):
    for student in students:
        if(student==nameAndSurname):
            students=students.remove(nameAndSurname)
```

```python
def addStudents():
    while True:
        newStudent=input("Eklemek istediğiniz öğrenciyi giriniz ya da çıkmak için q'ya basınız: ")
        if(newStudent=="q"):
            break
        else:
            students.append(newStudent)
```

```python
def showAllStudent():
    for i in students:
        print(i)
```

```python
def findSudentNo(nameAndSurname):
    for i in range(len(students)):
        if (students[i]==nameAndSurname):
            print(i)
```

```python
def removeStudents(namesAndSurnames):
    x=namesAndSurnames.split(",")
    y=[]
    for i in x:
        y.append(i.strip())
    for i in y:
        for j in students:
            if(i==j):
                students.remove(j)
```        
                 
```python    
addStudent(input("isim giriniz: "),input("soy isim giriniz: "))
removeStudent(input("Silmek istediğiniz isim ve Soyismi Giriniz: "))
addStudents()
print(students)
showAllStudent()
findSudentNo(input("Numarasını öğrenmek istediğiniz öğrencini adı ve soyadını giriniz: "))
removeStudents(input("Silmek istediğiniz öğrencilerin isim ve soyisimlerini arasına virgül koyarak Giriniz: "))
print(students)
```



