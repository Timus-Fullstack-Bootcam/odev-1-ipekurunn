## Ödev - Hafta 1-2
### **2. Java ile JavaScript arasındaki fark nedir?**
Java ve JavaScript, farklı kullanım alanları ve özelliklere sahip iki farklı programlama dilidir. Java genellikle büyük uygulamalar için tercih edilirken, JavaScript web geliştirme ve tarayıcı tabanlı uygulamalar için kullanılır.

•	Java, sunucu tarafı ve büyük ölçekli uygulamalar için kullanılırken, JavaScript tarayıcı tarafı ve web geliştirmeye odaklıdır.

•	Java, derlenip platforma özgü bir şekilde çalıştırılması gereken bir dildir. JavaScript ise tarayıcılarda doğrudan çalışır.

•	Java daha katı kurallara ve karmaşıklığa sahiptir, JavaScript ise daha esnek ve hızlı prototipleme sağlar.

•	Java genellikle büyük projeler ve sunucu tarafı uygulamalar için tercih edilirken, JavaScript web sayfalarına etkileşim eklemek ve tarayıcı tabanlı uygulamalar geliştirmek için kullanılır.
### **3. JavaScript'teki veri tipleri nelerdir açıklayınız.**
JavaScript'te 2 farklı veri tipi vardır.

1- Primitive (ilkel) Veri Tipleri:

• String, Number, Boolean, Undefined, Null, Symbol.

2- Complex (Karmaşık) Veri Tipleri:

• Obje, Array, Fonksiyon.
### **4. null ve undefined arasındaki fark nedir açıklayınız.**
Null ve Undefined bir değişkenin değerinin tanımsız olduğunu gösteren değerlerdir. 

**-Undefined:** Bir değişken tanımlanmış ancak değeri atanmadığını ifade eder. 

**-Null:** Bir değişkenin bilinçli olarak boşaltıldığını veya atanmadığını ifade eder. Yani değişkenin değeri olmadığına ve özellikle boş olduğunu söyler.
### **5. NaN nedir açıklayınız.**
NaN, "Not-a-Number"ın kısaltmasıdır ve JavaScript'te özel bir değerdir. Bu değer, matematiksel bir işlemin sonucunun sayısal bir değere dönüşmediği veya tanımlanamadığı durumları temsil eder. NaN, genellikle hatalı veya geçersiz sayısal işlemler sonucunda ortaya çıkar.
### **6. Javascript’te yorum satırı eklemenin kaç farklı yolu vardır?**
JavaScript’te yorum satırı eklemenin 2 farklı yolu vardır.
`//` tek satırlı yorumlar ya da bir kod satırının bir kısmına veya kodun tamamına yorum yapmak için kullanılır.
```javascript 
//Tek satır yorum örneği.
```
Birden çok satırlı yorumlar ise `/*` ile başlayıp `*/` ile biter. 
```javascript 
/* Birden
çok
satırlı
yorum
öğreniği. */
```
### **7. Global değişken ne demektir?**
Global değişkenler programın herhangi bir yerinden erişilebilen değişkenlerdir. Değişkenleri global olarak bildirmek için ise `Var` değişken tanımlama ifadesi kullanılır. Ek olarak, bir değişkene değer atayıp değişkenin tanımlama ifadesini bildirmezsek otomatik olarak global değişken olarak kabul edilir.
### **8. Javascript’te this anahtar kelimesi nedir açıklayınız.**
JavaScript'te `this` anahtar kelimesi ait olduğu nesneyi ifade eder ve nerede kullanıldığına bağlı olarak farklı değerler alabilir;

• Eğer bir metot içerisinde kullanılıyorsa ait olduğu nesneyi temsil eder.

• Tek başına kullanılıyorsa global bir nesneyi temsil eder.

• Bir fonksiyon içerisinde kullanılıyorsa global bir nesneyi ifade eder.
### **9. == ile === farkını örnekler ile açıklayınız.**
`==` operatörü karşılaştırılan değerlerin eşit olup olmadığını kontrol eder, ancak türlerini dikkate almaz. Yani karşılaştırılan değerler farklı türlerden olsalar bile değerleri aynıysa `true` olarak döner. 

    "5" == 5; // true, çünkü değerler eşittir. (Türlerini dikkate almıyoruz.)
`===` operatörü karşılaştırılan değerlerin hem değer hem de tür açısından eşit olup olmadığını kontrol eder.

    "5" == 5; // false, çünkü değerler eşit ancak türleri farklı.

`NOT:` === operatöründe eğer hem değerleri hem türleri eşitse ancak referans noktaları farklıysa yine `false` döner!
### **10. let var const farkını tablo yapınız.**

