![MarkDown](https://img.shields.io/badge/Kurs-MarkDown-cccccc?style=for-the-badge&logo=markdown)
![Dil](https://img.shields.io/badge/Kaynak-T%C3%BCrk%C3%A7e-red?style=for-the-badge&logo=bookstack&logoColor=white)

Videolu içerikten faydalanın! (Belki 20 dakikada da öğrenebilirsiniz.)

[![YouTube Video](https://img.shields.io/badge/Videoya_gİt-red?logo=youtube&style=for-the-badge)](https://www.youtube.com/watch?v=uRM54l1bQrk)
![YouTube Video Views](https://img.shields.io/youtube/views/uRM54l1bQrk?label=%C4%B0zlemeler&logo=youtube&logoColor=red&style=for-the-badge)
![YouTube Video Likes](https://img.shields.io/youtube/likes/uRM54l1bQrk?label=Beğeniler&logo=undertale&logoColor=red&style=for-the-badge)

Github hesabınız varsa repoya yıldız bırakmayı unutmayın. :smile:

![Yıldızlar](https://img.shields.io/github/stars/Elagoht/30-dakikada-markdown-ogrenin?Label=Yıldızlar&logo=starship&logoColor=white&style=for-the-badge)

# MarkDown Nedir?

Markup, yani işaretleme dilleri gerekli programlar tarafından yorumlanarak
insanların daha kolay anlayabilecekleri bir hale getirilmesini sağlarlar.
Bunlardan en sık kullanılanı, ve herkesçe duyulanı HTML (Hyper Text Markup
Language) olarak karşımıza çıkar. MarkDown ise Up kelimesini tersine çevirerek
kendince bir kelime oyunu yapmıştır.

MarkDown HTML etiketlerini de destekleyen ve gerçekten çok kısa sürede kolayca
öğrenilebilecek bir işaretleme dilidir.

# Neden MarkDown Öğrenmeliyim?

Eğer bu yazıyı Github üzerinden okuyorsanız -öncelikle orijinal repoya yıldız
atın- Github'da neredeyse her repoda `README.md` dosyaları olduğunun farkına
varmışsınızdır. Bu dosyalar Github tarafından reponun web sitesinde HTML
olarak yorumlanarak sayfada gösterilir. Fark edeceğiniz üzere şu an okuduğunuz
dosya da README.md dosyasıdır. O halde ilk olarak Github'da projelerimizi doğru
bir şekilde tanıtmak için markdown öğrenmelisiniz.

İkincil olarak da markdown tabanlı blog yazıları yayınlamak isteyebilirsiniz.
MarkDown ile kolayca yazdığınız metinleri otomatik olarak web sitenize ekleyen
programlar bulunmakta. Burada kullanmak için de MarkDown öğrenebilirsiniz.

Ayrıca ben ders notlarımı da yazması kolay olduğu için MarkDown formatında
tutuyorum. Ardından bu notları programlarıma tanıtmak çok kolay oluyor.

Programlara metninizi mantıksal olarak tanıtmak da çok kolay.

# MarkDown Elementleri

MarkDown'ın başlıca amacı yazılarımızın web tarayıcılarında mantıksal olarak
görüntülenmesidir. Web tarayıcıları da HTML dilinden anladığına göre MarkDown
ile yazdığımız elementler de HTML'e çevrilmek zorunda. O halde elimizde neler
olduğuna bir bakalım.

**MarkDown Elementleri:**

* Yazı tipleri
    * Kalın
    * İtalik
    * Altı çizili
    * Üstü çizili
    * Fonu renkli
* Başlıklar (1-6. derece arası)
* Paragraflar
* Sıralı ve sırasız listeler
* Kod blokları
* Yatay ayraçlar
* Resimler
* Bağlantılar
* Alıntılar
* Tablolar
* Alt notlar
* Tanım listeleri
* Görev listeleri
* Emojiler
* Üst ve alt yazı

Şimdi teker teker bunların ne olduğuna bakalım.

## Yazı Tipleri

Metninizde dikkat çekmeniz gereken yerlerde **kalın**, _italik_, ~~üstü
çizili~~, <u>altı çizili</u> ==fonu renkli== yazılar yazmak isteyebilirsiniz.
Ancak birçok MarkDown işleyicisi altı çizili veya fonu renlkli yazıyı
desteklemeyecektir. Burada HTML kodları kullanmanız gerekecektir.

```md
* **Kalın yazı**
* __Kalın yazı__
* _İtalik yazı_
* *İtalik yazı*
* ___Kalın italik yazı___
* _**Kalın italik yazı**_
* **_Kalın italik yazı_**
* ~~Üstü çizili yazı~~
* <u>Altı çizili yazı</u>
* ==Fonu renkli yazı== (Çoğunlukla desteklenmez.)
* <mark>Fonu renkli yazı</mark>
```

Bu gösterimlerin HTML hâli şu şekildedir:

```html
<ul>
	<li><b>Kalın yazı</b></li>
	<li><b>Kalın yazı</b></li>
	<li><i>İtalik yazı</i></li>
	<li><i>İtalik yazı</i></li>
	<li><b><i>Kalın italik yazı</i></b></li>
	<li><i><b>Kalın italik yazı</b></i></li>
	<li><b><i>Kalın italik yazı</i></b></li>
	<li><strike>Üstü çizili yazı</strike></li>
	<li><u>Altı çizili yazı</u></li>
	<li>==Fonu renkli yazı== (Çoğunlukla desteklenmez.)</li>
	<li><mark>Fonu renkli yazı</mark></li>
</ul>
```

---

Dokümanın işlenmiş hâli:

* **Kalın yazı**
* __Kalın yazı__
* _İtalik yazı_
* *İtalik yazı*
* ___Kalın italik yazı___
* _**Kalın italik yazı**_
* **_Kalın italik yazı_**
* ~~Üstü çizili yazı~~
* <u>Altı çizili yazı</u>
* ==Fonu renkli yazı== (Çoğunlukla desteklenmez.)
* <mark>Fonu renkli yazı</mark>

## Başlıklar

Web tarayıcıları varsayılan olarak 6 düzeyde başlık tanımlaması yapar.
Mantıksak olarak da arama motorlarınca bu başlık düzeyleri taranır. HTML
üzerinde `<h1>1. Düzey Başlık</h1>`, `<h6>6. Düzey Başlık</h6>`
şeklinde tanımlamalar yapılırken bunlar MarkDown üzerinde

```md
# 1. Düzey Başlık
## 2. Düzey Başlık
### 3. Düzey Başlık
#### 4. Düzey Başlık
##### 5. Düzey Başlık
###### 6. Düzey Başlık
```

olarak gösterilir. Yani kaçıncı dereceden olacaksa o kadar `#` koyarız. Ancak
başlık ile `#` arasında boşluk olmasına dikkat edin.

Dokümanın işlenmiş hâli:

# 1. Düzey Başlık
## 2. Düzey Başlık
### 3. Düzey Başlık
#### 4. Düzey Başlık
##### 5. Düzey Başlık
###### 6. Düzey Başlık

## Paragraflar

Paragraf için herhangi bir şey belirtmenize gerek yok. Normalde HTML üzerinde
`<p>Paragraf metni burada.</p>` şeklinde gösterilen bu element, MarkDown
üzerinde sadece bir adet fazladan satır atlama ile belirtilir.

Tek satır atladığınızda paragrafa aynen devam eder. İkinci bir paragrafa geçmek
için fazladan satır aralığı bırakmalısınız. 

> **Not:** Vim üzerinde `vgw` kısayolu ile gösterdiğimiz satırı birden fazla satıra
> bölme komutu ile metin düzenleyicisinde daha rahat kod yazabileceğimizi
> biliyoruz. Bu nedenle de fazladan satır atlamak önemlidir.

---

Dokumanın işlenmiş hâli:

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Et malesuada fames ac turpis
egestas maecenas pharetra convallis. Eget egestas purus viverra accumsan in
nisl nisi scelerisque.

Sodales ut etiam sit amet nisl purus in. Aliquam ultrices sagittis orci a
scelerisque purus. Etiam dignissim diam quis enim lobortis scelerisque.
Scelerisque in dictum non consectetur a. Nibh venenatis cras sed felis. Nunc
faucibus a pellentesque sit amet. 

## Sıralı ve Sırasız Listeler

Listelerde sıranın önemli olduğu ve olmadığı durumlarda iki farklı türünü
kullanıyoruz.

### Sıralı Listeler 

Sıralı listelerde sıralar web tarayıcılarınca otomatik olarak artırlmaktadır.
Dolayısıyla HTML ve MarkDown formalarında da kendiniz artırarak gitmek zorunda
değilsiniz. Sadece başlangıç değerini vermeniz MarkDown için yeterlidir. Sayı,
nokta ve boşluk koyularak liste elemanı oluşturulur.

```md
1. Liste Elemanı
2. Liste Elemanı
3. Liste Elemanı
```

gösterimi aslında 

```md
1. Liste Elemanı
1. Liste Elemanı
1. Liste Elemanı
```

ile aynıdır. Bu gösterim HTML de aşağıdaki şekilde gösterilir.

```html
<ol>
    <li>Liste Elemanı</li>
    <li>Liste Elemanı</li>
    <li>Liste Elemanı</li>
</ol>
```

Gördüğünüz üzere HTML gösteriminde de sıralama için herhangi bir sıra vermedik.
Sıralamaya başka bir şekilde başlamak isteseydik istediğimiz sayı ile yazmaya
başlayabilirdik. Bu durumda da sadece ilk elemanın numaraasına dikkat etmemiz
yetecektir.

```md
17. Liste Elemanı
1. Liste Elemanı
1. Liste Elemanı
```

Bu gösterim ise HTML'de şu anlama gelir:

```html
<ol start="17">
    <li>Liste Elemanı</li>
    <li>Liste Elemanı</li>
    <li>Liste Elemanı</li>
</ol>
```

---

> **Not:** Maalesef MarkDown sadece varsayılan listeleme türlerini
> kullanabilmekte. Sayı, harf, Romen rakamı gibi gösterimleri css ya da html
> ile ayarlamanız gerekmektedir.

Dokümanın işlenmiş hâli:

17. Liste Elemanı
1. Liste Elemanı
1. Liste Elemanı

### Sırasız Listeler

Elemanlarının sırası önemli olmayan durumlarda bu liste türü kullanılır. Burada
eleman belirtmek için `-`, `*` ya da `+` ifadeleri ve ardından bir boşluk
koyularak yazmaya başlanır.

```md
* Liste Elemanı
- Liste Elemanı
+ Liste Elemanı
```

Bu gösterimin HTML karşılığı şu şekilde olacaktır:

```html
<ul>
	<li>Liste Elemanı</li>
</ul>
<ul>
	<li>Liste Elemanı</li>
</ul>
<ul>
	<li>Liste Elemanı</li>
</ul>
```

Anlamına gelecektir çünkü burada 3 farklı liste elemanı operatörü kullandık.
Dolayısıyla 3 farklı listemiz bulunmakta.

---

Dokümanın işlenmiş hâli:

* Liste Elemanı
- Liste Elemanı
+ Liste Elemanı

### İç İçe Listeler

Bir liste elemanının alt elemanları da bulunabilir. Bu durumlarda tab boşluğu
ya da 4 tane boşluk bırakabilirsiniz. Ayrıca sıralı ve sırasız listeler iç içe
kullanılabilir. Örneğin: 

```md
* Liste Elemanı
    1. Alt Liste Elemanı
    1. Alt Liste Elemanı
        - Alt Listenin Alt Elemanı
        - Alt Listenin Alt Elemanı
        - Alt Listenin Alt Elemanı
    1. Alt Liste Elemanı   
* Liste Elemanı
* Liste Elemanı
```

---

Dokümanın işlenmiş hâli:

* Liste Elemanı
    1. Alt Liste Elemanı
    1. Alt Liste Elemanı
        - Alt Listenin Alt Elemanı
        - Alt Listenin Alt Elemanı
        - Alt Listenin Alt Elemanı
    1. Alt Liste Elemanı   
* Liste Elemanı
* Liste Elemanı

## Kod Blokları

Kod blokları her işleyici tarafından işlenir ancak sözdizimi renklendirme
özelliğini hepsi sağlamayabilir. Github'da bir README dosyası yazacaksanız bu
özelliği kullanabilirsiniz.

Kod blokları şu şekilde gösterilir:

<pre>
```
def sayHi():
    print("Merhaba Dünya!")
}
```
</pre>

Burada kullanılan tırnaklar back quote, backtick olarak belirtilir ve Türkçe Q
klavyede <kbd>Alt Gr</kbd>+<kbd>,</kbd> ile yazılır.

Bu gösterimin HTML karşılığı şu şekildedir.

```html
<code>
    def sayHi():
        print("Merhaba Dünya!")
</code>
```

---

Dokümanın işlenmiş hâli:

```
def sayHi():
    print("Merhaba Dünya!")
}
```

Bir de sözdizimi renklendirmeye bakalım. Dediğim gibi, bu özellik her platform
tarafından desteklenmeyebilir. Kullanmak içinse istediğiniz dilin adını ya da
dosya uzantısını, kod bloğu başlangıcına yazmanız yeterlidir.

<pre>
```js
const sayHi = () => {
    console.log("Merhaba Dünya")
}
```
</pre>
<pre>
```rust
fn main() {
    println!("Merhaba Dünya!")
}
```
</pre>

---

Dokümanın işlenmiş hâli:

```js
const sayHi = () => {
    console.log("Merhaba Dünya")
}
```

```rust
fn main() {
    println!("Merhaba Dünya!")
}
```

---

## Yatay Ayraçlar

İki metni birbirinden ayırmak için kullanılan ayraçlardır. HTML üzerinde `<hr/>`
elemanı ile gösterilirken MarkDown'da `---`, `***`, `*-*`, `-*-` gibi
şekillerde kullanılır.

---

Dokümanın işlenmiş hâli:

---

## Resimler

Dokümana resim koymak da oldukça kolaydır. Ünlem işareti koyup ardından **dik
parantezeler içinde** _resim açıklamasını_ ve **parantezler içinde** _resmin
adresini_ yazarak resim ekleyebilirsiniz. Örneğin:

```md
![Mavi Penguen Duvar Kağıdı](https://raw.githubusercontent.com/Elagoht/OneLinePinguin/main/pinguin-blue.png)
```

Bu gösterimin HTML karşılığı ise şu şekildedir:

```html
<img alt="Mavi Penguen Duvar Kağıdı" src="https://raw.githubusercontent.com/Elagoht/OneLinePinguin/main/pinguin-blue.png"/>
```

---

Dokümanın işlenmiş hâli:

![Mavi Penguen Duvar Kağıdı](https://raw.githubusercontent.com/Elagoht/OneLinePinguin/main/pinguin-blue.png)

## Bağlantılar

Bağlantılar ya da linkler, köprüler sayesinde sayfa içinde ya da başka
sayfalara bağlantı kurabiliriz. **Bağlantı oluşturmak istediğiniz metni** _dik
parantez içinde_ ve **bağlantıyı** _parantezler içinde_ vererek bağlantı
oluşturabilirsiniz. Yani bağlantıları, resimlerin başında ünlem işareti olmayan
hâli gibi düşünebilirsiniz.

```md
Kanalıma abone olmak için [tıkla](https://www.youtube.com/@herkesicinlinux)!
```

Bu gösterimin HTML karşılığı şu şekildedir:

```html
<p>
    Kanalıma abone olmak için <a href="https://www.youtube.com/@herkesicinlinux">tıkla</a>!
<p>
```

---

Dokümanın işlenmiş şekli ise şu şekilde olacaktır:

Kanalıma abone olmak için [tıkla](https://www.youtube.com/@herkesicinlinux)!

Ayrıca bir bağlantı ile bağlantı metni aynı olacaksa dik parantez ve parantezlerin içerisine aynı bağlantıyı yazmak yerine doğrudan küçüktür ve büyüktür işaretlerinin arasına bağlantıyı yazabilirsiniz.

```md
Github Profil Adresim: <https://github.com/Elagoht>
```

Dokümanın işlenmiş hâli:

Github Profil Adresim: <https://github.com/Elagoht>

## Alıntılar

Alıntılar normalde tırnak içerisinde gösterdiğimiz özlü söz gibi metinlerdir,
birden fazla satırda gösterilebilirler:

```md
> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
> tempor incididunt ut labore et dolore magna aliqua. Et malesuada fames ac
> turpis egestas maecenas pharetra convallis. Eget egestas purus viverra
> accumsan in nisl nisi scelerisque.
```

HTML üzerinde bu komut şu şekilde gösterilir:

```html
<blockquote>
    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
    eiusmod tempor incididunt ut labore et dolore magna aliqua. Et malesuada
    fames ac turpis egestas maecenas pharetra convallis. Eget egestas purus
    viverra accumsan in nisl nisi scelerisque.</p>
</blockquote>
```

---

Metnin işlenmiş hâli:

> Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
> tempor incididunt ut labore et dolore magna aliqua. Et malesuada fames ac
> turpis egestas maecenas pharetra convallis. Eget egestas purus viverra
> accumsan in nisl nisi scelerisque.

## Tablolar

HTML üzerinde tabloları algılamak oldukça zor olsa da MarkDown üzerinde işler
çok kolaydır. Ancak MarkDown üzerinde yazdığınız tabloların mutlaka bir
başlık satırı olmalıdır.

Hücreler düz çizgi (pipe) işareti (`|`) ile ayrılırken başlık satırından sonra
bir kere hücreleri `-` olan bir satır yazılır:

```md
| Başlık 1 | Başlık 2 |
| - | - |
| Hücre 1 | Hücre 2 |
| Hücre 3 | Hücre 4 |
```

şeklinde gösterilebileceği gibi metni ham halde okuyanlar açısından daha okunur
olması amacıyla aşağıdaki şekilde de gösterilebilir:

```md
| Başlık 1 | Başlık 2 |
| -------- | -------- |
| Hücre 1  | Hücre 2  |
| Hücre 3  | Hücre 4  |
```

Bu gösterimin HTML üzerindeki gösterimi aşağıdaki gibi olacaktır. Fark
edebileceğiniz üzere Markdown halini okumak çok daha kolaydır.

```html
<table>
	<thead>
		<tr>
			<th>Başlık 1</th>
			<th>Başlık 2</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>Hücre 1</td>
			<td>Hücre 2</td>
		</tr>
		<tr>
			<td>Hücre 3</td>
			<td>Hücre 4</td>
		</tr>
	</tbody>
</table>
```

---

Dokümanın işlenmiş hâli:

| Başlık 1 | Başlık 2 |
| -------- | -------- |
| Hücre 1  | Hücre 2  |
| Hücre 3  | Hücre 4  |

Ancak şunu da belirtmeliyiz ki eğer bir hücre ya da satırı uzatmak, hücreleri
birleştirmek isterseniz HTML kodlarını kullanmak zorunda kalırsınız.

Bununla birlikte tablolarda verinin nasıl hizalanacağına da karar
verebilirsiniz. Verileri, eğer tirelerden önce iki nokta (`:`) koyarsanız sola,
sonra koyarsanız sağa, her iki tarafına koyarsanız ortaya hizalar.

```md
| Ürün     | Fiyat |
|:--------:| -----:|
| Mont     | 999   |
| Ayakkabı | 399   |
| Pantolon | 449   |
| Gömlek   | 299   |
```

---

Dokümanın işlenmiş hâli:

| Ürün     | Fiyat |
|:--------:| -----:|
| Mont     | 999   |
| Ayakkabı | 399   |
| Pantolon | 449   |
| Gömlek   | 299   |

## Alt Notlar

Kitaplarda ve bilgisayar dokümanlarında bu notları görmeye oldukça alışığız. Al
bilgi olarak bazı kelime anlamları ya da çevirmenin notu gibi ek bilgileri
yazarız. Markdown'da bunu desteklese de her işleyici tarafından
desteklenmeyebilir[^1]. Aşağıdaki şekilde kullanabilirsiniz.

```
Açıklanması gereken metin[^1]

...

[^1]: Metnin açıklaması
```

---

Dokümanın işlenmiş hâli:

Açıklanması gereken metin[^2]

...

[^2]: Metnin açıklaması

## Tanım Listeleri

Tanım listeleri birden çok kavramı ve tanımını bir arada vermek için
kullanılır. Bu özellik de her işleyici de bulunmayabilir.

```md
Rust
: Düşük seviye bir dil sahip olan Rust, hafıza yönetimini en yüksek
  performansla sağlamaktadır.

Python
: Yüksek seviye dillerden biridir ve sözdiziminin esnekliği onu çok kullanışlı
  yapmaktadır. Ancak Diğer dillere göre oldukça yavaştır.

JavaScript
: Web tarayıcısında istemci taraflı çalışan, dinamik web sayfası içeriği
  oluşturmak için kullanılan bir betik dilidir.

Shell Script
: Unix kabuk programlama için kullanılan betik dilidir.
```

Gösterimin HTML karşılığı şu şekilde olacaktır:

```html
<dl>
	<dt>Rust</dt>
	<dd>Düşük seviye bir dil sahip olan Rust, hafıza yönetimini en yüksek performansla sağlamaktadır.</dd>
	<dt>Python</dt>
	<dd>Yüksek seviye dillerden biridir ve sözdiziminin esnekliği onu çok kullanışlı yapmaktadır. Ancak Diğer dillere göre oldukça yavaştır.</dd>
	<dt>JavaScript</dt>
	<dd>Web tarayıcısında istemci taraflı çalışan, dinamik web sayfası içeriği oluşturmak için kullanılan bir betik dilidir.</dd>
	<dt>Shell Script</dt>
	<dd>Unix kabuk programlama için kullanılan betik dilidir.</dd>
	<dt>Rust</dt>
	<dd>Düşük seviye bir dil sahip olan Rust, hafıza yönetimini en yüksek performansla sağlamaktadır.</dd>
</dl>
```

---

Dokümanın işlenmiş hâli:

Rust
:  Düşük seviye bir dil sahip olan Rust, hafıza yönetimini en yüksek
  performansla sağlamaktadır.

Python
: Yüksek seviye dillerden biridir ve sözdiziminin esnekliği onu çok
  kullanışlı yapmaktadır. Ancak Diğer dillere göre oldukça yavaştır.

JavaScript
: Web tarayıcısında istemci taraflı çalışan, dinamik web sayfası içeriği
  oluşturmak için kullanılan bir betik dilidir.

Shell Script
: Unix kabuk programlama için kullanılan betik dilidir.

## Görev Listeleri

Yapılacaklar listesi, alışveriş listesi gibi ihtiyaçları karşılayabilen bir
özelliktir. Bu özellik de her her yerde desteklenmeyebilir. Ayrıca `-` yerine
diğer liste elemanı işaretlerini de kullanabilirsiniz.

```md
- [X] Dokümanı dikkatlice oku.
- [ ] Github reposunu yıldızla.
- [ ] Youtube kanalına abone ol.
```

---

Dokümanın işlenmiş hâli:

- [X] Dokümanı dikkatlice oku.
- [ ] Github reposunu yıldızla.
- [ ] Youtube kanalına abone ol.

## Emojiler

Muhtemelen en az desteklenen özelliklerden biridir. Tüm emojilerin listesine
<https://github.com/markdown-templates/markdown-emojis> adresinden
ulaşabilirsiniz.

```md
:point_right::point_left:
```

---

Dokümanın işlenmiş hâli:

:point_right::point_left:

## Üst ve Alt Yazılar

Markdown ile de H~2~O, 3^rd^, 1^st^ gibi gösterimleri yazabilirsiniz.

```md
* H~2~O
* H~2~SO~4~
* 1^st^
* 2^nd^
* 3^rd^
* 4^th^
```

```html
<ul>
	<li>H<sub>2</sub>O</li>
	<li>H<sub>2</sub>SO<sub>4</sub></li>
	<li>1<sup>st</sup></li>
	<li>2<sup>nd</sup></li>
	<li>3<sup>rd</sup></li>
	<li>4<sup>th</sup></li>
</ul>
```

Metnin işlenmiş hâli:

* H~2~O
* H~2~SO~4~
* 1^st^
* 2^nd^
* 3^rd^
* 4^th^

# MarkDown Yetmediğinde

Fark ettiğiniz üzere MarkDown pratik ve kolay olması açısından geliştirilmiş
bir işaretleme dilidir. MarkDown'ın basitliğinin üzerinde daha karmaşık şeyler
yapacaksanız bunu HTML ile yapabilirsiniz.

Örneğin aşağıdaki kod bir MarkDown kodudur ancak HTML ile birebir aynıdır.
Çünkü MarkDown'da istediğiniz zaman HTML etiketlerine kaçabilirsiniz.

```md
<table>
	<thead>
		<tr>
			<th>Kategori</th>
			<th>Ürün</th>
			<th>Fiyat</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td rowspan="3">Giyim</td>
			<td>Mont</td>
			<td>999</td>
		</tr>
		<tr>
			<td>Ayakkabı</td>
			<td>399</td>
		</tr>
		<tr>
			<td>Pantolon</td>
			<td>449</td>
		</tr>
		<tr>
			<td rowspan="3">Kitap</td>
			<td>Yazılım</td>
			<td>147</td>
		</tr>
		<tr>
			<td>Roman</td>
			<td>68</td>
		</tr>
		<tr>
			<td>Kişisel Gelişim</td>
			<td>73</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td colspan="2" align="center">Toplam</td>
			<td>2135</td>
		</tr>
	</tfoot>
</table>
```

---

Dokümanın işlenmiş hâli:

<table>
	<thead>
		<tr>
			<th>Kategori</th>
			<th>Ürün</th>
			<th>Fiyat</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td rowspan="3">Giyim</td>
			<td>Mont</td>
			<td>999</td>
		</tr>
		<tr>
			<td>Ayakkabı</td>
			<td>399</td>
		</tr>
		<tr>
			<td>Pantolon</td>
			<td>449</td>
		</tr>
		<tr>
			<td rowspan="3">Kitap</td>
			<td>Yazılım</td>
			<td>147</td>
		</tr>
		<tr>
			<td>Roman</td>
			<td>68</td>
		</tr>
		<tr>
			<td>Kişisel Gelişim</td>
			<td>73</td>
		</tr>
	</tbody>
	<tfoot>
		<tr>
			<td colspan="2" align="center">Toplam</td>
			<td>2135</td>
		</tr>
	</tfoot>
</table>

# Kurs Bitti :blush:

Eğer kursu gerçekten faydalı bulduysanız repoyu yıldızlamayı, arkadaşlarınızla paylaşmayı unutmayınız. 


[^1]: Şu an buraya gelebiliyorsanız kullandığınız program tarafından bu özellik
    destekleniyor demektir.
