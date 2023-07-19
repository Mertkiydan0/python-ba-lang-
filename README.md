# python-baslangıc

pythonda üslü sayıları ifade etmek için "**" işareti kullanılır 
örnek : 2**3 : 8 gibi.

kalan bulmak için kullandığımız ifade "%" kullanılır
örnek : 11%2 : 1

##DEĞİŞKENLER :

integer : tam sayılardır.

float: ondalıklı sayılar.

string: harfleri belirtmek için kullanılır tanımlarken "" tırnak işareti ile kullanmamız gerekir.
değişkenlerin değer tanımlamalarını değiştirirken diğer dillere nazaran integer veya string atamlarını otomatik olarak python kendi içinde yapabilir.
belirtilen değişkenin uzunluğunu elde etmek için length(len) ifadesini kullanırız. !! string değerleri için değişkenin içerisindeki boşluk karakterini de dahil etmektedir.

yazacağımız çıktının belirtilen bir kısmını alt satırda görmek istiyorsak "\n" ifadesini kullanırız.
örnek : print("mert \nkiydan")

yazacağımız çıktının belirtilen bir kısmına tab kadar boşluk atmak istiyorsan "\t" ifadesini kullanırız.
örnek : print("mert \tkiydan")

yazacağımız çıktının ilk elemanını görmek için"[]" ifadesini kullanırız.
örnek : my_string = "mert kiydan"
        my_string[0] ifadesini yazdırdığımızda bize : "m"ifadesini verecektir.
çünkü bilgisayar dilinde sayılar 0dan başladığı için ilk terim olarak 0 değerini alacaktır.

yazacağımız çıktının son harfini elde etmek için de "[-1]" ifadesini kullanabiliriz.

yazacağımız çıktının elemanlarını sondan çıkartmak için de son eleman sayısının başına "-" getirerek istediğimiz sayılı elemanı elde edebiliriz.

##SLICING: 

 girdiğimiz değişkenin belirlediğimiz sıradaki elemanını çağırmak için kullanılır, "[]" ifadesi ile kullanılır. Başlangıç eleman olarak "[0]" değeri kullanılır.

 değişkenin en son harfini öğrenmek için "[-1]" ifadesini kullanırız, sondan başlayarak herhangi bir değer öğrenmek istediğimizde istediğimiz değerin sırasının başına"-" ifadesi getirmemiz yeterlidir.

 değişkenimizin istediğimiz sıralamadan sonraki değerlerini almak için "[:]" ifadesi kullanılır.
örnek vermek gerekirse:

  my_string2 = "1234567890"
  my_string2[0] 
çıktısı : "1"
  my_string2[2:]
çıktısı : "34567890"

buradaki "[2:] ifadesinde "2" değeri 2. eleman yani 3. değeri ile ondan sonraki değerleri göster anlamına gelmektedir.

  my_string2[:2],
çıktısı : "12"

buradaki "[:2]" ifadesinde ise "2" değeri 2. elemana kadar yani 3.değerden önceki değerleri göster anlamına gelmektedir.

":" işaretinin sol tarafındaki değerde verilen ifadedeki değeri dahil edip sağ tarafında dahil etmemesinin sebebi sıralama sırasında bir kesişim olmaması içindir. İki taraftan da dahil edilseydi ortak istenilen bir değerde kesişim olabilirdi.

#3STEP SIZE

"[::] ifadesi ile kullanılır. Adım boyutunu verir yani kaç adet eleman atlayacağını belirtiriz.

örnek: my_string2[::3] 
çıktısı : '1470' olur.

eğer diğer parametreleri de girersek istediğimiz sıralamalar arasındaki değerleri istediğimiz sayıda atlatarak ekrana yazdırabiliriz.

örnek: my_string2[1:6:2]
çıktısı :'246'
olacaktır.

eğer verilen tüm çıktıyı tam tersi yazdırmak istiyorsak da "[::-1]" ifadesini kullanabilriz.

örnek : my_string2[::-1]
çıktısı : '0987654321'
olacaktır.

#STRING METHODS

girdiğimiz string değerleri için bazı metotlar kullanabiliriz, bunlardan bazıları;

.capitalize() : değişken değerimizin ilk karakterini büyük yazdırmayı sağlar.
.split() : değişken değerimizin kelimelerini ayrı ayrı çıktı vermesini sağlar.
.upper() : değişken değerimizin her harfini büyütmeye yarar.

#LİSTELER

listeleri toplayabiliriz, çarpabiliriz.

oluşturduğumuz listeye eleman eklemek için 

"my_list.append("ekleyeceğimiz eleman")" ifadesini kullanabiliriz.