| let     | var | const |
|----------|--------|-------|
| Function Scope'tur. Tanımlandığı fonksiyon aralığının dışında erişilmez.     | Global Scope'tur. Her yerden erişilebilir.      | Function Scope'tur Tanımlandığı fonksiyon aralığının dışında erişilmez.    |
| Üst üste değişken tanımlanamaz.      | Üst üste değişken tanımlanabilir.      | Üst üste değişken tanımlanamaz.  |
| Değiştirilebilir. | Değiştirilebilir.      | Değiştirilemez.    |

### **11. Arrow fonksiyonun normal fonksiyondan farkları nelerdir?**
Temel farkları, arrow fonksiyonlarının daha kısa ve hızlı söz dizimi kullanmalarıdır. Aynı zamanda `this` bağlamını da farklı işlerler. Arrow fonksiyonları kendi `this` bağlamını oluşturmaz ve genelde fonksiyonun dışındaki `this`'i miras alırlar.
### **12. switch bloğu içinde hatasız nasıl değişken tanımlanır?**
JavaSript'te `switch` bloğu içerisinde değişken tanımlamak için `case` ifadeleri içinde `let` veya `const` kullanılır. Ancak, `switch` bloğu içinde tanımlanan değişken, sadece ilgili `case` bloğu içinde geçerlidir ve diğer `case` bloklarından erişilemez.

`NOT:` Eğer iki farklı `case` içerisinde aynı isimde değişken tanımlandıysa hata verir. Farklı case'lerde de olsa aynı isimde değişken tanımlanamaz.
### **13. Pure fonksiyon ne demektir açıklayınız.**
Pure fonksiyonları, aynı parametre değerleri ile çağırıldığında aynı çıktıyı üreten ve dışarıda herhangi bir değişiklk yapmaytan yan etkisiz fonksiyonlardır. 

Pure fonksiyonları her çağrıda aynı çıktıyı ürettikleri için beklenmeye durumlar daha az olur bu yüzden kod güvenliği için kullanılabilir. Ayrıca Önbellek optimizasyonu için de kullanılır. Çünkü aynı girdilerle tekrar tekrar çaprıldıklarında aynı çıktıyı üretirler, bu da önbellek performansını artırabilir.

Matematiksel işlemler ve tarih ve saat işlemlerinde pure fonksiyonlar kullanılır.

### **14. Rest operatör nedir örnekle açıklayınız.**
Rest operatörü (...) değişken sayıda argümanları veya özellikleri bir araya getirmek için kullanılır ve genellikle bir fonksiyonun parametreleri ya da bir nesnenin özellikleri üzerinde kullanılır.

**-Fonksiyon Parametreleri içinde Rest Operatörü:**
```javascript
function collection (...numbers) {
  let sum = 0;
  for (let number of numbers) {
    sum += number;
  }
  return sum;
}

console.log(collection(2, 5, 8, 10)); // 25
```
**-Nesne özellikleri içinde Rest Operatörü:**
```javascript
const {name, age, ...rest} = {name: 'Nora', age: 30, city: 'NY', job: 'Software Engineer'};

console.log(name); //Nora
console.log(age); //30
console.log(rest); //{city; 'NY', job: 'Software Engineer'}
```

### **15. Object destructuring nedir örnekle açıklayınız.**
Object destructuring, bir nesnenin içindeki özelliklere kolayca erişmeyi sağlayan bir JavaScript özelliğidir.
```javascript
//Kullanıcı nesnesi:
const use = {
  id: 1,
  username: 'Nora',
  address: {
    city: 'NY',
    country: 'USA'
  }
};

// Object destructuring kullanarak belirli özellere erişmek:
const {id, username, address: {city}} = user;

console.log(id); // 1
console.log(username); //Nora
console.log(city); // NY
```
Yukarıdaki örnekte `user` adlı nesnenin içindeki belirli özelliklere destructuring kullanarak erişiyoruz.

`const {id, username, address: {city}} = user;` satırıyla `id` ve `username` gibi direkt özelliklere, `address` özelliğinin içindeki `city` özelliğine de erişmiş oluyoruz.

Yani özellikle karmaşık nesne yapılarından sadece ihtiyacımız olan verilere kolayca erişmemizi sağlıyor.

### **16. 2 elemanlı bir objeyi 6 farklı şekilde oluşturunuz.**
1. Nesne söz dizimi ile oluşturma:
```javascript
const users = {name: 'Nora', age: 30};
```
2. new Object() ile oluşturma:
```javascript
const users = new Object();
users.name = 'Nora';
users.age = 30;
```
3. Object.create() ile oluşturma:
```javascript
const users = Object.create();
users.name = 'Nora';
users.age = 30;
```
4. Destructing ile oluşturma:
```javascript
const {name, age} = {name:'Nora', age:30}
const users = {name,age} 
```
5. Fonksiyon ile oluşturma:
```javascript
const {name, age} = {name:'Nora', age:30}
const users = {name,age} 
```
6. JSON stringi ile oluşturma:
```javascript
const {name, age} = {name:'John', age:30}
const users = {name,age} 
```
### **17. 2 elemanlı bir objenin key ve value değerlerinin karakter sayısı ile 2 farklı döngü methodu kullanarak yeni bir obje oluşturunuz.**
```javascript
const originalObject = {name: 'Nora', age: 30];

//Method 1 - for..in döngüsü kullanarak:
const newObj1 = {};
for (let key in originalObject) {
  newObj1[key] = originalObject[key].length;
}

console.log(newObj1); //{name: 4, age: 2}

//Method 2 - while döngüsü kullanarak:
const newObj2 = {};
const = originalKeys = Object.keys(originalObject);
let index = 0;

while (index < originalKeys.length) {
  const newKey = originalKeys[index];
  newObj2[newKey] = originalObject[newKey].length;
  index++;
}

console.log(newObj2); //{name: 4, age: 2}
```
Method 1'de `for...in` döngüsünü `originalObject`'in içindeki key'e erişmek için kullandık. Key'e erişip her birinin uzunluğunu `length` ile alarak `newObj1` adlı yeni bir obje oluşturduk.

Method 2'de ise `while` döngüsünü `Object.keys(originalObject)` ile `originalObject`'in key'lerine ulaşmak için kullandık. Bu key'leri alarak `newObj2` adlı yeni bir obje oluşturduk.

Yani her iki yöntem de `originalObject`'in içindeki keylerin uzunlarını alarak bir obje oluşturuyor ve sonuç olarak `{name:4, age:2}` elde etmiş oluyoruz.

### **18. Cookie, local storage ve session storage farkını tablo yapınız.**

| Cookie     | Local Storage | Session Storage |
|----------|--------|-------|
| Depolama kapasitesi 4KB    | Depolama kapasitesi 10MB      | Depolama kapasitesi 5MB    |
| Oturum kimleri gibi uzun süre saklanmaması gereken verileri depolamak için kullanılır | Çevrimdışı veriler gibi kullanıcının daha sonra erişmesi gereken verileri depolamak için kullanılır.      | Web uygulamalarının performansını artırmak için kullanılır.    |
| Verilerin süresi belirli bir zamanda dolacak şekilde ayarlanabilir.     | Saklanan veriler tarayıcı kapatıldığında silinmez.    | Veriler yalnızca oturum için saklanır ve tarayıcı kapatıldığında silinir.  |
| Veriler istemciden sunucuya istekle birlikte gönderilir.    | Veriler istemciden sunucuya istekle birlikte gönderilmez.   | Veriler istemciden sunucuya istekle birlikte gönderilmez. |
| Veriler yalnızca tarayıcıda saklanır   | Veriler tarayıcıda ve sistemde saklanır.   | Veriler yalnızca tarayıcıda saklanır. |

### **19. asenkron ve senkron işlem farkı nedir?**
**Senkron:** İşlerin sırasıyla yapıldığı ve işlerin her birinin birbirini beklediği durumdur.