listemizdeki son elemanı öğrenip silmek için 

"my_list.pop()" ifadesini kullanabilriz bu hem listemizin son değerini gösterir hem de son değeri silmemize yarar.

listemizdeki elemanların sırasını değiştirmek için de "my_list.reverse()" ifadesini kullabiliriz.

#İÇ İÇE GEÇMİŞ LİSTELER

bir listenin içerisine farklı bir liste daha oluşturabiliriz.

oluşturduğumuz listedeki elemanı öğrenmek için de içine koyduğumuz listenin ana listemizin kaçıncı elemanı olduğunu bilmemiz gerekir daha sonrasında ise yanına bir parametre daha girerek listemizin içindeki listeden dilediğimiz elemanı öğrenebiliriz.

örnek : my_list = [1,2,3,["5,6,7]]
        my_list[3][2]
  çıktısı : 7 olacaktır.

#SÖZLÜKLER

sözlükler hemen hemen listelere benzerler fakat bir sözlük açmak için "my_dictionary = {}" ifadesi ile süslü parantez kullanarak açarız.

bir anahtar değer ile bir değeri birleştireceksek bunun için sözlük "dictionary" kullanabiliriz.

sözlükler bir anahtar değerden bir de değerden oluşurlar. 
örnek : my_dictionary = {"anahtar","değer"}

oluşturduğumuz sözlükler için anahtar kısmının illa string bir değer veya değer kısmının integer bir değer almasına gerek yoktur, tıpkı listelerde olduğu gibi iki kısım da istediği değerleri alabilir.

açtığımız sözlükteki anahtar kelimleleri almak için : "my_disctionary.keys()" ifadesini kullanabiliriz.

açtığımız sözlükteki değerlerini almak için : "my_disctionary.values()" ifadesini kullanabiliriz.

açtığımız sözlükteki anahtar kelimeye karşılık girdiğimiz değerleri değiştirebiliriz.
örneğin :
my_dictionary_5 = {"k1":1,"k2":2}
my_dictionary_5["k1"] = 5

çıktısı : {'k1': 5, 'k2': 2} olacaktır.

oluşturduğumuz sözlüğe yeni bir değer de ekleyebiliriz.

örneğin: my_dictionary_5["k3"]= 7 

çıktısı : {'k1': 5, 'k2': 2, 'k3': 7} olacaktır.

oluşturduğumuz sözlükten değerleri de silebiliriz.

bunun için pop fonksiyonunu kullanırız 

örneğin: "my_dictionary_5.pop("k3")" ifadesini kullandığımızda "k3" anahtar kelimesini değeriyle birlikte silecektir.

çıktısı : {'k1': 5, 'k2': 2}
olacaktır.

#SETLER

setler de listeler ile hemen hemen aynıdır fakat listeler belirli değerleri tekrar tekrar yazabilirken sette her bir değer sadece bir defa yazılabilir.

setler direkt olarak oluşturuluken my_set{} şeklinde oluşturulursa eğer python oluşturduğumuz seti sözlük olarak alıp dictionary sanacaktır. 
bunu önlemek için de my_set = set() şeklinde boş bir set tanımlayabiliriz. Bu yöntemi ayrıca diğer veri yapıları için de kullanabiliriz.

#TUPLE
verilen değişmesini istediğimiz örnekler için tuple kullanabiliriz.

kullanımı çok yaygın değildir açık kaynak kodlu uygulamalarda genellikle kullanılır.

tuple içindeki bir değerin kaç adet olduğunu öğrenmek için "my_tuple.count("öğrenmek istediğimiz değişken adı")"  kullanabiliriz.

tuple içindeki bir değerin kaçıncı sırada olduğunu öğrenmek için "my_tuple.index("öğrenmek istediğimiz değişken adı")" kullanabiliriz.

#BOOLEAN

basit bir evet hayır veri yapısıdır.

"True" ve "False" olarak kullanılır. Küçük yazılan "true" veya "false" kabul görülmez.
 
 if else gibi sorgulamaya dayalı kontrollerde kullanılır.

 matematiksel sorgulama işlemlerinde de kullanılır.
 
#AND OR NOT KAVRAMI

ve veya kavramı olarak da değerlendirilebilir.

değerlerin doğruluğu için "and" kavramında iki değerinde de doğru olması gerekliyken "or"kavramı için sadece tek bir değerin doğru olması yeterlidir.

  
çıktı almak için "print" ifadesini kullanırız.



Değer almak için "input" ifadesini kullanırız.
örnek: r = input("r : ").
!!! inputa atılan default değer string cinsinde olacağı için değerini verdikten sonra türünü belirlemeyi unutmayalım.