**Asenkron:** Yine işlerin sırasıyla yapıldığı ama birbirini beklemedği durumdur. (JavaScript'te asenkron yapıdadır.)
### **20. promise nedir ve neden ihtiyaç duyarız?**

Promise, JavaScript'teki asenkron programlamada kullanılan bir yapıdır. Olumlu durumlarda resolve ile belirtilen işlemleri, olumsuz durumlarda ise reject ile belirtilen işlemlerin yapılacağına dair güvence (söz) verir.

Pending, Resolve ve Reject olmak üzere 3 adet parametre alır. 

Asenkron programlamada, bir işlem tamamlanana kadar beklenmez ve program diğer işlemlere devam eder. Promise, bu tür asenkron işlemleri daha düzenli ve okunabilir bir şekilde ele almamıza olanak tanır.

Ek olarak, Callback Hell durumundaki karmaşıklığı azaltarak kodun daha okunabilir olmasını sağlar.

## Array Soruları 1
`var dolap = ["Shirt", "Pant", "Tshirt"];`
#### **1- dolap arrayindeki son elemanı silip consola yazdırın.**
```javascript
var deletedElement = dolap.pop();

console.log("Deleted Element: ", deletedElement);
```
#### **2- dolap arrayindeki ilk elamanı silip yerine “Hat” elemanını gönderip consola yazdırın.**
```javascript
dolap.splice(0, 1, "Hat");

console.log("Current Dolap: ", dolap);
```
#### **3- dolap değişkeninin array olup olmadığını kontrol edin ve sonucu bir değişkeneeşitleyin**
```javascript
var isDolapArray = Array.isArray(dolap);

console.log("Is Dolap Array?: ", isDolapArray);
```
#### **4- dolap arrayinde “Pant” elemanın olup olmadığını 3 farklı method ile kontrol edin**
```javascript
// includes() kullanarak:
var isTherePant = dolap.includes("Pant");

console.log("Pant" var mı?: ", isTherePant);

// find() kullanarak:
var isTherePant = dolap.find(item => === "Pant" !== undefined;

console.log("Pant var mı?: ", isTherePant);

// indexOf() kullanarak:
var indexOfPant = dolap.indexOf("Pant");

console.log("Pant var mı?: ", isTherePant);
```

#### **5- dolap arrayindeki elemanların karakter sayısını toplayıp geriye döndürecekfonksiyonu yazın.**

#### **6- dolap arrayindeki tüm elemanları büyük harfe çevirip yeni bir değişkene 3 farklı yöntemle atayın.**

#### **7- dolap arrayini index sayıları key olacak şekilde objeye çeviriniz.**

#### **8- slice ile splice farkı nedir?**
`slice()` metodu bir dizinin belirli bir bölümünü seçerek kopyalar ve bu kopyayı yeni bir dizi olarak döndürür.

`splice()` metodu ise bir dizinin belirli bir bölümünü çıkarır veya yeni elemanlar ekler.

`NOT:` slice orijinal diziyi değiştirmez, sadece bir kısmını kopyalar. Ancak splice orijinal diziyi değiştirir, belirtilen bölümü çıkarır veya yeni eleman ekleyer.

## Array Soruları 2
`const arr = [1,2,3,4,5,6,7,7,8,6,10];`
#### **1. arrayindeki yinelenen sayıları bulun.**
```javascript
const arr = [1,2,3,4,5,6,7,7,8,6,10];
function getDuplicates(data) {
    return data.filter((value, index) => data.indexOf(value) !== index);
}

console.log(getDuplicates(arr));
```

#### **2. arrayindeki tüm yinelenen sayıları silip yeni bir arrayi 2 farklı method ile oluşturun.**
```javascript
//Method 1 - filter ile:
const arr = [1,2,3,4,5,6,7,7,8,6,10];
function removeDuplicates(data) {
    return data.filter((value, index) => data.indexOf(value) === index);
}

console.log(removeDuplicates(arr));

//Method 2 - set ile:
const arr = [1,2,3,4,5,6,7,7,8,6,10];
function removeDuplicates(data) {
    return [...new Set(data)]
}

console.log(removeDuplicates(arr));

```

#### **3. arrayindeki en yüksek ve en düşük değeri 2 farklı methodla bulun.**
```javascript
//Method 1- Reduce ile:
const arr = [1,2,3,4,5,6,7,7,8,6,10];

const{max, min} = arr.reduce(
    (acc, curr) => ({
        max: Math.ax(acc.max, curr),
        min: Math.min(acc.min, curr),
    }),
    {max: -Infinity, min: Infinity}
);

console.log("En yüksek değer:", max);
console.log("En düşük değer:", min);

//Method 2- Math.min, Math.max ile:


```

## Kodlama Soruları
1- Bu kodun çıktısı nedir? Neden?
```javascript
function job() {
    return new Promise(function(resolve, reject) {
        reject();
    });
}

let promise = job();

promise
    .then(function() {
        console.log('Success 1');
    })
    .then(function() {
        console.log('Success 2');
    })
    .then(function() {
        console.log('Success 3');
    })
    .catch(function() {
        console.log('Error 1');
    })
    .then(function() {
        console.log('Success 4');
    });
```

Output:
```
Error 1
Success 4
```
İlk olarak `job` fonksiyonu bir Promise döndürüyor ve bu Promise hemen reddediliyor (reject). Bu nedenle, önceki `.then` blokları atlanarak direkt `.catch` bloğu çalıştırılır. Ancak zincirin sonundaki `then` bloğu olan `Success 4` çalışır çünkü bu blok önceki promise zincirinde bir hata olup olmadığına bakmaksızın her durumda çalışır.

2- Bu kodun çıktısı nedir? Neden?
```javascript
function job(state) {
    return new Promise(function(resolve, reject) {
        if (state) {
            resolve('success');
        } else {
            reject('error');
        }
    });
}

let promise = job(true);

promise
    .then(function(data) {
        console.log(data);
        return job(true);
    })
    .then(function(data) {
        if (data !== 'victory') {
            throw 'Defeat';
        }
        return job(true);
    })
    .then(function(data) {
        console.log(data);
    })
    .catch(function(error) {
        console.log(error);
        return job(false);
    })
    .then(function(data) {
        console.log(data);
        return job(true);
    })
    .catch(function(error) {
        console.log(error);
        return 'Error caught';
    })
    .then(function(data) {
        console.log(data);
        return new Error('test');
    })
    .then(function(data) {
        console.log('Success:', data.message);
    })
    .catch(function(data) {
        console.log('Error:', data.message);
    });
```

Output:
```

```
