# --- BIRINCI DONEM PYTHON ÇEVRİMDIŞI EL KİTABI ---
## --- PYTHON BASLAYIP BITIRME PLANI ---
1. --Bölüm 2--Tahmini Süre 3--Odak Noktası 4--Neden Önemli?
1.1 Kısım: Temeller	5 - 7 Hafta	Döngüler, Karar Yapıları, Fonksiyonlar.	 Bu kısım senin temelin. Burası ne kadar sürerse sürsün (ister 5 ister 7 hafta), tam oturmadan geçmeyeceğiz.
2. Kısım: Profesyonellik	8 - 10 Hafta	OOP (Nesne Yönelimli Programlama), Hata Yönetimi, Dosyalar.	Backend'in kalbi burasıdır. Karmaşık sistemleri yönetmeyi burada öğreneceksin.
3. Kısım: Uzmanlık & Veri	12 - 14 Hafta	SQL, Veritabanları, API Mantığı ve Projeler.	Bilgiyi kalıcı hale getirip gerçek dünya uygulamalarına döktüğün yer.

Dönem,Odak Noktası,Hedef
Temmuz 2026,Python & Algoritma,Temeli Çelik Gibi Yapmak
Kasım 2026,SQL & Veritabanı,Verinin Kalbine İnmek
Eylül 2027,Java & Spring Boot,Almanya Bileti (En Kritik Aşama)
Ocak 2028,Linux & Docker,Sistem Altyapısı (DevOps Giriş)
## --- KUCUK GIRIS VE BILGI ---
### --- PYTHON'IN MANTIĞI VE ÇALIŞMA SİSTEMİ --- [0.1.0-0.1.9]
```PY
0.1.0 Python Nasıl Çalışır  (Yorumlayıcı Mantığı)
0.1.1 Python, "Interpreted" (Yorumlanan) bir dildir.

0.1.2 Mantık: Sen kodu yazdığında, bir "Yorumlayıcı" (Interpreter) kodu satır satır okur ve o an bilgisayara ne yapması gerektiğini söyler.

0.1.3 Farkı: C++ gibi diller önce tüm kodu bir "pakete" (exe dosyasına) dönüştürür, sonra çalıştırır. Python ise doğrudan satırı okur ve çalıştırır. Bu da hata bulmayı çok hızlandırır.

0.1.4 Python Bilgisayarı Nasıl Anlar?
Bilgisayarlar aslında sadece 0 ve 1 (elektrik var/yok) mantığıyla çalışır.

0.1.5 Süreç: Yazdığın print("Merhaba") kodu, önce Bytecode denilen bir ara forma, sonra da bilgisayarın işlemcisinin anlayacağı Makine Diline (0-1) dönüştürülür.

0.1.6 Kolaylık: Sen karmaşık 0-1 dünyasıyla uğraşmazsın, Python senin yerine bu çeviriyi yapar.

0.1.7 Diğer Dillerden Farkı Nedir?
Okunabilirlik: Python, İngilizceye en yakın dildir. C++'ta 10 satırda yapacağın işi Python'da 2 satırda yapabilirsin.

0.1.8 Hız vs. Kolaylık: C++ daha hızlı çalışır (donanıma yakındır) ama Python ile uygulama geliştirmek çok daha hızlıdır.

0.1.9 Kütüphaneler: Python'ın her şey için hazır bir "modülü" vardır. Tekerleği her seferinde yeniden icat etmene gerek kalmaz.
```
### --- KOD ORGANİZASYONU VE SIRALAMA DİSİPLİNİ --- [0.2.0-0.3.3]
```PY
0.2.0 Python kodu bir inşaat gibidir; önce temeli atmalı, sonra katları çıkmalı ve en son dekorasyonu yapmalısın. 

0.2.1 Python yukarıdan aşağıya (top-to-bottom) okuma yaptığı için sıralama hayati önem taşır.

0.2.2 Kat: Kütüphaneler (Imports)
Detay: Programına dışarıdan süper güçler eklediğin yerdir.

0.2.2 Küçük Örnek:
import math # Matematiksel formülleri getirir
import random # Rastgele sayı üretme yeteneği getirir

0.2.3 Kat: Sabitler ve Değişkenler (Variables)
Detay: Kodun her yerinde kullanacağın ana verileri burada tanımlarsın.

0.2.4 Küçük Örnek:
kullanici_adi = "Dawut"
hedef_ulke = "Avusturya"
python_notlari = [90, 100, 95]

0.2.5 Kat: Fonksiyonlar (Functions)
0.2.6 Detay: Bir işi yapan "mini makinelerdir". Onları burada kurarsın ama henüz düğmesine basmazsın.

0.2.7 Küçük Örnek:
def selamla():
    print("Merhaba Mühendis Dawut!")

0.2.8 Kat: Ana Çalıştırma Alanı (The Main Loop / Execution)
0.2.9 Detay: Yukarıda hazırladığın her şeyi burada birleştirirsin. Kodun aslında "başladığı" yer burasıdır.

0.3.0 Küçük Örnek:
selamla() # Yukarıdaki fonksiyonu şimdi çağırdık
print(kullanici_adi + " için kod çalışıyor...")

# --- BÜYÜK MÜHENDİSLİK ÖRNEĞİ (Hepsini Birleştiriyoruz)
0.3.1 Bu örnekte bir öğrencinin Python notlarını hesaplayan ve sıralayan tam bir kod yapısı görmekteyiz

0.3.2 Büyük Örnek:
# --- 1. KÜTÜPHANELER ---
import math # Karmaşık hesap gerekirse hazırda dursun

# --- 2. DEĞİŞKENLER (VERİLER) ---
ogrenci_adi = "Dawut Gociyew"
ders_notlari = [85, 95, 100, 70] # Python sınav sonuçları

# --- 3. FONKSİYONLAR (İŞLEMLER) ---
def notlari_duzenle(liste):
    """Notları büyükten küçüğe sıralayan fonksiyon"""
    liste.sort(reverse=True)
    return liste

def ortalama_hesapla(liste):
    """Notların ortalamasını bulan fonksiyon"""
    toplam = sum(liste)
    adet = len(liste)
    return toplam / adet

# --- 4. ANA ÇALIŞTIRMA (SONUÇ) ---
print("--- Sistem Başlatılıyor ---")

# Fonksiyonları kullanıyoruz
sirali_liste = notlari_duzenle(ders_notlari)
ortalama = ortalama_hesapla(ders_notlari)

# Ekrana yazdırma
print("Öğrenci:", ogrenci_adi)
print("Sıralı Notların:", sirali_liste)
print("Başarı Ortalaman:", ortalama)

if ortalama > 80:
    print("Durum: Harika! Mühendislik için hazırsın.")


0.3.4 # --- BIRLESTIRILMIS BUYUK ORNEGI ---


# --- Degiskenler ---
SINIR_KAPISI_ADI = "Arztorzka Dogu Sinir Kapisi"
MAX_GIRIS_DENEMESI = 3
YAS_SINIRI = 18
MIN_BANKA_BAKIYESI = 5000
YASAKLI_ESYALAR = ["silah", "uyusturucu", "kacak icerik", "sahte pasaport"]

# --- Fonksiyonlar ---
def vize_kontrol(gecici_vize_durumu, puan):
    """Vize durumunu ve Almanca puanini kontrol eder."""
    if gecici_vize_durumu and puan >= 70:
        return True
    return False

def esya_kontrol(esya_listesi):
    """Yasakli esyalari kontrol eder."""
    for esya in esya_listesi:
        if esya.lower() in YASAKLI_ESYALAR:
            return False # Yasakli esya bulundu
    return True # Yasakli esya yok

def giris_yap(isim):
    """Basarili giris mesaji."""
    print(f"\n{isim}, Hos Geldin Arztozka'ya! Gecisiniz onaylandi. Heil Arztorzka!")

def giris_red(isim, neden):
    """Giris reddedildiginde gosterilen mesaj."""
    print(f"\nUzgunuz {isim}, girisiniz reddedildi. Sebep: {neden}")

# --- Ana Program Akisi ---
print(f"--- {SINIR_KAPISI_ADI} Sistemine Hos Geldiniz ---")

deneme_sayisi = 0
while deneme_sayisi < MAX_GIRIS_DENEMESI:
    print(f"\n--- Giris Denemesi {deneme_sayisi + 1} / {MAX_GIRIS_DENEMESI} ---")
    
    isim = input("Tam Adiniz: ")
    yas = int(input("Yasiniz: "))
    banka_bakiyesi = float(input("Banka bakiyeniz (Euro): "))
    almanca_puan = int(input("Almanca Sinav Puaniniz (0-100): "))
    vize_durumu = input("Vizeniz var mi? (evet/hayir): ").lower() == 'evet'
    
    # Listeler: Esya girdisi
    esya_girdisi = input("Yaninizdaki esyalari virgul ile ayirarak giriniz (orn: telefon, kitap, silah): ")
    yolcu_esyalari = [esya.strip().lower() for esya in esya_girdisi.split(',')]

    # Fonksiyon Cagrilari ve Kosullu Kontroller (If-Elif-Else)
    if not vize_kontrol(vize_durumu, almanca_puan):
        giris_red(isim, "Vize veya Almanca puaniniz yetersiz.")
    elif yas < YAS_SINIRI:
        giris_red(isim, "Yasiniz yetersiz.")
    elif banka_bakiyesi < MIN_BANKA_BAKIYESI:
        giris_red(isim, "Banka bakiyeniz yetersiz.")
    elif not esya_kontrol(yolcu_esyalari): # Fonksiyon cagrisi
        giris_red(isim, "Yasakli esya tasima.")
    else:
        giris_yap(isim)
        break # Basarili giris, donguden cik
        
    deneme_sayisi += 1

if deneme_sayisi == MAX_GIRIS_DENEMESI:
    print("\n--- Maksimum giris denemesi aşıldı. Lütfen daha sonra tekrar deneyiniz. ---")

print("--- Sistem Sonlandi ---")

```
### --- PYTHON'IN 4 TEMEL SÜTUNU (THE BIG FOUR) --- [0.4.0-0.6.0]
```PY
0.4.0 Bir programın hayatta kalması için bu dört yapıya ihtiyacı vardır. Bunları bir mutfak gibidir mesela:

0.4.1 # --- I. Değişkenler (Variables) - "Kavanozlar"
0.4.2 Nedir: Bilgiyi bilgisayarın hafızasında saklamak için kullandığın etiketli kavanozlardır.

0.4.3 Neden Kullanılır: Bir veriyi (isim, sayı, fiyat) defalarca kullanmak için isimlendirmek gerekir.

0.4.4 Örnek:
isim = "Dawut"          # String (Metin)
yas = 16                # Integer (Tam sayı)
hedef = "Avusturya"     # String
puan = 95.5             # Float (Ondalıklı sayı)

0.4.5 II. # --- Listeler (Lists) - "Dolaplar"
0.4.6 Nedir: Birden fazla değişkeni tek bir isim altında, sırayla tutan koleksiyonlardır.

0.4.7 Neden Kullanılır: 100 tane öğrenci ismini 100 ayrı değişkene yazmak yerine tek bir "ogrenciler" listesine koymak için.

0.4.8 Örnek:
diller = ["Almanca", "Python", "Turkmen"]
diller.append("Ingilizce") # Listeye yeni eleman ekler
diller.sort()              # Alfabetik sıralar

0.4.9 # --- III. Döngüler (Loops) - "Tekrarlayıcılar"
0.5.0 Nedir: Bir işlemi, belirli bir koşul gerçekleşene kadar veya bir listenin sonuna gelene kadar defalarca yapan mekanizmadır.

0.5.0 Neden Kullanılır: 1000 elemanlı bir listedeki her ismi tek tek ekrana yazdırmak için 1000 satır kod yazmamak, sadece 2 satırla işi bitirmek için.

0.5.1 Örnek:
# Listedeki her dili sırayla yazdırır
for dil in diller:
    print(dil + " öğreniyorum.")

0.5.2 # --- IV. Fonksiyonlar (Functions) - "Mutfak Robotları"
0.5.3 Nedir: Belirli bir görevi olan, istediğin zaman çağırıp çalıştırabildiğin kod bloklarıdır.

0.5.4 Neden Kullanılır: Bir matematiksel hesabı veya işlemi kodun 10 farklı yerinde kullanacaksan, her seferinde aynı kodu yazmak yerine fonksiyonu çağırırsın.

0.5.5 Örnek:
def selamla(kisi):
    print("Merhaba " + kisi + ", mühendislik yolunda başarılar!")

selamla("Dawut") # Fonksiyonu çağırdık

# --- BÜYÜK "4 SÜTUN" BİRLEŞİK ÖRNEĞİ ---
0.5.6 Şimdi bu dördünü tek bir senaryoda birleştirelim: Bir Almanca kelime öğrenme sistemi:
# 1. DEĞİŞKENLER (Verilerimiz)
kullanici = "Dawut"
ogrenilecek_kelime_sayisi = 72

# 2. LİSTELER (Kelimelerimiz)
almanca_kelimeler = ["bis bald", "natürlich", "prost"]

# 3. FONKSİYONLAR (İşlemimiz)
def kelime_kartini_goster(kelime):
    # Bu fonksiyon bir kelimeyi süslü bir şekilde yazdırır
    print("--- KART ---")
    print("Almanca: " + kelime)
    print("------------")

# 4. DÖNGÜLER (Hepsini çalıştırma)
print(kullanici + " için kelime listesi hazırlanıyor...\n")

for kelime in almanca_kelimeler:
    kelime_kartini_goster(kelime) # Her kelime için fonksiyonu çalıştırır

# --- Mühendislik Özeti ---
0.5.7 Değişken bilgiyi tutar.

0.5.8 Liste bilgileri gruplar.

0.5.9 Fonksiyon bilgiyle ne yapılacağını tarif eder.

0.6.0 Döngü işlemi herkes için tekrarlar.
```
## --- PYTHON TEMEL MANTIK ARSIVI ---
#### --- [TEMEL_DEGISKENLER] --- {I-KISIM}
##### --- PRINT(SEP VE END)--- [1.0-1.9]
```PY
1.0 print() - Veri Yazdırma

1.1 Nedir: Belirtilen mesajı veya değişkeni ekrana (terminale) yazdırmak için kullanılır.

1.2 Nasıl Kullanılır: Fonksiyonun parantezleri içine yazdırmak istediğin veriyi girersin. Metinler (string) tırnak içinde, değişkenler ise tırnaksız yazılır

1.3 Örnek:
print("Merhaba Dünya") # Metin yazdırır
sayi = 10
print(sayi) # Değişkenin değerini yazdırır
```
###### --- SEP
```PY
1.4 sep Parametresi - Ayırıcı Kontrolü
1.5 Nedir: print() fonksiyonu içinde virgülle ayrılmış birden fazla veri varken, bu verilerin arasına hangi işaretin geleceğini belirler.

1.6 Nasıl Kullanılır: print() parantezinin en sonuna sep="sembol" şeklinde eklenir. Eğer kullanılmazsa Python otomatik olarak bir boşluk bırakır.

1.7 Örnek:
print("D", "A", "W", "U", "T", sep="-")
# Çıktı: D-A-W-U-T (Aralara çizgi koydu)
```
###### --- END
```PY
1.8 end Parametresi - Satır Sonu Kontrolü
1.9 Nedir: print() fonksiyonu işini bitirdiğinde satırın en sonuna ne koyacağını ve alt satıra geçip geçmeyeceğini belirler.

1.9.1 Nasıl Kullanılır: print() parantezinin sonuna end="sembol" şeklinde eklenir. Eğer kullanılmazsa Python otomatik olarak alt satıra geçer (\n).

1.9.2 Örnek:
print("Yükleniyor", end="...")
print("Bitti")
# Çıktı: Yükleniyor...Bitti (Alt satıra geçmeden yan yana yazdı)
```
##### --- INPUT --- [2.0-2.3]
```PY
2.0 input() - Kullanıcıdan Veri Alma

2.1 Nedir: Program çalışırken kullanıcıdan klavye yoluyla bilgi almak için kullanılır.

2.2 Nasıl Kullanılır: Alınan veri her zaman string (metin) tipindedir. Eğer sayısal bir işlem yapacaksan dönüştürmen gerekir.

2.3 Örnek:
isim = input("Adın nedir? ")
print("Hoş geldin " + isim)
```
##### --- INT --- [3.0-3.3]
```PY
3.0 int() - Tam Sayı Dönüştürme

3.1 Nedir: Bir metni veya ondalıklı sayıyı tam sayıya (integer) çevirmek için kullanılır.

3.2 Nasıl Kullanılır: Özellikle input() ile alınan sayısal verileri matematiksel işleme sokmak için şarttır.

3.3 Örnek:
yas = int(input("Yaşını gir: ")) # Kullanıcıdan gelen metni sayıya çevirdik
print(yas + 5)
```
##### --- STR --- [4.0-4.3]
```PY
4.0 str() - Metne Dönüştürme (String)

4.1 Nedir: Herhangi bir veri tipini (sayı, liste, sözlük vb.) metin (string) formatına dönüştürür. Özellikle sayıları metinlerle birleştirip ekrana yazdırmak istediğinde hayat kurtarır.

4.2 Nasıl Kullanılır: Dönüştürülmek istenen nesne parantez içine alınır.

4.3 Örnek:
yas = 16
mesaj = "Dawut " + str(yas) + " yasinda." # Sayıyı metne çevirip birleştirdik
print(mesaj) # Çıktı: Dawut 16 yasinda.
```
##### --- FLOAT --- [5.0-5.3]
```PY
5.0 float() - Ondalıklı Sayı Dönüştürme
5.1 Nedir: Belirtilen bir tam sayıyı veya sayı içeren bir metni ondalıklı sayıya (floating point) çevirmek için kullanılır. Python'da hassas hesaplamalar (para birimi, koordinat vb.) için gereklidir.

5.2 Nasıl Kullanılır: Parantez içine dönüştürmek istediğin değer yazılır. Eğer değer sayıya dönüştürülemiyorsa hata verir.

5.3 Örnek:
sayi = float(5)        # Çıktı: 5.0 (Tam sayıyı ondalıklı yapar)
fiyat = float("19.99") # Çıktı: 19.99 (Metni sayıya çevirir)
```
##### --- LEN --- [6.0-6.3]
```PYTHON
6.0 len() - Uzunluk Ölçme

6.1 Nedir: Bir listenin eleman sayısını veya bir metnin kaç karakterden oluştuğunu verir.

6.2 Nasıl Kullanılır: Parantez içine uzunluğu ölçülecek nesne (liste, string vb.) yazılır.

6.3 Örnek:
sehirler = ["Istanbul", "Viyana", "Askabat"]
print(len(sehirler)) # Çıktı: 3
```
##### --- SEMBOLLER_VE_OPERATORLER--[7.0-7.9]
###### --- MATEMATIKSEL OPERATORLER --- [7.0-7.5]
```PY
7.0 + (Toplama / Birleştirme): İki sayıyı toplar. Eğer metinlerle (string) kullanılırsa, metinleri birbirine ekler.

Örnek: 5 + 10 = 15 | "Python" + " Hard" → "Python Hard"

7.1 - (Çıkarma): Bir sayıyı diğerinden çıkarmak için kullanılır.

Örnek: 20 - 5 = 15

7.2 * (Çarpma): Sayıları çarpar. Metinlerle kullanılırsa metni tekrarlar.

Örnek: 4 * 3 = 12 | "A" * 3 → "AAA"

7.3 / (Bölme): Bölme işlemi yapar. Sonuç her zaman float (ondalıklı) döner.

Örnek: 10 / 2 = 5.0

7.4 % (Mod Alma): Bölme işleminden kalan sayıyı verir. IQ soruları gibi mantık yürütürken (çift/tek sayı bulma) çok işine yarar.

Örnek: 10 % 3 = 1 (10'un içinde 3 üç kere var, kalan 1)
```
###### --- YAPISAL SEMBOLLER --- [7.6-7-9]
```PY
7.6.1 () (Normal Parantez): Fonksiyonları çağırmak (örneğin print()) ve matematikteki işlem önceliğini belirlemek için kullanılır.

Örnek: (2 + 3) * 4 = 20

7.6.2 { } (Süslü Parantez): f-string içinde değişkenleri göstermek ve ileride göreceğimiz "Sözlük" (Dictionary) yapılarını oluşturmak için kullanılır.

Örnek: f"Merhaba {isim}"

7.6.3 [] (Köşeli Parantez): Listeleri tanımlamak veya bir verinin içindeki belirli bir sıradaki (indeks) elemana ulaşmak için kullanılır.

Örnek: sehirler[0] (Listenin ilk elemanını seçer).

7.7 : (İki Nokta Üst Üste): Python'da bir blok (döngü, fonksiyon veya koşul) başlatırken veya "dilimleme" (slicing) işlemlerinde aralık belirtirken kullanılır.

Örnek: print(isim[0:3]) (0'dan 3'e kadar olan harfleri al).

7.8 " veya ' (Tırnak İşaretleri): Python'da bir verinin metin (string) olduğunu belirtmek için kullanılır. Başta ne kullandıysan sonda da aynısını kullanmalısın.

Örnek: "Merhaba" veya 'Dünya'

7.9 # (Yorum Satırı): Kodun yanına açıklama yazmak için kullanılır. Python bu satırı okumaz, sadece yazılımcı (senin) için nottur.

Örnek: # Bu satır ekrana isim yazdırır.
```

#### --- [LISTELER] --- {II-KISIM}
##### --- APPEND()--[8.0-8.3]
```PY
8.0 append() - Sona Ekleme

8.1 Nedir: Mevcut bir listenin en sonuna yeni bir eleman eklemek için kullanılır.

8.2 Nasıl Kullanılır: liste_adi.append(yeni_eleman) şeklinde yazılır.

8.3 Örnek:
sayilar = [1, 2, 3]
sayilar.append(4)
print(sayilar) # Çıktı: [1, 2, 3, 4]
```
##### --- LISTE[]--[9.0-9.3]
```PY
9.0 liste[0] - İndeksleme (Erişim)

9.1 Nedir: Bir listenin içindeki belirli bir sıradaki elemana ulaşmak için kullanılır. Python saymaya 0'dan başlar.

9.2 Nasıl Kullanılır: Köşeli parantez içine ulaşmak istediğin sıranın numarasını yazarsın.

9.3 Örnek:
meyveler = ["Elma", "Armut", "Muz"]
print(meyveler[0]) # Çıktı: "Elma"
print(meyveler[2]) # Çıktı: "Muz"
```
##### --- INSERT()--[10.0-10.3]
```PY
10.0 insert() - Araya Ekleme

10.1 Nedir: Bir elemanı listenin sonuna değil, istediğin özel bir konuma (indekse) yerleştirmek için kullanılır.

10.2 Nasıl Kullanılır: insert(indeks, eleman) şeklinde kullanılır. Belirlediğin indeksteki eski eleman sağa kayar.

10.3 Örnek:
isimler = ["Dawut", "Gemini"]
isimler.insert(1, "Python") # 1. indekse (araya) ekle
print(isimler) # Çıktı: ["Dawut", "Python", "Gemini"]
```
##### --- REMOVE()--[11.0-11.3]
```PY
11.0 remove() - Değere Göre Silme

11.1 Nedir: Listeden belirli bir elemanın adını (değerini) yazarak silmek için kullanılır.

11.2 Nasıl Kullanılır: Eğer listede aynı isimden iki tane varsa, sadece ilk gördüğünü siler.

11.3 Örnek:
esyalar = ["Defter", "Kalem", "Silgi"]
esyalar.remove("Kalem")
print(esyalar) # Çıktı: ["Defter", "Silgi"]
```
##### --- POP()--[12.0-12.3]
```PY
12.0 pop() - Konuma Göre Silme

12.1 Nedir: Belirli bir indeksteki (sıradaki) elemanı silmek için kullanılır. Eğer parantez içi boş bırakılırsa en sondaki elemanı siler.

12.2 Nasıl Kullanılır: pop(indeks) şeklinde kullanılır. Silinen elemanı sana geri verebilir (bir değişkene atayabilirsin).

12.3 Örnek:
notlar = [85, 90, 100]
notlar.pop(0) # İlk elemanı (85) siler
print(notlar) # Çıktı: [90, 100]
```
##### --- SORT()--[13.0-13.3]
```PY
13.0 .sort() - Listeyi Sıralama

13.1 Nedir: Bir listenin elemanlarını kalıcı olarak belirli bir düzene (küçükten büyüğe veya alfabetik) sokmak için kullanılır.

13.2 Nasıl Kullanılır: liste_adi.sort() şeklinde yazılır. Bu komut listeyi "yerinde" değiştirir, yani listenin orijinal hali artık sıralanmış halidir.

13.3 Örnek:
# Sayılarda kullanım
sayilar = [45, 10, 85, 2]
sayilar.sort()
print(sayilar) # Çıktı: [2, 10, 45, 85]

# Metinlerde kullanım (Alfabetik)
isimler = ["Dawut", "Nurjemal", "Gurban"]
isimler.sort()
print(isimler) # Çıktı: ["Dawut", "Gurban", "Nurjemal"]
```
##### --- SORTED()--[14.0-14.3]
```PY
14.0 sorted() - Geçici Sıralama

14.1 Nedir: Bir listeyi sıralanmış bir kopyasını oluşturmak için kullanılır. Orijinal liste değişmeden kalır. .sort() listeyi kalıcı olarak değiştirirken, sorted() sadece o anlık sıralanmış bir sonuç verir.

14.2 Nasıl Kullanılır: sorted(liste_adi) şeklinde, listenin dışına yazılan bir fonksiyon olarak kullanılır. Genelde sonucu yeni bir değişkene atamak veya print() içinde kullanmak için idealdir.

14.3 Örnek:
rakamlar = [3, 1, 4, 2]

# Geçici olarak sıralı yazdırıyoruz
print(sorted(rakamlar)) # Çıktı: [1, 2, 3, 4]

# Orijinal liste bozulmadı!
print(rakamlar) # Çıktı: [3, 1, 4, 2]
```
##### --- REVERSE()--[15.0-15.3]
```PY
15.0 .reverse() - Listeyi Tersine Çevirme

15.1 Nedir: Bir listenin elemanlarını alfabetik veya sayısal büyüklüğe bakmaksızın, sadece bulundukları sırayı sondan başa doğru kalıcı olarak çevirmek için kullanılır.

15.2 Nasıl Kullanılır: liste_adi.reverse() şeklinde yazılır. Bu bir sıralama işlemi değil, sadece listenin mevcut dizilimini "takla attırma" işlemidir.

15.3 Örnek:
moduller = ["Print", "Input", "Sort"]
moduller.reverse()
print(moduller) # Çıktı: ["Sort", "Input", "Print"]

# Sayılarla örnek (Küçük-büyük bakmaz, sadece ters çevirir)
sayilar = [1, 9, 3, 7]
sayilar.reverse()
print(sayilar) # Çıktı: [7, 3, 9, 1]
```
##### --- (REVERSE = ...)--[16.0-16.7]

```PY
16.0 .sort(reverse = ...) - Sıralama Yönünü Belirleme

16.1 Nedir: .sort() metodunun içine yazılan bu özel komutlar, sıralamanın küçükten büyüğe mi yoksa büyükten küçüğe mi olacağını kontrol eder.

16.2 Nasıl Kullanılır: Parantez içine reverse=True (Doğru) veya reverse=False (Yanlış) yazılarak kullanılır.

16.3 reverse = True (Büyükten Küçüğe): Listeyi tam tersine, yani en büyükten en küçüğe (veya Z'den A'ya) doğru sıralar.

16.4 Örnek:
puanlar = [50, 100, 10, 80]
puanlar.sort(reverse = True)
print(puanlar) # Çıktı: [100, 80, 50, 10]

16.5 reverse = False (Küçükten Büyüğe): Bu Python ın varsayılan (standart) ayarıdır. Eğer parantez içine hiçbir şey yazmazsan Python bunu False kabul eder ve küçükten büyüğe sıralar.

16.6 Örnek:
puanlar = [50, 100, 10, 80]
puanlar.sort(reverse=False) # VEYA sadece puanlar.sort()
print(puanlar) # Çıktı: [10, 50, 80, 100]

16.7 reverse=True/False ayarı sadece sıralama yapan fonksiyonlarda (sort() ve sorted()) kullanılır. Diğer liste komutlarında (append, remove, pop vb.) bu ayar bulunmaz.
```
##### --- MAX()--[17.0-17.3]
```PY
17.0 max() - En Büyük Değeri Bulma

17.1 Nedir: Bir listenin veya sayı grubunun içindeki en büyük (maksimum) değeri bulmak için kullanılır.

17.2 Nasıl Kullanılır: max(liste_adi) şeklinde kullanılır.

17.3 Örnek:
notlar = [85, 95, 70, 100, 80]
en_yuksek = max(notlar)
print(en_yuksek) # Çıktı: 100
```
##### --- MIN()--[18.0-18.3]
```PY
18.0 min() - En Küçük Değeri Bulma

18.1 Nedir: Bir listenin veya sayı grubunun içindeki en küçük (minimum) değeri bulmak için kullanılır.

18.2 Nasıl Kullanılır: min(liste_adi) şeklinde kullanılır.

18.3 Örnek:
sicakliklar = [18, 22, 15, 25, 20]
en_dusuk = min(sicakliklar)
print(en_dusuk) # Çıktı: 15
```
##### --- INDEX()--[19.0-19.2]
```py
19.0 İndeks (Dizin) Nedir: Bir listenin içindeki her bir elemanın sahip olduğu benzersiz "adres numarası"dır. Python'da elemanlara bu numaralar üzerinden ulaşılır.

19.1 Sarsılmaz Kurallar:
1. Python saymaya daima 0'dan başlar. (İlk eleman = 0. İndeks)
2. İndeks numaraları köşeli parantez [ ] ile gösterilir.
3. İndeks, bir elemanın konumudur; Insert veya Pop gibi işlemler bu konumu hedef alır.

19.2 Örnek Mantık:
plan = ["Python", "Matematik", "Almanca"]
# İndeks:  0            1            2

print(plan[0]) # Çıktı: "Python"
```

#### --- [KOSULLU_IFADELER] --- {III-KISIM}
##### --- F-STRING--[25.0-25.4]
```PY
25.0 f-string - Modern Metin Biçimlendirme

25.1 Nedir: Değişkenleri ve işlemleri bir metnin (string) içine en hızlı, en temiz ve en profesyonel şekilde yerleştirme yöntemidir.

25.2 Nasıl Kullanılır: Metnin (tırnağın) en başına f harfi konur. Metin içinde değişkenler süslü parantez { } içine yazılır.

25.3 Örnek:
ad = "Dawut"
hedef = "Avusturya"

# Eski usul (Karmaşık)
print("Merhaba " + ad + ", hedefin " + hedef)

# f-string usulü (Temiz ve Mühendisçe)
print(f"Merhaba {ad}, hedefin {hedef}")

25.4 İşlem Yapma Özelliği:
hizlar = [100, 150]
print(f"En yüksek hız: {max(hizlar)}") # Parantez içinde fonksiyon çalışabilir
```
##### --- IF ELIF ELSE NESTED IF
###### --- IF ---
```PY
26.0 if - "Eğer" Kontrolü

26.1 Nedir: Programın bir karara varmasını sağlar. Belirli bir şart doğruysa (True) o kod bloğunu çalıştırır.

26.2 Kurallar:
1. if kelimesinden sonra şart yazılır.
2. Şartın sonuna mutlaka : (iki nokta) konur.
3. Bir sonraki satır mutlaka "indent" (4 boşluk/tab) içeriden başlar. (Python'ın blok mantığı).

26.3 Örnek:
yas = 16
if yas >= 16:
    print("Mühendislik eğitimi için yaşın uygun.")
```
###### --- ELIF ---
```PY
26.4 elif - "Yok Eğer Şöyleyse" (Çoklu Karar)

26.5 Nedir: Birden fazla şartı kontrol etmek gerektiğinde kullanılır. if başarısız olursa elif kontrol edilir.

26.6 Kurallar:
1. if ve else arasında sınırsız sayıda elif kullanılabilir.
2. İlk sağlanan elif şartı çalışır, diğerleri atlanır.

26.7 Örnek:
notun = 95
if notun >= 90:
    print("Notun: A (Mükemmel)")
elif notun >= 70:
    print("Notun: B (İyi)")
else:
    print("Notun: C (Daha çok çalışmalısın)")
```
###### --- ELSE ---
```PY
26.8 else - "Değilse" Durumu

26.9 Nedir: if ile belirtilen şart sağlanmadığında (False olduğunda) otomatik olarak devreye giren "B planı"dır.

26.9.1 Kurallar:
1. else tek başına yazılamaz, mutlaka bir if bloğundan sonra gelir.
2. else yanına şart yazılmaz; sadece : konur.

26.9.2 Örnek:
hiz = 120
if hiz > 130:
    print("Hız sınırı aşıldı! Ceza kesiliyor.")
else:
    print("Hızınız normal, iyi yolculuklar.")
```
###### --- NESTED IF ---
```PY
26.9.3 Nested If - İç İçe Geçmiş "Eğer"

26.9.4 Nedir: Bir if bloğunun içine yazılan ikinci (veya üçüncü) bir if yapısıdır. İçerideki if'in kontrol edilmesi için dışarıdaki if'in mutlaka doğru (True) olması gerekir.

26.9.5 Kurallar:
1. İçerideki if, dışarıdaki if'in "indent" (4 boşluk) hizasından daha içeride (toplam 8 boşluk) başlar.
2. Girinti (boşluk) seviyesi Python'da hangi kararın hangisine bağlı olduğunu belirler.

26.9.6 Örnek:
pasaport = True
vize = True

if pasaport == True:
    print("Pasaport kontrolü başarılı.")
    if vize == True:
        print("Vize de onaylı. Avusturya'ya giriş yapabilirsiniz!")
    else:
        print("Pasaport var ama vize yok. Giriş reddedildi.")
else:
    print("Pasaport yok. Sınırdan geçemezsiniz.")
```
##### --- AND OR NOT--[27.0-27.9]
###### --- AND ---
```py
27.0 and - "Ve" Bağlacı

27.1 Nedir: İki veya daha fazla şartın "hepsinin birden" doğru (True) olmasını bekler. Eğer şartlardan biri bile yanlışsa, sonuç yanlıştır.

27.2 Kullanım Mantığı: 
Şart 1  |  Şart 2  |  SONUÇ
True    |  True    |  True (Çalışır)
True    |  False   |  False (Çalışmaz)

27.3 Örnek:
kullanici_adi = "Dawut"
sifre = "1234"

if kullanici_adi == "Dawut" and sifre == "1234":
    print("Sisteme giriş başarılı.")
else:
    print("Kullanıcı adı veya şifre hatalı.")
```
###### --- OR ---
```PY
27.4 or - "Veya" Bağlacı

27.5 Nedir: Şartlardan "en az birinin" doğru olmasını yeterli bulur. Sadece tüm şartlar yanlışsa sonuç yanlış (False) çıkar.

27.6 Kullanım Mantığı:
Şart 1  |  Şart 2  |  SONUÇ
True    |  False   |  True (Çalışır)
False   |  True    |  True (Çalışır)
False   |  False   |  False (Çalışmaz)

27.7 Örnek:
hava_durumu = "Yagmurlu"
enerji = "Dusuk"

if hava_durumu == "Gunesli" or enerji == "Yuksek":
    print("Dışarı çıkıp spor yapabilirsin.")
else:
    print("Evde kalıp Python çalışmaya devam!")
```
###### --- NOT ---
```py
27.8 not - "Değil" (Tersine Çevirme)

27.9 Nedir: Bir şartın sonucunu tam tersine çevirir. True ise False yapar, False ise True yapar.

27.9.1 Kullanım Mantığı:
İşlem: not True  -> Sonuç: False
İşlem: not False -> Sonuç: True

27.9.2 Örnek:
ehliyet_var_mi = False

if not ehliyet_var_mi:
    print("Araç kullanamazsın, önce ehliyet almalısın.")
```
##### --- KARSILASTIRMA_OPERATORLERI
```PY
28.0 == (Eşit mi?): İki değerin birbirinin aynısı olup olmadığını kontrol eder.
     Örnek: 5 == 5 -> True | 5 == 3 -> False

28.2 != (Eşit değil mi?): İki değerin birbirinden farklı olup olmadığını kontrol eder.
     Örnek: 5 != 3 -> True | 5 != 5 -> False

28.3 > (Büyüktür): Soldaki sayının sağdakinden büyük olup olmadığına bakar.
     Örnek: 10 > 5 -> True 

28.4 < (Küçüktür): Soldaki sayının sağdakinden küçük olup olmadığına bakar.
     Örnek: 5 < 10 -> True

28.5 >= (Büyük veya Eşit): Sayı hem büyük hem de eşitse True döner.
     Örnek: 10 >= 10 -> True | 11 >= 10 -> True

28.6 <= (Küçük veya Eşit): Sayı hem küçük hem de eşitse True döner.
     Örnek: 5 <= 5 -> True | 4 <= 5 -> True

28.7 Önemli Uyarı: "=" işareti değer atamak için kullanılır (x = 5), 
     "==" işareti ise soru sormak/kontrol etmek içindir (x == 5).
``` 

#### --- [DONGULER] --- {IV-KISIM}
##### --- FOR IN RANGE--[29.0-29.9]
###### --- FOR ---
```py
29.0 for - "Tekrar" Döngüsü

29.1 Nedir: Belirli bir veri grubundaki (liste, metin, sayı aralığı) her bir öğe için kodun tekrar tekrar çalıştırılmasını sağlar. "Her biri için şunu yap" demektir.

29.2 Kurallar:

for kelimesinden sonra bir değişken adı yazılır (bu değişken, her adımda sıradaki öğeyi temsil eder).

in anahtar kelimesiyle döngünün hangi veri üzerinde döneceği belirtilir.

Satır sonuna : (iki nokta) konur ve alt satır içeriden (indent) başlar.

29.3 Örnek:
diller = ["Python", "Java", "SQL"]

for dil in diller:
    print(dil + " öğrenerek backend yolunda ilerliyorum.")
```
###### --- IN ---
```py
29.4 in - "İçinde mi?" ve "Üyelik" Kontrolü

29.5 Nedir: Python'da iki temel görevi vardır. Birincisi, for döngüsünde bir veri grubunun içinde gezinmeyi sağlar. İkincisi ise, bir öğenin bir grubun (liste, metin, set) parçası olup olmadığını kontrol eder.

29.6 Görevleri:

Döngü Kurucu: Bir koleksiyonun (liste vb.) başından sonuna kadar her elemanı sırayla yakalar.

Sorgulayıcı: Bir eleman o grubun içinde varsa True, yoksa False değerini döndürür.

29.7 Örnek:
# 1. Kullanım: Döngü içinde (Gezinme)
hedef_ulkeler = ["Almanya", "Avusturya"]
for ulke in hedef_ulkeler:
    print(ulke + " hedefim için çalışıyorum.") [cite: 2026-01-03]

# 2. Kullanım: Şart içinde (Kontrol)
yetenekler = ["Python", "SQL", "Algorithm"]
if "Python" in yetenekler:
    print("Backend için doğru yoldasın.") [cite: 2026-02-11]
```
######  --- RANGE ---
```PY
29.8 range() - "Aralık" Fonksiyonu

29.9.1 Nedir: Belirli bir başlangıç noktasından bitiş noktasına kadar sayı dizileri üretir. Elle liste yazmak yerine, bilgisayara "1'den 100'e kadar say" demeni sağlar.

29.9.2 Kurallar:

Tek parametre: range(5) yazarsan 0'dan başlar, 5'e kadar gider (5 dahil değildir).

İki parametre: range(2, 6) yazarsan 2'den başlar, 6'ya kadar gider (6 dahil değildir).

Üç parametre: range(1, 10, 2) yazarsan 1'den başlar, 10'a kadar ikişer ikişer atlayarak gider.

29.9.3 Örnek:
# 0'dan 4'e kadar (toplam 5 kez) çalışır
for i in range(5):
    print(f"{i}. adım: Disiplin başarı getirir.") [cite: 2026-01-25]

# 10'dan 100'e kadar 10'ar 10'ar sayar
for puan in range(10, 101, 10):
    print(f"IQ Test Puanı: {puan}") [cite: 2026-01-25]
```
##### --- DIYM VE AAO--[30.0-30.7]
###### --- DONGU YAPILARI VE ISIMLENDIRME MANTIGI ---
```PY
30.0 for x in y: vs for x in range(y):
30.1 Nedir: Bu iki yapı arasındaki temel fark, birinin var olan bir grubun (liste, metin vb.) elemanları üzerinde gezmesi, diğerinin ise belirli bir sayıda (sayısal aralık) dönmesidir.

30.2 Karşılaştırma ve İsimlendirme:

for x in y: (Eleman Odaklı): y burada bir listedir (örneğin: sehirler). x ise o anki elemandır.

İsimlendirme Tavsiyesi: x yerine elemanı tanımlayan bir isim seç (örneğin: for sehir in sehirler:).

for x in range(y): (Sayı Odaklı): Burada döngü y kadar tekrar eder. x burada bir sayıdır (indeks).

İsimlendirme Tavsiyesi: Genelde matematiksel bir sayaç olduğu için i, j veya sayac gibi kısa isimler kullanılır.

30.3 Örnek ve Mantık:
# 1. Mevcut bir liste üzerinde gezmek (Eleman odaklı)
dersler = ["Matematik", "IQ", "Geometri"]
for ders in dersler:
    print(f"Bugün {ders} çalışılacak.") [cite: 2026-01-26]

# 2. Belirli sayıda tekrar yapmak (Sayı odaklı)
for i in range(3):
    print(f"{i+1}. kod denemesi başarılı.")
```
###### --- ARTIRILMI ATAMA OPERATORLERI---
```PY
30.4 Atama ve Artırma Operatörleri

30.5 Nedir: Bir değişkenin değerini mevcut değerinin üzerine bir işlem yaparak güncellemenin kısa yollarıdır. Özellikle döngü sayaçlarında ve toplam alma işlemlerinde kullanılır.

30.6 Operatörler ve Mantığı:
Operatör,Uzun Yazım,Kısa (Profesyonel) Yazım,Kullanım Amacı
Toplama,x = x + y,x += y,Değeri y kadar artırır. (En çok kullanılan budur).
Çıkarma,x = x - y,x -= y,Değeri y kadar azaltır. (Geri sayımlar için).
Çarpma,x = x * y,x *= y,Değeri y katına çıkarır.
Bölme,x = x / y,x /= y,Değeri y'ye böler.

30.7 Döngü İçinde Pratik Örnek:
toplam_calisma = 0
gunluk_saat = 2

# 5 gün boyunca toplam saati artırıyoruz
for gun in range(5):
    toplam_calisma += gunluk_saat # Her adımda 2 ekler
    print(f"{gun+1}. gün sonunda toplam: {toplam_calisma} saat") [cite: 2026-01-28]
```
##### --- WHILE--[31.0-31.3]
```PY
31.0 while - "Şartlı Tekrar" Döngüsü
31.1 Nedir: Bir şart True (doğru) olduğu sürece kod bloğunu tekrar tekrar çalıştıran döngü yapısıdır. "Şu durum devam ettiği sürece, bu işi yapmaya devam et" demektir.

31.2 Kurallar:

while kelimesinden sonra bir mantıksal şart yazılır.

Şartın sonuna : (iki nokta) konur.

Döngü içindeki kodlar mutlaka indent (içeriden) başlar.

Kritik Kural: Döngünün bir noktada bitmesi için şartı bozan bir güncelleme (sayaç artırma vb.) yapılmalıdır; aksi takdirde "sonsuz döngüye" girer.

31.3 Örnek:
# Basit bir sayaç örneği
deneme_hakki = 3

while deneme_hakki > 0:
    print(f"Sisteme giriş yapılıyor... Kalan hak: {deneme_hakki}")
    deneme_hakki -= 1  # Öğrendiğin artırımlı atama!

print("Giriş hakkınız doldu.")
```
##### --- CONTINUE BREAK--[32.0-32.7]
###### --- CONTINUE ---
```PY
32.0 continue - "Pas Geç" Komutu
32.1 Nedir: Döngü içinde bu komutla karşılaşıldığında, altındaki kodlar çalıştırılmaz ve döngü anında bir sonraki adıma (başa) döner. "Bu seferlik bunu atla ama devam et" demektir.

32.2 Kurallar:

Genellikle bir if şartı ile birlikte kullanılır.

continue çalıştığı anda o tur biter; döngü tamamen durmaz, sadece o turdaki kalan işlemler iptal edilir.

32.3 Örnek:
# Sadece tek sayıları yazdırmak için çiftleri pas geçiyoruz
for sayi in range(1, 6):
    if sayi % 2 == 0:
        continue # Çift sayıyı gördüğün an alt satırı okuma, başa dön!
    print(f"Sayı: {sayi} (Tek olduğu için işleme alındı)")
```
###### --- BREAK ---
```PY
32.4 break - "Döngüyü Kır" Komutu
32.5 Nedir: Döngü hangi aşamada olursa olsun, break komutu görüldüğü anda döngü tamamen durdurulur ve döngüden çıkılır. Döngünün geri kalan turları asla çalışmaz.

32.6 Kurallar:

Genellikle bir if şartı (arama, hata veya çıkış şartı) ile birlikte kullanılır.

break çalıştığı anda program döngü bloğunun dışındaki ilk satıra atlar.

32.7 Örnek:
```
##### --- NESTED FOR NESTED IF--[33.0-33.7]
###### --- NESTED FOR ---
```PY
33.0 Nested Loops (İç İçe Döngüler)
33.1 Nedir: Bir döngü bloğunun içerisinde ikinci bir döngünün yer almasıdır. Dıştaki döngünün her bir adımı için, içteki döngü baştan sona tüm turlarını tamamlar.

33.2 Kurallar:

İçteki döngü mutlaka dıştaki döngünün "indent" (4 boşluk) içinde olmalıdır.

İçteki döngü bittikten sonra dıştaki döngü bir sonraki adımına geçer.

Değişken isimleri karışmaması için genelde dıştakine i, içtekine j denir (matematiksel standart).

33.3 Nested for (İç İçe For)
Genellikle koordinat sistemleri, tablolar veya listelerin içindeki listeleri (matris) işlemek için kullanılır.

Örnek (Koordinat Sistemi):
for satir in range(1, 3): # Dış döngü 2 kez döner
    for sutun in range(1, 4): # İç döngü, her satır için 3 kez döner
        print(f"Konum: ({satir}, {sutun})")
```
###### --- NESTED WHILE ---
```PY
33.4 Nested while (İç İçe While)
33.5 Nedir: Bir while döngüsünün içerisinde başka bir while döngüsünün çalışmasıdır. Koşula bağlı süreçlerin içinde, başka alt koşulların da kontrol edilmesi gereken durumlarda kullanılır.

33.6 Kurallar:

İç Sayaç Yönetimi: İçteki döngünün sayacı, genellikle dıştaki döngünün her adımında tekrar sıfırlanmalıdır (başlangıç değerine döndürülmelidir).

Çifte İlerleme: Hem içteki hem de dıştaki döngünün durabilmesi için her iki sayacın da kendi blokları içinde artırılması (+= 1) zorunludur.

Bağımsız Şartlar: İçteki while kendi şartı bozulana kadar döner, o bitince dıştaki while bir sonraki adıma geçer.

33.7 Örnek (Antrenman Programı):
set_sayisi = 1

while set_sayisi <= 3: # Dış döngü: 3 set boyunca döner
    print(f"--- {set_sayisi}. Set Başladı ---")
    
    tekrar = 1 # İç sayaç: Her set başında 1'den başlar
    while tekrar <= 5: # İç döngü: Her sette 5 tekrar yapar
        print(f"Tekrar: {tekrar}")
        tekrar += 1 # İç sayacı artır
        
    print(f"--- {set_sayisi}. Set Bitti ---\n")
    set_sayisi += 1 # Dış sayacı artır
```

#### --- [SOZLUKLER] --- {V-KISIM}
##### --- KEY-VALUE AND F-SHRING--[35.0-35.8]
```PY
35.0 Dictionaries (Sözlükler)
35.1 Nedir: Verileri Key-Value (Anahtar-Değer) çiftleri şeklinde tutan, sırasız ama çok hızlı çalışan bir veri yapısıdır. Gerçek bir sözlükte nasıl bir "kelime" ve onun "anlamı" varsa, Python sözlüklerinde de bir "anahtar" ve ona karşılık gelen "değer" vardır.

35.2 Temel Kurallar:

Süslü parantez {} ile tanımlanır.

Anahtar ve değer arasında : (iki nokta) kullanılır.

Her çift birbirinden , (virgül) ile ayrılır.

Kritik: Anahtarlar (keys) benzersiz (unique) olmalıdır.

35.3 Örnek (Kullanıcı Profil Kartı):
# Bir yazılımcı profili oluşturalım
yazilimci = {
    "isim": "Dawut",
    "yas": 16,
    "hedef": "Backend Developer",
    "diller": ["Python", "German"]
}

# Veriye erişim
print(yazilimci["isim"]) # Çıktı: Dawut

35.4 Sozluklerde islem

İşlem,Kod Yazımı,Açıklama
Ekleme/Güncelleme,"yazilimci[""sehir""] = ""Berlin""","Yeni anahtar yoksa ekler, varsa günceller."
Silme,"del yazilimci[""yas""]",Belirtilen anahtarı ve değerini siler.
Kontrol,"""hedef"" in yazilimci",Anahtarın sözlükte olup olmadığını sorgular (True/False).
```
###### --- KV F-SHRING ---
```PY
35.5 Sözlüklerde f-string Kullanımı
35.6 Nedir: Sözlük içerisindeki değerleri (values), süslü parantezler {} aracılığıyla doğrudan metin içerisine gömme yöntemidir.

35.7 Kritik Yazım Kuralı (Tırnak İşareti Disiplini):
f-string içinde sözlük anahtarı çağırırken en büyük hata tırnak işaretlerini karıştırmaktır.

Eğer f-string'i çift tırnak f"..." ile başlattıysan, anahtarı tek tırnak ['anahtar'] ile yazmalısın.

Bunun tersi de geçerlidir: f'...["anahtar"]...'

35.8 Örnek Senaryo (Sistem Raporu):
# Veri tabanından gelen bir sözlük gibi düşün
sunucu_durumu = {
    "ip": "192.168.1.1",
    "islemci_yuk": 45,
    "aktif_mi": True
}

# f-string ile raporlama
rapor = f"Sunucu IP: {sunucu_durumu['ip']} | Yük: %{sunucu_durumu['islemci_yuk']}"
print(rapor)

# Şartlı f-string kullanımı
durum_metni = "Aktif" if sunucu_durumu["aktif_mi"] else "Devre Dışı"
print(f"Sistem Durumu: {durum_metni}")
```
##### --- DEL POP GET--[36.0-36.9]
###### --- DEL ---
```PY
36.0 Sözlüklerde Veri Silme: del
36.1 Nedir: del (delete), bir sözlükteki belirli bir anahtarı ve ona bağlı olan değeri kalıcı olarak bellekten siler.

36.2 Kurallar:

del sozluk_adi["anahtar"] şeklinde kullanılır.

Kritik Uyarı: Eğer sözlükte olmayan bir anahtarı silmeye çalışırsan Python KeyError hatası verir ve program durur. Bu yüzden silme işleminden önce anahtarın varlığından emin olmalısın.

36.3 f-string ile Gelişmiş Örnek:
# Bir kullanıcı veri tabanı örneği
kullanici = {
    "id": 101,
    "kullanici_adi": "Dawut_Dev",
    "gecici_kod": "123456", # Bu silinecek
    "durum": "Aktif"
}

print(f"Sistem: {kullanici['kullanici_adi']} için güvenlik taraması başlıyor...")

# Hassas veriyi silme işlemi
del kullanici["gecici_kod"]

# Kontrol çıktısı
print(f"İşlem Tamam: Gecici kod silindi. Güncel veriler: {kullanici}")

36.4 Temizleme İşlemi (clear)
Eğer sözlüğün içindeki tek bir anahtarı değil de, tüm içeriği bir kerede boşaltmak istersen (sözlüğün kendisi kalsın ama içi boş olsun), şu komutu kullanırsın:
kullanici.clear()
print(f"Sözlük temizlendi mi? Liste: {kullanici}") # Çıktı: {}
```
###### --- POP ---
```PY
36.5 Sözlüklerde .pop() Metodu
36.6 Nedir: Belirtilen bir anahtarı (key) sözlükten çıkarır ve o anahtara ait olan değeri (value) geri döndürür. Yani sildiğin şeyi bir değişkene atayıp kullanabilirsin.

36.7 Kurallar:

sozluk.pop("anahtar") şeklinde yazılır.

Hata Önleme: Eğer sözlükte olmayan bir anahtarı silmeye çalışırsan Python hata verir. Bunu engellemek için ikinci bir parametre (varsayılan değer) ekleyebilirsin: sozluk.pop("anahtar", "Bulunamadı").

36.8 Uygulamalı Örnek:
kullanici = {
    "isim": "Dawut",
    "rutbe": "Admin",
    "gecici_kod": "ABC-123"
}

# Veriyi hem silip hem de bir değişkene alıyoruz
silinen_kod = kullanici.pop("gecici_kod")

print(f"Sistem: {silinen_kod} kodlu veri güvenlik amacıyla silindi.")
print(f"Güncel Kullanıcı Verisi: {kullanici}")

# Olmayan bir veriyi silmeye çalışırken hata almamak için:
not_bilgisi = kullanici.pop("notlar", "Böyle bir veri zaten yok")
print(f"İşlem Sonucu: {not_bilgisi}")
```
###### --- GET ---
```PY
36.9.A Sözlüklerde .get() Metodu
36.9.B Nedir: Bir sözlükten belirtilen anahtara ait değeri çekmeye yarar. Normal köşeli parantez yönteminden farkı, aranan anahtar sözlükte yoksa programın çökmesini (KeyError) engellemesidir.

36.9.C Kurallar:

sozluk.get("anahtar") şeklinde kullanılır. Anahtar bulunamazsa hata vermez, geriye None (boş) döner.

Varsayılan Değer: Eğer anahtar yoksa None yerine kendi belirlediğin bir mesajın dönmesini sağlayabilirsin: sozluk.get("anahtar", "Varsayılan Mesaj").

36.9.D Uygulamalı Örnek:
ayarlar = {
    "dil": "Almanca",
    "tema": "Koyu"
}

# 1. Mevcut bir veriyi çekme
mevcut_dil = ayarlar.get("dil")
print(f"Sistem Dili: {mevcut_dil}")

# 2. Olmayan bir veriyi çekme (HATA VERMEZ)
konum = ayarlar.get("sehir")
print(f"Konum Bilgisi: {konum}") # Çıktı: None

# 3. f-string ile Varsayılan Değer atayarak çekme
kullanici_adi = ayarlar.get("isim", "Misafir Kullanıcı")
print(f"Hoş geldin, {kullanici_adi}!")
```
##### --- SOZLUK YONETIMI (EKLEME VE SORGULAMA)--[37.0-37.3]
```PY
37.0 Sözlük Yönetimi (Ekleme ve Sorgulama)
37.1 Ekleme ve Güncelleme:
Python'da sözlüğe yeni bir veri eklemek ile mevcut bir veriyi değiştirmek için aynı yöntem kullanılır.

Eğer köşeli parantez içine yazdığın anahtar sözlükte yoksa, yeni bir kayıt oluşturulur.

Eğer o anahtar zaten varsa, eski değer silinir ve üzerine yenisi yazılır.

37.2 Varlık Kontrolü (in Operatörü):
Bir sözlükten veri çekmeye çalışmadan önce, o anahtarın sözlükte olup olmadığını kontrol etmek sistemin hata verip çökmesini engeller. Bu işlem True veya False değer döner.

37.3 Uygulamalı Örnek:
yazilimci = {
    "isim": "Dawut",
    "hedef": "Backend"
}

# 1. EKLEME: Sözlükte olmayan bir anahtar ekleyelim
yazilimci["sehir"] = "Berlin" 
print(f"Ekleme Sonrası: {yazilimci['isim']} artık {yazilimci['sehir']} şehrinde.")

# 2. GÜNCELLEME: Mevcut bir anahtarın değerini değiştirelim
yazilimci["hedef"] = "Senior Backend Developer"
print(f"Güncelleme Sonrası Yeni Hedef: {yazilimci['hedef']}")

# 3. KONTROL: Anahtar sözlükte mi?
if "yas" in yazilimci:
    print(f"Yaş Bilgisi: {yazilimci['yas']}")
else:
    print("Uyarı: Sözlükte yaş bilgisi bulunamadı!")

# f-string içinde doğrudan kontrol kullanımı
print(f"Uzmanlık bilgisi var mı?: {'hedef' in yazilimci}")
```
##### --- UPDATE() CLEAR()--[38.0-38.7]
###### --- UPDATE()
```PY
38.0 Sözlüklerde .update() Metodu
38.1 Nedir: Bir sözlüğe başka bir sözlüğü veya anahtar-değer çiftlerinden oluşan bir grubu (tuple gibi) tek seferde ekleme işlemidir.

38.2 Kurallar:

sozluk.update({"anahtar": "deger"}) şeklinde kullanılır.

Toplu İşlem: Birden fazla veriyi tek satırda güncelleyebilirsin.

Üstüne Yazma: Eğer eklemeye çalıştığın anahtar zaten sözlükte varsa, eski değer silinir ve yeni değer onun yerini alır.

38.3 Uygulamalı Örnek (Terminal Güvenlik Güncellemesi):
# Mevcut terminal durumu
terminal_verisi = {
    "bolge": "Terminal-A",
    "guvenlik_seviyesi": "Orta",
    "aktif_personel": 5
}

print(f"Sistem Baslatiliyor... Mevcut Durum: {terminal_verisi['guvenlik_seviyesi']}")

# Birden fazla veriyi ayni anda guncelleme (update)
terminal_verisi.update({
    "guvenlik_seviyesi": "Yüksek", # Guncellendi
    "ek_onlem": "Lazer bariyerler", # Yeni eklendi
    "aktif_personel": 12            # Guncellendi
})

print(f"\n--- GÜNCELLEME TAMAMLANDI ---")
print(f"Yeni Seviye: {terminal_verisi['guvenlik_seviyesi']}")
print(f"Ek Onlem: {terminal_verisi['ek_onlem']}")
print(f"Toplam Personel: {terminal_verisi['aktif_personel']}")
```
###### --- CLEAR() ---
```PY
38.4 Sözlüklerde .clear() Metodu
38.5 Nedir: Bir sözlüğün içindeki tüm verileri silerek sözlüğü tamamen boş hale getiren metottur.

38.6 Kurallar:

sozluk.clear() şeklinde kullanılır.

Sonuç: İşlemden sonra sözlük {} (boş sözlük) haline gelir.

del ile Farkı: del sozluk dersen sözlük değişkeni tamamen yok olur ve ona bir daha erişemezsin (hata alırsın). Ancak .clear() dersen sözlük "boş bir kutu" olarak kalmaya devam eder, içine tekrar veri ekleyebilirsin.

38.7 Uygulamalı Örnek (Kanıt Temizleme Senaryosu):
kanitlar = {
    "lokasyon": "Depo-7",
    "parmak_izi": "Bulundu",
    "dosya_no": 9982
}

print(f"Baskın Öncesi Kanıt Sayısı: {len(kanitlar)}")

# Tüm verileri tek seferde temizle
kanitlar.clear()

print("--- SISTEM SIFIRLANDI ---")
print(f"Mevcut Kanıt Durumu: {kanitlar}") # Çıktı: {}

# Sözlük hala yaşıyor, yeni veri ekleyebiliriz
kanitlar["durum"] = "Temiz"
print(f"Yeni Kayıt: {kanitlar}")
```
##### --- NESTED DICTIONARIES{SOZLUKLER}--[39.0-39.4]
```PY
39.0 Nested Dictionaries (İç İçe Sözlükler)
39.1 Nedir: Bir sözlüğün içindeki bir "anahtarın" (key), değer (value) olarak başka bir sözlüğü tutmasıdır. Bu yapı, verileri kategorize etmek ve hiyerarşik bir düzen kurmak için kullanılır.

39.2 Kurallar:

Derinlik: İstediğin kadar iç içe sözlük açabilirsin (sözlük içinde sözlük, onun içinde başka bir sözlük...).

Erişim: İçteki verilere ulaşmak için ardı ardına köşeli parantez [][] kullanılır.

Benzersizlik: Her seviyedeki anahtarlar kendi içinde benzersiz olmalıdır.

39.3 Uygulamalı Örnek (Backend Kullanıcı Yönetimi):
# Bir yazılım şirketindeki çalışanların veritabanı gibi düşün
sirket = {
    "calisan_1": {
        "ad": "Dawut",
        "rol": "Backend Developer",
        "diller": ["Python", "Java"]
    },
    "calisan_2": {
        "ad": "Jessie",
        "rol": "DevOps",
        "diller": ["Go", "Docker"]
    }
}

# 1. Veriye Erişme
print(f"1. Çalışan Adı: {sirket['calisan_1']['ad']}") # Çıktı: Dawut

# 2. Veri Güncelleme
sirket["calisan_2"]["rol"] = "Senior DevOps"

# 3. Yeni İç Sözlük Ekleme
sirket["calisan_3"] = {"ad": "Walter", "rol": "Architect"}

print(f"Güncel Rapor: {sirket['calisan_2']['ad']} artık bir {sirket['calisan_2']['rol']}.")

39.4 İç İçe Sözlüklerde İşlemler ve f-string
İç içe yapılarda f-string kullanırken tırnak işaretlerine ekstra dikkat etmeli
İşlem,Kod Yazımı,Açıklama
Derin Erişim,"sozluk[""dis""][""ic""]",Katman katman içeri girer.
Güvenli Erişim,"sozluk.get(""dis"").get(""ic"")",Dıştaki anahtar yoksa hata vermez.
Silme,"del sozluk[""dis""][""ic""]",Sadece içteki belirli bir veriyi siler.
```
##### --- LIST[] DICTIONARIES[SOZLUKLER]--[40.0-40.4]
```PY
40.0 List of Dictionaries (Liste İçinde Sözlükler)
40.1 Nedir: Birden fazla sözlük objesinin tek bir liste ([]) içerisinde toplanmasıdır. Bu yapı, aynı özelliklere sahip (ad, para, id vb.) birden fazla varlığı (yolcular, ürünler, öğrenciler) yönetmek için kullanılır.

40.2 Temel Avantajları:

Düzen: Her sözlük tek bir kişiyi temsil eder.

Dinamiklik: append() ile yeni bir sözlük (kişi) eklenebilir.

Analiz: for döngüsü ile tüm liste taranıp şartlı işlemler (if-else) yapılabilir.

40.3 Uygulamalı Örnek (Karakter Veritabanı):
# 1. Başlangıç Listesi
yolcular = [
    {"isim": "Mike", "para": 10000}
]

# 2. Yeni Kayıtlar Ekleme (Backend Simülasyonu)
yolcular.append({"isim": "Gus", "para": 50000}) 
yolcular.append({"isim": "Walter", "para": 22000})

# 3. Veri Analizi ve Raporlama
print("--- GÜVENLİK SORGULAMASI BAŞLADI ---")

for yolcu in yolcular:
    # İç içe tırnak kuralına dikkat! (Dışta çift, içte tek)
    if yolcu["para"] >= 30000:
        print(f"BİLDİRİM: {yolcu['isim']} yüksek risk grubunda! (Bakiye: {yolcu['para']})")
    else:
        print(f"BİLDİRİM: {yolcu['isim']} bakiyesi normal seviyede. (Bakiye: {yolcu['para']})")

40.4 Veri Erişimi ve Manipülasyon Tablosu
Listenin içindeki sözlüklere ulaşmak için önce indeks, sonra anahtar kullanılır.
İşlem,Örnek Kod,Açıklama
İlk Kişiye Ulaşma,yolcular[0],Listenin ilk elemanı olan sözlüğü verir.
İçeriğe Ulaşma,"yolcular[1][""isim""]",2. kişinin ismine ulaşır (Gus).
Veri Değiştirme,"yolcular[2][""para""] += 500",Walter'ın parasına 500 ekler.
Yeni Kişi Ekleme,yolcular.append({...}),Listenin sonuna yeni bir sözlük ekler.
```



#### --- [FONKSIYONLAR] --- {VI-KISIM}
##### --- DEF--[41.0-41.3]
```PY
41.0 Fonksiyonlar (Def: Define)
41.1 Nedir: Belirli bir işi yapmak üzere bir araya getirilmiş kod bloklarıdır. Bir fonksiyonu bir kez yazarsın, sonra ihtiyaç duydukça binlerce kez çağırırsın. Bu, yazılımda "DRY" (Don't Repeat Yourself - Kendini Tekrar Etme) prensibinin temelidir.

41.2 Kurallar:

Tanımlama: def anahtar kelimesi ile başlar.

İsimlendirme: Fonksiyon isimleri küçük harfle başlar ve ne işe yaradığı belli olmalıdır (hesapla, kaydet, gonder).

Parametreler: Parantez () içine, fonksiyonun çalışması için gereken dış bilgileri (değişkenleri) yazarsın.

Çağırma: Tanımlanan fonksiyonu kullanmak için fonksiyon_adi() şeklinde çağırmalısın.

41.3 Uygulamalı Örnek (Operasyonel Fonksiyon):
# Fonksiyonu tanımlıyoruz (Sadece tarif)
def rapor_yazdir(isim, miktar):
    print(f"[RAPOR] {isim} adlı kişi tarafından {miktar} miktar madde işlendi.")

# Fonksiyonu çağırıyoruz (Tarifi uyguluyoruz)
rapor_yazdir("Walter", 50000)
rapor_yazdir("Gale", 12000)
```
Bölüm,Görev
def,Fonksiyonu başlatır.
parantez(),Dışarıdan gelecek verileri (parametre) bekler.
:,Fonksiyon gövdesini başlatır.
indentation,Fonksiyona ait kodlar içe (4 boşluk) yazılır.
##### --- RETURN--[42.0-42.3]
```PY
42.0 Fonksiyonlarda return
42.1 Nedir: Bir fonksiyonun çalışması bittikten sonra, çağıran yere bir değer (cevap) göndermesidir. Fonksiyon bir fabrikaysa, return o fabrikanın ürettiği nihai üründür.

42.2 Kurallar:

Fonksiyonu Bitirir: Bir fonksiyonda return satırı çalıştığı anda fonksiyon o saniyede durur; altındaki kodlar okunmaz.

Değeri Yakalama: return ile gelen cevabı bir değişkene eşitleyebilirsin.

Çoklu Kullanım: Bir fonksiyon içinde birden fazla return olabilir (genellikle if-else yapılarında), ancak sadece bir tanesi çalışır.

42.3 Uygulamalı Örnek (Komisyon Hesaplama):
def net_kazanc_hesapla(toplam_para, komisyon_orani):
    kesinti = toplam_para * (komisyon_orani / 100)
    net_tutar = toplam_para - kesinti
    return net_tutar # Sonucu paketleyip dışarı gönderiyoruz

# Fonksiyonu çağır ve dönen cevabı bir değişkene ata
saul_kazanci = net_kazanc_hesapla(10000, 20) 

print(f"Saul'un eline geçen net para: {saul_kazanci}") 
# Eğer print kullansaydık bu veriyi başka bir hesaplamada kullanamazdık.
Özellik,print(),return
Amaç,Sadece ekranda bilgi göstermek.,Bir değeri hafızada tutmak/iletmek.
Etki,Programın geri kalanını etkilemez.,Programın akışında veri olarak kullanılır.
Süreklilik,Veri ekranda kalır ama uçup gider.,Veri bir değişkene atanabilir.
```
##### --- RETURN VS PRINT--[43.0-43.4]
```PY
43.0 print() vs return: Büyük Karşılaştırma
43.1 print() (Sadece Gösteri):

Nedir: Veriyi sadece terminale (ekrana) yazdırır.

Ömrü: Ekranda göründüğü an biter. Program o veriyi hafızasında tutmaz.

Kullanım Amacı: Yazılımcının kodun o an ne yaptığını görmesi (debugging) içindir.

Benzetme: Bir garsonun siparişi mutfağa söylemek yerine sadece müşteriye "Yemeğiniz hazırlanıyor" demesi gibidir. Mutfak (programın kalanı) hala ne piştiğini bilmez.

43.2 return (Veri Paketleme):

Nedir: Fonksiyonun ürettiği sonucu "elimize" verir.

Ömrü: Veri bir değişkene atanırsa program sonlanana kadar yaşar.

Kullanım Amacı: Fonksiyondan çıkan sonucu başka bir hesaplamada veya bir listede kullanmak içindir.

Benzetme: Bir aşçının yemeği paketleyip garsona vermesi gibidir. Artık o paketlenmiş yemek (veri) istenilen masaya (değişkene) götürülebilir.

43.3 Uygulamalı Senaryo (Laboratuvar Örneği)
Farkı bu kod bloğunda net bir şekilde görebilirsin:
# --- PRINT KULLANAN FONKSİYON (Çıkmaz Sokak) ---
def sadece_yazdir(miktar):
    sonuc = miktar * 0.8
    print(f"Hesaplanan: {sonuc}") # Sadece ekrana yazar, veri uçup gider.

# --- RETURN KULLANAN FONKSİYON (Backend Standartı) ---
def veri_dondur(miktar):
    saf_madde = miktar * 0.8
    return saf_madde # Veriyi paketleyip dışarı fırlatır.

# TEST:
deger1 = sadece_yazdir(100) # deger1 'None' olur, çünkü fonksiyon bir şey vermedi.
deger2 = veri_dondur(100)   # deger2 '80' olur, artık bu sayıyı kullanabiliriz.

final_stok = deger2 + 50    # ÇALIŞIR: 80 + 50 = 130
# final_stok = deger1 + 50  # HATA VERİR: None ile sayı toplanamaz!
43.4 Karar Tablosu
Özellik	print()	return
Görünürlük	Kullanıcı terminalde görür.	Yazılımcı hafızada saklar.
Tekrar Kullanım	İmkansız (Veri yok olur).	Mümkün (Değişkene atanır).
Fonksiyon Durumu	Devam edebilir.	Fonksiyonu o an bitirir.
Backend Rolü	Hata ayıklama (Loglama).	Veri işleme (Mekanizma).
```
##### --- *ARGS UND **KWARGS--[44.0-44.4]
```PY
44.0 Dinamik Parametre Esnekliği (*args ve **kwargs)
44.1 Nedir: Bir fonksiyona kaç tane veri (argüman) gönderileceği önceden bilinmiyorsa kullanılır. Fonksiyonun kapasitesini sınırsız hale getirir ve backend sistemlerinde esneklik sağlar.

44.2 Kurallar:

*args (Sınırsız Liste): Fonksiyona gönderilen tüm isimsiz değerleri bir Tuple (demet) içinde toplar. Başına tek yıldız (*) konur.

**kwargs (Sınırsız Sözlük): Fonksiyona anahtar=değer şeklinde gönderilen tüm verileri bir Dictionary (sözlük) içinde toplar. Başına çift yıldız (**) konur.

Sıralama: Fonksiyon tanımlanırken önce standart parametreler, sonra *args, en son **kwargs yazılmalıdır.

44.3 Uygulamalı Örnek (Operasyonel Dinamik Fonksiyon):
# Fonksiyonu tanımlıyoruz (Dinamik Yapı)
def sevkiyat_merkezi(sorumlu, *uyusturucular, **ozellikler):
    print(f"Sorumlu: {sorumlu}")
    
    # *args içindeki her bir elemanı dönüyoruz
    for urun in uyusturucular:
        print(f"- Gönderilen Ürün: {urun}")
    
    # **kwargs içindeki her bir anahtar-değer çiftini dönüyoruz
    for baslik, detay in ozellikler.items():
        print(f"Detay -> {baslik}: {detay}")

# Fonksiyonu çağırıyoruz (Esnek Veri Gönderimi)
sevkiyat_merkezi("Mike", "Mavi_meth", "Sari_meth", Sehir="Albuquerque", Durum="Acil")

44.4 Ek bilgi:
Bölüm,Veri Yapısı,Gönderim Şekli,Kullanım Amacı
*args,Tuple (Sıralı),"""Veri1"", ""Veri2""",Bilinmeyen sayıda eleman listelemek.
**kwargs,Dictionary (İsimli),"id=101, tip=""Gaz""",Bilinmeyen sayıda detay/özellik eklemek.
```
##### --- FONKSIYON BIRINCI KISIM ILGILI--[45.0-50.0]
###### --- FONKSIYONLU DEGISKENLER--[45.0-45.4]
```PY
45.0 Fonksiyonu Değişkene Atama (Function as Variable)
45.1 Nedir: Bir fonksiyonun ismini, parantez kullanmadan başka bir değişkene eşitleme işlemidir. Bu sayede o değişken, artık o fonksiyonun "takma adı" (alias) olur ve fonksiyon gibi çalışmaya başlar.

45.2 Kurallar:

Parantezsiz Eşitleme: Fonksiyonu değişkene atarken degisken = fonksiyon şeklinde yazılır. Eğer fonksiyon() dersen, fonksiyonun içindeki sonucu atamış olursun. Biz ise fonksiyonun kendisini atıyoruz.

Aynı Yetenek: Yeni değişken, orijinal fonksiyonun sahip olduğu tüm parametreleri ve özellikleri devralır.

Esneklik: Backend tarafında, hangi işlemin yapılacağına çalışma anında (runtime) karar vermek için kullanılır.

45.3 Uygulamalı Örnek (Kod Adı Operasyonu):
# 1. Orijinal fonksiyonu tanımlıyoruz
def operasyon_merkezi(kod_adi):
    print(f"Sistem Erişimi Onaylandı: {kod_adi}")

# 2. Fonksiyonu bir değişkene atıyoruz (Takma Ad oluşturuyoruz)
# DİKKAT: Parantez yok!
heisenberg = operasyon_merkezi

# 3. Artık yeni değişkeni fonksiyon gibi çağırıyoruz
heisenberg("Mavi Kristal") 
# Çıktı: Sistem Erişimi Onaylandı: Mavi Kristal

45.4 Mantıksal Fark: Fonksiyon vs. Fonksiyon Sonucu

Bu ikisi arasındaki farkı anlamak, backend tarafında veri hatalarını önlemek için hayati önem taşır:
İşlem,Örnek,Ne Atanır?
Fonksiyonun Kendisi,x = selamla,Fonksiyonun çalışma yeteneği kopyalanır.
Fonksiyonun Sonucu,x = selamla(),Fonksiyondan dönen return değeri atanır.
```
###### --- FONKSIYONLU LISTELER--[46.0-46.4]
```PY
46.0 Fonksiyonlu Listeler (Functions in Lists)
46.1 Nedir: Birden fazla fonksiyonun bir liste ([]) içerisinde saklanmasıdır. Bu sayede bir döngü kullanarak birçok farklı işlemi tek bir komutla sırayla tetikleyebiliriz.

46.2 Kurallar:

Parantezsiz Kayıt: Liste içine eklerken fonksiyonun yanına parantez () koymazsın. Parantez koyarsan fonksiyonun kendisini değil, sonucunu listeye eklemiş olursun.

İndeksle Erişim: Listenin 0. elemanını çağırıp parantez ekleyerek liste[0]() şeklinde çalıştırabilirsin.

Döngü Kolaylığı: for f in liste: f() diyerek tüm operasyonu tek seferde başlatabilirsin.

46.3 Uygulamalı Örnek (Laboratuvar Hazırlık Zinciri):
# 1. Fonksiyonlarımızı tanımlıyoruz
def kimyasal_karistir():
    print("Kimyasallar %80 saflıkta karıştırıldı.")

def isi_kontrol():
    print("Isı 100 dereceye sabitlendi.")

def sevkiyat_hazirla():
    print("Ürünler paketlendi, Mike'a haber verildi.")

# 2. Fonksiyonları bir listenin içine diziyoruz (PARANTEZ YOK)
operasyon_plani = [kimyasal_karistir, isi_kontrol, sevkiyat_hazirla]

# 3. Tüm operasyonu sırayla başlatıyoruz
print("--- OPERASYON BAŞLIYOR ---")
for islem in operasyon_plani:
    islem() # Burada parantez koyarak fonksiyonu tetikliyoruz

46.4 Neden Fonksiyonlu Liste Kullanırız:
Avantaj,Açıklama
Sıralı İşlem,İşlemlerin tam olarak hangi sırayla yapılacağını garanti eder.
Dinamik Yapı,Listeye çalışma anında yeni bir fonksiyon ekleyebilir (append) veya silebilirsin.
Temiz Kod,50 tane fonksiyonu alt alta çağırmak yerine tek bir döngüyle işi bitirirsin.
```
###### --- FONKSIYONLU KOSULLU_IFADELER--[47.0-47.3]
```PY
47.0 Fonksiyonlu Karar Sistemleri (Dynamic Dispatch)
47.1 Nedir: Bir if veya match bloğu kullanarak, sistemin durumuna göre hangi fonksiyonun tetikleneceğine karar verme yöntemidir. Buna backend dünyasında "Dynamic Dispatch" denir; yani fonksiyonun çalışma anında (dispatch) seçilmesi.

47.2 Kurallar:
Karar Mekanizması: Fonksiyonu çağırmadan önce bir if bloğu ile "Hangi fonksiyonu çalıştırmalıyım?" sorusuna cevap aranır.

Esneklik: Kullanıcıya menü sunmak veya sistemin kritiklik seviyesine göre farklı prosedürler çalıştırmak için idealdir.

Hata Yönetimi: Beklenmedik bir girdi gelirse else bloğu ile sistemin çökmesini engelleriz.

47.3 Uygulamalı Örnek (Laboratuvar Mod Seçimi):
def mod_temizle():
    print("Laboratuvar temizleniyor... Mod: [TEMİZLİK]")

def mod_uretim():
    print("Üretim süreci başlatıldı... Mod: [ÜRETİM]")

# Kontrol mekanizması
def sistem_yonetimi(secilen_mod):
    if secilen_mod == "temizle":
        islem = mod_temizle # Fonksiyonu değişkene atadık
    elif secilen_mod == "uretim":
        islem = mod_uretim
    else:
        print("Hata: Geçersiz mod!")
        return # İşlemi durdur

    islem() # Seçilen fonksiyonu burada tetikliyoruz

# Test:
sistem_yonetimi("uretim") # Üretim modunu çalıştırır
```
###### --- FONKSIYONLU DONGULER--[48.0-48.4]
```PY
48.0 Fonksiyonlu Döngüler (Iterative Function Execution)
48.1 Nedir: Bir listedeki her bir elemanı sırayla bir fonksiyona parametre olarak gönderme veya bir fonksiyonu belirli bir sayıda tekrar çalıştırma işlemidir.

48.2 Kurallar:

Parametre Aktarımı: Döngüdeki her bir eleman, fonksiyonun parantez içine (argüman olarak) gönderilir.

Toplu İşleme: Tek bir fonksiyon yazarak binlerce farklı veriyi (stoklar, kullanıcılar, sıcaklıklar) aynı kural setinden geçirebilirsin.

Dönüş Değerlerini Toplama: Fonksiyondan return ile gelen sonuçları yeni bir listede biriktirerek "işlenmiş veri" seti oluşturabilirsin.

48.3 Uygulamalı Örnek (Toplu Safiyet Kontrolü):
# 1. İşlem yapacak fonksiyonu tanımlıyoruz
def saflik_analizi(miktar, oran):
    saf_gram = miktar * (oran / 100)
    return saf_gram

# 2. Veri setimiz (Miktarlar)
sevkiyatlar = [1000, 5000, 12000, 800]
analiz_sonuclari = []

# 3. Döngü ile fonksiyonu tetikliyoruz
print("--- ANALİZ BAŞLATILDI ---")
for s in sevkiyatlar:
    sonuc = saflik_analizi(s, 99.1) # Her sevkiyatı %99.1 oranla hesapla
    analiz_sonuclari.append(sonuc)
    print(f"Miktar: {s}g | Net Saf Madde: {sonuc}g")

# Artık elimizde işlenmiş verilerden oluşan bir liste var!

48.4 Döngü İçinde Fonksiyon Kullanmanın Avantajları:
Avantaj,Açıklama
Hata Kontrolü,"Eğer kural değişirse (örneğin oran %99 yerine %96 olursa), sadece fonksiyonu değiştirmen yeterlidir; döngüye dokunmazsın."
Okunabilirlik,Döngünün içinde 20 satır kod yazmak yerine islem_yap() diyerek kodu tertemiz tutarsın.
Performans,Büyük veri setlerini (Big Data) parçalara ayırıp fonksiyonlar aracılığıyla işlemek çok daha güvenlidir.
```
###### --- FONKSIYONLU SOZLUKLER--[49.0-49.4]
```PY
Harika bir final Dawut! Fonksiyonları Sözlükler (Dictionaries) içine koymak, backend dünyasında "Yönlendirme Tablosu" (Mapping/Routing) dediğimiz en üst seviye profesyonel yöntemdir.

Bu yöntemle, uzun if-elif-else bloklarını çöpe atıp, tek bir satırla binlerce komuttan istediğini anında tetikleyebilirsin.

Arşivin için bu bölümü "105.0 Fonksiyonlu Sözlükler (Function Mapping)" olarak kaydedebiliriz.

49.0 Fonksiyonlu Sözlükler (Function Mapping)
49.1 Nedir: Bir sözlüğün "değer" (value) kısmına bir fonksiyonun ismini (parantezsiz) yerleştirme işlemidir. Anahtar kelime (key) çağrıldığında, o anahtara bağlı olan fonksiyon tetiklenir.

49.2 Kurallar:

Eşleştirme: Sözlüğü tanımlarken {"komut": fonksiyon_adi} şeklinde yazılır.

Tetikleme: Sözlükten fonksiyonu çekerken sonuna parantez eklenir: sozluk["anahtar"]().

Hız: if-else blokları her satırı tek tek kontrol ederken, sözlükler hedef fonksiyonu anında bulur. Bu da büyük sistemlerde yüksek performans sağlar.

49.3 Uygulamalı Örnek (Merkezi Komuta Sistemi):
# 1. Görev fonksiyonlarını tanımlıyoruz
def sevkiyat_baslat():
    print("Mike yola çıktı, sevkiyat güvenli.")

def uretim_baslat():
    print("Laboratuvar aktif, üretim %99 saflıkta.")

def sistemi_kapat():
    print("Tüm izler silindi, sistem kapalı.")

# 2. Fonksiyonları sözlüğe yerleştiriyoruz (PARANTEZ YOK)
komuta_merkezi = {
    "SEVKIYAT": sevkiyat_baslat,
    "URETIM": uretim_baslat,
    "KAPAT": sistemi_kapat
}

# 3. Dinamik tetikleme
emir = "URETIM"

if emir in komuta_merkezi:
    komuta_merkezi[emir]() # Seçilen fonksiyonu parantez ekleyerek çalıştırıyoruz
else:
    print("Geçersiz Emir!")

49.4 Neden Fonksiyonlu Sözlük Kullanırız:
Avantaj,Açıklama
Hız (O(1)),Binlerce seçenek arasından doğru fonksiyonu milisaniyeler içinde bulur.
Temizlik,20 tane elif yazmak yerine tek bir sözlükle kodu tertemiz tutarsın.
Modülerlik,Sisteme yeni bir özellik eklemek için sadece sözlüğe bir satır eklemen yeterlidir.
``` 
###### --- FONKSIYONLU HEPSI--[50.0-50.4]
```PY
50.0 Büyük Senaryo: Entegre Fonksiyonel Sistemler
50.1 Nedir: Yazılımın farklı parçalarının (veri girişi, kontrol, işleme ve raporlama) birbirine bağlı fonksiyonlar aracılığıyla bir makine gibi çalışmasıdır.

50.2 Senaryo: Bir laboratuvar yönetim sistemi kuruyoruz. Sistem; gelen ham maddeyi alacak (*args), özelliklerini kaydedecek (**kwargs), durumuna göre hangi işlemi yapacağına karar verecek (Sözlük/Mapping) ve tüm sevkiyatı döngüyle bitirecek.

50.3 Büyük Final Kodu (Entegre Sistem):
# --- 1. ALT FONKSİYONLAR (İŞLEMCİLER) ---
def saflik_hesapla(miktar):
    return miktar * 0.991  # %99.1 saflık oranı

def kalite_kontrol(durum):
    if durum == "KRITIK":
        return "!!! ACIL MUDAHALE !!!"
    return "Standart Prosedür Uygulanıyor."

# --- 2. ANA YÖNETİM SÖZLÜĞÜ (MAPPING) ---
# Fonksiyonları bir sözlüğe hapsediyoruz
operasyon_rehberi = {
    "ANALIZ": saflik_hesapla,
    "KONTROL": kalite_kontrol
}

# --- 3. DİNAMİK SEVKİYAT MERKEZİ (ARGS & KWARGS) ---
def laboratuvar_sistemi(sorumlu, *miktarlar, **detaylar):
    print(f"=== OPERASYON SORUMLUSU: {sorumlu} ===")
    
    # Döngü ile her bir miktarı fonksiyondan geçiriyoruz
    for m in miktarlar:
        net_sonuc = operasyon_rehberi["ANALIZ"](m) # Sözlükten fonksiyon çağrıldı
        print(f"Ham Madde: {m}g | Saf Madde: {net_sonuc}g")

    # Sözlük ve Karar Yapısı Birleşimi
    print("\n--- TEKNİK DETAYLAR ---")
    for ozellik, deger in detaylar.items():
        mesaj = operasyon_rehberi["KONTROL"](deger) # Dinamik karar
        print(f"Özellik: {ozellik} -> Durum: {deger} | Karar: {mesaj}")

# --- 4. SİSTEMİ TETİKLEME ---
# Mike sorumlu, 3 farklı miktar var, 2 farklı kritik detay var.
laboratuvar_sistemi("Mike", 1000, 5000, 12000, Sicaklik="STABIL", Basinc="KRITIK")

50.4 Sistemin Anatomisi (Neyi Birleştirdik?):
Kullanılan Yapı,Kodun Neresinde?,Backend Görevi
*args,*miktarlar,Belirsiz sayıdaki veriyi paketlemek.
**kwargs,**detaylar,"Esnek teknik özellikleri (sıcaklık, basınç) toplamak."
Sözlük (Mapping),operasyon_rehberi,Hangi fonksiyonun çalışacağını anında bulmak.
Döngü (Loop),for m in miktarlar,Operasyonu tüm veri seti üzerinde tekrarlamak.
Return,return miktar * 0.991,Hesaplanan veriyi sisteme geri vermek.

50.5 Operasyonel Akış Diyagramı (Mermaid):
```
```mermaid
graph TD
    Start([Başlat: laboratuvar_sistemi]) --> UnpackArgs[args: Miktarları Listele]
    Start --> UnpackKwargs[kwargs: Detayları Sözlükle]
    
    UnpackArgs --> Loop1[Döngü: Her Miktar İçin]
    Loop1 --> Map1[Sözlükten ANALIZ Fonksiyonunu Bul]
    Map1 --> Calc[Safiyet Hesapla ve Yazdır]
    Calc --> Loop1
    
    UnpackKwargs --> Loop2[Döngü: Her Detay İçin]
    Loop2 --> Map2[Sözlükten KONTROL Fonksiyonunu Bul]
    Map2 --> Check[Kritiklik Kontrolü ve Yazdır]
    Check --> Loop2
    
    Loop1 & Loop2 --> End([Operasyon Tamamlandı])

    style Map1 fill:#bbf,stroke:#333
    style Map2 fill:#bbf,stroke:#333
    style Check fill:#f9f,stroke:#333
```

# --- CODEX PYTHON: BIRINCI DONEM --- 
## --- BIRINCI KISIM --- [01.01.2026-03.04.2026]
### --- I BOLUM: TEMEL_DEGISKENLER --- [26.01.2026-30.01.2026]
#### --- PRINT,INPUT,INT,STR --- [26.01.2026] ---
##### --- ilk bolum
```py
isim = input("isminizi buraya girin: ")
yas = int(input("yasiniz kac: "))

print("sayin", isim, "on yil sonra", yas + 10, "Olucaksiniz")
```
##### --- ikinci bolum
```py
sehir = input("sehirin ismi: ")
nesne = str(input("nesnenin ismi: "))
renk = input("renkin ismi: ")

print(sehir, "sokaklarinda", renk, "bir", nesne, "gordum",)
```
##### --- sablon bolum
```mermaid
graph TD
    subgraph "Bölüm 1: Yaş Hesaplayıcı"
        A1[Giriş: İsim ve Yaş] --> B1[İşlem: Yaş + 10]
        B1 --> C1[Çıkış: Gelecek Tahmini]
    end

    subgraph "Bölüm 2: Hikaye Oluşturucu"
        A2[Giriş: Şehir, Nesne, Renk] --> B2[İşlem: Metin Birleştirme]
        B2 --> C2[Çıkış: Hikaye Cümlesi]
    end
```
#### --- FLOAT,INT,%*/,STR --- [28.01.2026] ---
##### --- ilk bolum
```py
ekmek = float(input("ekmegin fiyati: "))
adet = int(input("adet fiyati: "))
```
##### --- ikinci bolum
```py
ekmek = float(input("ekmegin fiyati: "))
adet = int(input("adet fiyati: "))

toplam = (adet - 1) * ekmek 

print("ekmegin fiyati", ekmek, "tl", "adetin fiyati", adet, "tl", "toplam", toplam, "tl")
```
##### --- Ucuncu bolum
```py
sehir = str(input("gidicegin sehrin ismi: "))
mesafe = int(input("gidicegin uzakligi: "))
yakit = float(input("arabanin km yakacagi yakiti: "))

toplam = mesafe * yakit 

print(sehir, "sehirine gidiyorsun", mesafe, "kadar uzakliktasin", yakit, "bu kadar yakitin var", "toplam bu kadar tl harcadiniz", toplam )
```
##### --- sablon bolum
```mermaid
graph TD
    subgraph "Bolum 1 & 2: Ekmek Hesabi (Matematiksel Islem)"
        A1[Giris: Ekmek Fiyati ve Adet] --> B1[Islem: toplam = adet-1 * ekmek]
        B1 --> C1[Cikis: Toplam TL Yazdir]
    end

    subgraph "Bolum 3: Yolculuk Hesabi (Degisken Yonetimi)"
        A2[Giris: Sehir, Mesafe, Yakit] --> B2[Islem: toplam = mesafe * yakit]
        B2 --> C2[Cikis: Yol ve Maliyet Bilgisi]
    end
```
#### --- LEN,[0:2 -2:],INPUT,PRINT --- [30.01.2026] ---
##### --- Birinci bolum
```py
isim = input("ismini gir: ")
soyad = input("soyismini gir: ")
Dogum_yili = input("Dogum yilini gir: ")
ismin_boyu = len(isim)

bas_isim = isim[0:2]
bas_soyad = soyad[-2:]
bas_Dogum_yili = Dogum_yili[-2:]

kullanici_adi = "ID_" + bas_isim + bas_soyad + bas_Dogum_yili

print("ismin", isim, "soyadin", soyad, "Dogum yilin", Dogum_yili, "Kullanici ismin", kullanici_adi, "ismin boyu", ismin_boyu )
```
##### --- Ikinci bolum
```py
hayvan = input("hayvanin ismi: ")
sehir = input("sehirin ismi: ")
sayi = str(input("sansli sayi: "))


hayvan_adi = hayvan[0:2]
sehir_adi = sehir[-2:]
sayi_rakami = sayi[-2:]

kisa_takma_adi = hayvan_adi + sehir_adi + sayi_rakami 
uzunluk = len(kisa_takma_adi)

print("hayvanin ismi", hayvan, sehir, "sehirde yerlesiyor", sayi_rakami, "rakami duruyor", "takma ismi", kisa_takma_adi,)
print("HSS rakami", uzunluk)
```
##### --- sablon bolum
```mermaid
graph TD
    subgraph "Bolum 1: Kullanici ID Olusturucu"
        A1[Giris: Isim, Soyad, Dogum Yili] --> B1[Islem: Dilimleme 0:2 ve -2:]
        B1 --> C1[Birlestirme: 'ID_' + Parcalar]
        C1 --> D1[Cikis: Kullanici Adi ve Isim Boyu]
    end

    subgraph "Bolum 2: HSS Takma Ad Olusturucu"
        A2[Giris: Hayvan, Sehir, Sansli Sayi] --> B2[Islem: Dilimleme 0:2 ve -2:]
        B2 --> C2[Birlestirme: Parcalari Uc Uca Ekle]
        C2 --> D2[Cikis: Takma Ad ve HSS Uzunlugu]
    end
```
### --- II BOLUM: LISTELER --- [02.02.2026-06.02.2026]
#### --- INSERT,APPEND,REMOVE,LEN --- [02.02.2026]
##### --- ilk bolum 
```py
sehir = ["Istanbul", "Ankara", "Trabzon", "Adana", "Diyarbakir"]

print("sehirler: ", sehir)
```
##### --- ikinci bolum 
```py
sehir = ["Istanbul", "Ankara", "Trabzon", "Adana", "Diyarbakir"]

print("birinci sehir", sehir[2], "ikinci sehir", sehir[3])
```
##### --- ucuncu bolum 
```py
sehir = ["Istanbul", "Ankara", "Trabzon", "Adana", "Diyarbakir"]

sehir.insert(1, "Viyana")
sehir.append("Munih")
sehir[2] = "Askabat"

print("yeni sehirler", sehir)
```
##### --- dorduncu bolum 
```py
sehir = ["Istanbul", "Ankara", "Trabzon", "Adana", "Diyarbakir"]

sehir.insert(1, "Viyana")
sehir.append("Munih")
sehir[2] = "Askabat"
sehir.remove("Adana")
sehirler = len("sehirlerin listesi")

print("yeni sehirler", sehir, "sehirlerin sayisi", sehirler)
```
##### --- besinci bolum 
```py
sehir = ["Istanbul", "Ankara", "Trabzon", "Adana", "Diyarbakir"]

sehir.insert(1, "Viyana")
sehir.append("Munih")
sehir[2] = "Askabat"
sehir.remove("Adana")
sehirler_sayisi = len(sehir)

print("yeni sehirler", sehir)
print("sehirlerin sayisi", sehirler_sayisi)
```
##### --- altinci bolum 
```py
sehir = ["Istanbul", "Ankara", "Trabzon", "Adana", "Diyarbakir"]

sehir.insert(1, "Viyana")
sehir.append("Munih")
sehir[2] = "Askabat"
sehir.remove("Adana")
sehirler_sayisi = len(sehir)

print("yeni sehirler", sehir)
print("sehirlerin sayisi", sehirler_sayisi)
print("sondaki sehirler: ", sehir[-1], sehir[-2])

```
##### --- sablon bolum 
```mermaid
graph TD
    subgraph "Bolum 1 & 2: Temel Liste ve Index"
        A1[Liste Olusturma] --> B1[Index ile Veri Cekme: sehir 2 ve 3]
    end

    subgraph "Bolum 3, 4 & 5: Listeyi Degistirme"
        A2[Insert: 1. Indexe Viyana] --> B2[Append: Sona Munih]
        B2 --> C2[Guncelleme: 2. Index = Askabat]
        C2 --> D2[Remove: Adana Silindi]
    end

    subgraph "Bolum 6: Analiz ve Final"
        A3[len: Liste Sayisini Oolc] --> B3[Negatif Index: Sondan Veri Cekme -1, -2]
    end

    B1 -.-> A2
    D2 -.-> A3
```
#### --- SORT,SORTED,REVERSE,(REVERSE = T) --- [04.02.2026]
##### --- ilk bolum
```py
sehirler = ["Munih", "Bayern", "Berlin", "Frankfurt"]

sehirler.reverse()

print("Sehirler siralamasi", sehirler)

sehirler.sort()

print("Sehirler siralamasi", sehirler)
```
##### --- ikinci bolum
```py
notlar = [85, 45, 100, 20, 75, 90]

notlar.sort(reverse = False)

print("bastan sona notlar", notlar)

notlar.sort(reverse = True)

print("sondan baslangica notlar", notlar)

notlar.sort()

print("True veya false kullanmadan Notlar", notlar)
```
##### --- ucuncu bolum
```py
notlar = [70, 95, 40, 60, 10]
print("Gecici not siralamasi", sorted(notlar))

notlar.sort(reverse = True)
print("sondan basina kadar notlarim", notlar)

notlar.sort(reverse = False)
print("basdan sonuna kadar notlarim", notlar)

notlar.reverse()
print("tam tersi notlarim", notlar)

notlar.append(50)
print("en bastaki siralamasiz notlarim", notlar)
```
##### --- sablon bolum
```mermaid
graph TD
    subgraph "Bolum 1: Metin Siralama ve Yon"
        A1[Liste: Sehirler] --> B1["sehirler.reverse() (Sadece Listeyi Tersine Cevir)"]
        B1 --> C1["sehirler.sort() (Alfabetik A-Z Sirala)"]
        C1 --> D1[Cikis: Kalici Siralanmis Liste]
    end

    subgraph "Bolum 2: Sayisal Not Siralamasi"
        A2[Liste: Notlar] --> B2["sort(reverse=False) (Kucukten Buyuge)"]
        B2 --> C2["sort(reverse=True) (Buyukten Kucuge)"]
        C2 --> D2["sort() (Varsayilan: Kucukten Buyuge)"]
    end
```
#### --- IKINCI BOLUMDEKI HEPSI --- [06.02.2026]
##### --- ilk zorlu bolum
```py
sehirler = ["Almanya", "Berlin", "Dortmund", "Munih"]

sehirler.append("Kalingrad")

print(sorted(sehirler))

sehirler.sort(reverse = True)

print(sehirler)

print(len(sehirler))
```
##### --- ikinci zorlu bolum
```py
maaslar = [3000, 4500, 5000, 2500]
yeni_eleman = int(input("Yeni elemanin maasi: "))

print("eski butun personellerin maaslari", maaslar) 

maaslar.append(yeni_eleman)

print("suanki butun personellerin maaslari", maaslar)

yuksek_maasli = max(maaslar)
dusuk_maasli = min(maaslar)

print("yuksek maasli olan", yuksek_maasli)
print(" dusuk maasli olan", dusuk_maasli)
print("Eski personellerin sıralı maaşları:", sorted(maaslar))

maaslar.pop(2)

maaslar.sort(reverse = True)

print("Su anki en guncel maas bilgileri", maaslar)
```
##### --- ucuncu zorlu bolum
```py
araclar = ["W-123", "VI-99", "S-45"]

araclar.append("E-67")
araclar.append("V-84")

print("iki yeni gelen araclarin plakasi", araclar)

araclar.insert(0, "DIPLOMAT")

print("suanki yeni gelmis diplomat plakasi ve diger araclar", araclar)

araclar.remove("VI-99")
araclar.pop(2)

print("birisi plakasi ve digeri sinir doldugu icin geri kalan araclar", araclar)

hizlar = [120, 80, 140, 110, 90]
yuksek_hiz = max(hizlar)
dusuk_hiz = min(hizlar)

print("suanki mewcut araclar", araclar)
print("en yuksek hizda giden arac", yuksek_hiz)
print("en dusuk hizda giden arac", dusuk_hiz)

print("suanki sinirin icindeki araclar", araclar)

araclar.sort(reverse = True)

print("Suanki A/Z kadar harf sistemine sinirlandirilmis araclar", araclar)
print("yasasin Arztorzka")
```
##### --- dorduncu zorlu bolum
```py
nvanter = ["M4A1", "Glock 17", "El Bombasi", "Zirh", "Kask"]
envanter.append("M24")
envanter.remove("El Bombasi")

print(sorted(envanter))
print("envantere yeni ekipman ve birsey azaldi ", envanter )

envanter.insert(0, "Gece gorus durbunu")
envanter.sort(reverse = True)

print("su anki mevcut envanter listesi", envanter)

parcaciklar = len(envanter)

print("Su anki mevcut silahlar", parcaciklar)
```
##### --- sablon zorlu bolum
```mermaid
graph TD
    subgraph "Zorlu 1: Sehir Planlama"
        A1[Liste: Sehirler] --> B1[Append: Kaliningrad]
        B1 --> C1[Sorted: Gecici Alfabetik]
        C1 --> D1[Sort Reverse: Kalici Ters Siralama]
    end

    subgraph "Zorlu 2: Maas Yonetimi"
        A2[Liste: Maaslar] --> B2[Input: Yeni Eleman]
        B2 --> C2[Max/Min: Uclari Bul]
        C2 --> D2[Pop: 2. Index Cikarildi]
        D2 --> E2[Sort Reverse: Guncel Maaslar]
    end

    subgraph "Zorlu 3: Arztorzka Gümrük"
        A3[Liste: Araclar] --> B3[Insert: DIPLOMAT Basa]
        B3 --> C3[Remove/Pop: Arac Eksiltme]
        C3 --> D3[Hiz Analizi: Max/Min Hiz]
        D3 --> E3[Sort Reverse: Plaka Siralama]
    end

    subgraph "Zorlu 4: Askeri Envanter"
        A4[Liste: Envanter] --> B4[Append/Remove: Silah Guncelleme]
        B4 --> C4[Insert: Gece Gorus Durbunu]
        C4 --> D4[Sort Reverse: Ekipman Siralama]
        D4 --> E4[Len: Parcacik Sayisi]
    end
```
### --- III BOLUM: KONTROL_AKISI VE KOSULLU_IFADELER --- [09.02.2026-14.02.2026]
#### --- IF,ELIF,ELSE,AND/OR --- [09.02.2026]
##### --- ilk karmasik bolum
```py
isim = "Dawut"
yas = 19
vize_durumu = True
askerlik_durumu = True
if yas >= 18 and vize_durumu == True:
    if askerlik_durumu == False:
        print("askerliginizi yapmadan disari cikiyorsunuz geldiginiz an askerlige gonderilyorsunuz ")
    print("yasiniz ve vize_durumu onaylandi gecebilirsiniz yasasin arztozka ")

elif yas < 18 and vize_durumu == True:
    if askerlik_durumu == False:
        print("askerligi yapmadan resit olmadan baska ulkeye gidiyorsunuz aileniz olmadan cikmaniz mumkun degil")
    print("vize durumu olsada resit degilsiniz aileniz olmadan gecemezsiniz")
else:
    if askerlik_durumu == False and yas == 18:
        print("askerlik yapmadan baska ulkeye gidemediniz bu yuzden dogru askerlik subesine yonlendiriliyorsunuz")
    print("yas veya vize durumu olumsuz gecmeniz yasak")

print("yasasin artzozka")
```
##### --- ikinci sade bolum
```py
isim = "Dawut"
yas = 18
vize_durumu = True
askerlik_durumu = True
sabika_kaydi = False
izin_kagidi = True

if sabika_kaydi == True:
    print("gecis izni sabika kaydiniz oldugu icin reddedildi")

elif yas >= 18 and vize_durumu and askerlik_durumu and izin_kagidi:
    print(f"Hos geldin {isim} Butun prosudur uyuyor devam edebilirsiniz")

elif izin_kagidi == True:
    print("belgeleriniz eksik olsada izin kagidi oldugu icin gecebilirsiniz")

elif yas < 18 or vize_durumu == False:
    print("uzgunuz ama yasiniz veya vize durumu uygun degil giris reddedildi")

else:
    print("prosudurlerin cogunu karsilamadiginiz icin vize reddedildi")
```
##### --- ucuncu bolum
```py
isim = "Epstein"
yas = 18
para = 500
yaninda_arkadasin_varmi = True
vip_cart = False

if vip_cart == True:
    print(f"Hos geldiniz {isim} iceri girebilirsiniz")

elif vip_cart == False and yas >= 18 and (para >= 1000 or yaninda_arkadasin_varmi == True):
    print(f"iceri girebilirsiniz {isim}")

else:
    print("uzgunum iceri giremezsiniz")

iste gemini 
```
##### --- dorduncu bolum
```py
isim = "Epstein"
yas = 18
para = 500
yaninda_arkadasin_varmi = True
vip_cart = False

if vip_cart == True:
    print(f"Hos geldiniz {isim} iceri girebilirsiniz")

elif vip_cart == False and yas >= 18 and (para >= 1000 or yaninda_arkadasin_varmi == True):
    print(f"iceri girebilirsiniz {isim}")

else:
    print("uzgunum iceri giremezsiniz")

```
##### --- besinci bolum
```py
isim = "Dawut"
kart_var_mi = False
sifre_dogru_mu = False
parmak_izi_onayli_mi = False
yuz_tanima_onayli_mi = False
acil_durum_modu = False

if acil_durum_modu == True:
    print("UYARI KAPILAR KILITLENDI")

elif kart_var_mi and parmak_izi_onayli_mi:
    print(f"vip oldugunuc icin geciz izni verildi {isim} yasasin artzortkza")

elif kart_var_mi == False and sifre_dogru_mu == False and(parmak_izi_onayli_mi == True or yuz_tanima_onayli_mi == True ):
    print("giris onaylandi")

else:
    print("YETKISIZ GIRIS GUVENLIK CAGRILIYOR")
```
##### --- altinci bolum
```py
isim = "David Agnus"
vize = True
almanca_puan = 100
banka_bakiyesi = 9000
alman_pasaport = True

if alman_pasaport:
    print(f"GUTEN MORGEN {isim} lutfen devam edin Heil GERMANICH")

elif vize:
    if almanca_puan >= 70 and banka_bakiyesi >= 7000:
        print("vize diliniz ve banka seviyeniz iyi gecebilirsiniz")
    else:
        print("vizeniz var ama digerlerde sinifta kaldiniz vizeniz kismen reddedildi")
else:
    print("istekleri karsilamiyorsunuz reddedildi")

```
##### --- yedinci bolum
```py
kat_numarasi = 21
yetki_seviyesi = 2
yangin_alarmi = False

if yangin_alarmi == True:
    print("GECERSIZ BINA TAHLIYE EDILIYOR")

elif kat_numarasi >= 21 or kat_numarasi <= 40:
    if yetki_seviyesi >= 2:
        print(f"suan sizde {yetki_seviyesi} yetki karti bulunuyor suan {kat_numarasi} kat seviyesi cikiyor ")
    else:
        print("uzgunum bu kata cikalamaz yetki seviyeniz dusuk")
elif kat_numarasi <= 20:
    if yetki_seviyesi <= 1:
        print(f" 1 yetki karti bulunuyor suan 20 kata kadar erisim var {kat_numarasi} kata cikiliyor")
```
##### --- birinci sablon bolum
```mermaid
graph TD
    Start([Baslangic]) --> Check1{Yas >= 18 ve Vize?}
    Check1 -- Evet --> Check2{Askerlik Bitti mi?}
    Check2 -- Hayir --> P1[Uyari: Geldiginde askere gideceksin]
    Check2 -- Evet --> P2[Onay: Yasasin Arztozka]
    P1 --> P2
    Check1 -- Hayir --> Check3{Yas < 18 ve Vize?}
    Check3 -- Evet --> Check4{Askerlik Bitti mi?}
    Check4 -- Hayir --> P3[Uyari: Resit degilsin, aile lazim]
    Check3 -- Hayir --> P6[Ret: Olumsuz Durum]
    P2 --> Final[BUTUN YOLLAR ROMAYA CIKAR]
    P4 --> Final
    P6 --> Final
```
##### --- ikinci sablon bolum
```mermaid
graph TD
    Start2([Giris Denemesi]) --> Emergency{Acil Durum Modu?}
    
    Emergency -- Evet --> Alert[KAPILAR KILITLENDI]
    
    Emergency -- Hayir --> VIP{Kart VE Parmak Izi?}
    VIP -- Evet --> Welcome[Giris Onaylandi: Yasasin Artzortkza]
    
    VIP -- Hayir --> Complex{Kart Yok VE Sifre Yanlis VE <br/> Parmak Izi VEYA Yuz Tanima?}
    Complex -- Evet --> Basic[Giris Onaylandi]
    Complex -- Hayir --> Security[YETKISIZ GIRIS: GUVENLIK!]
```
##### --- ucuncu sablon bolum
```mermaid
graph TD
    Start([Asansor Paneli]) --> Alarm{Yangin Alarmi?}
    
    Alarm -- Evet --> Exit[BINA TAHLIYE EDILIYOR]
    
    Alarm -- Hayir --> KatCheck{Kat 21-40 arasi mi?}
    
    KatCheck -- Evet --> PowerCheck{Yetki Seviyesi >= 2?}
    PowerCheck -- Evet --> Access1[Erisim Onaylandi: Kata cikiliyor]
    PowerCheck -- Hayir --> Deny1[Erisim Red: Yetki Dusuk]
    
    KatCheck -- Hayir --> LowCheck{Kat <= 20 mi?}
    LowCheck -- Evet --> PowerCheck2{Yetki Seviyesi <= 1?}
    PowerCheck2 -- Evet --> Access2[Erisim Onaylandi: 20. kata kadar]
    PowerCheck2 -- Hayir --> Deny2[Gecersiz Islem]
    
    LowCheck -- Hayir --> Deny2
```
#### --- carsamba gunu dinlenme gunu oldu [11.02.2026]
#### --- UCUNCU BOLUMDEKI HEPSI --- [13.02.2026]
##### --- birinci bolum
```py
sinava_girdi = True
notu = 50

if sinava_girdi == True:
    print("sinava girdin tamam")
    if notu >= 50:
        print("sinavi gectin tebrikler")
    else:
        print("sinavi gecemedin seneye tekrar dene")
else:
    print("sinava girmemissin bir dahaki sefere")
```
##### --- ikinci bolum 
```py
kart_takili = True
if kart_takili == True:
    print("kart suan takili islem yapiliyor")
    sifre = int(input("sifrenizi girin: "))
    if sifre == 1234:
        print("sifre dogru kartinizi alabilirsiniz")
    else:
        print("PIN yanlis")
else:
    print("kartiniz yoksa islem yapilamaz")
```
##### --- ucuncu bolum 
```py
yas = 18
Los_polloz_hermanos = False

if Los_polloz_hermanos == True:
    print("iceri girin")
elif yas >= 18:
    print("yasiniz buyuk tamam")
    bilet_varmi = str(input("Bilet varmi?: "))
    if bilet_varmi == "evet":
        print("tamam iceri girebilirsiniz iyi eglecenler")
    else:
        para_varmi = int(input("paraniz varmi peki?: "))
        if para_varmi >= 200:
            print("tamam iceri girebilirsiniz sorun cikarmtmayin")
        else:
            print("uzgunum para olmadan giremezsiniz")
else:
    print("uzgunum yasiniz buna uygun degil") 
```
##### --- dorduncu bolum
```py
almanca = input("Almanca biliyormusunuz: ")
diploma = input("universite mezunumuzsunuz: ")
if almanca == "evet" and diploma == "evet":
    print("tamam o zaman ek detatylara basliyalim")
    maas = int(input("yillik kac euro maas aliyorsunuz ?"))
    if maas >= 50000:
        print("tebrikler! Blue kart onayli")
    elif maas >= 40000 and maas <= 50000:
        print("blue kart icin ek inceleme yapilmali")
    else:
            print("maasiniz yetersiz bu yuzden calisma vizesi ile gidiyorsunuz")
else:
    print("uzgunum almancaniz veya unicersite diplomaniz yok bu yuzden gecemezsini")
```
##### --- ilk sablon bolum
```mermaid
graph TD
    A[Başla] --> B{Los Pollos Hermanos?}
    B -- Evet --> C[İçeri girin]
    B -- Hayır --> D{Yaş >= 18?}
    D -- Hayır --> E[Yaş uygun değil]
    D -- Evet --> F[Yaşınız büyük tamam]
    F --> G{Bilet var mı?}
    G -- Evet --> H[İçeri girebilirsiniz]
    G -- Hayır --> I[Paranız var mı?]
    I --> J{Para >= 200?}
    J -- Evet --> K[Sorun çıkarmadan girin]
    J -- Hayır --> L[Para olmadan girilemez]
```
##### --- ikinci sablon bolum
```mermaid
graph TD
    Start[Süreç Başladı] --> Q1{Almanca ve Diploma?}
    Q1 -- Hayır --> Reject[Geçemezsiniz: Eksik belge/dil]
    Q1 -- Evet --> Info[Ek detaylara geçelim]
    Info --> Q2{Yıllık Maaş?}
    Q2 -- ">= 50.000€" --> Approved[Blue Kart Onaylandı!]
    Q2 -- "40.000€ - 50.000€" --> Review[Ek inceleme yapılmalı]
    Q2 -- "< 40.000€" --> WorkVisa[Çalışma vizesi ile gidiş]
```
#### --- CARSAMBA GUNU TELAFI IF,ELIF,ELSE,NESTED IF --- [14.02.2026]
##### --- ilk bolum
```py
butce = 12000
sponsor_var_mi = False
dil_seviyesi = "B2"

if butce >= 12000 or sponsor_var_mi == True:
    print("butce/sponsor bulunmakta devam edelim")
    if dil_seviyesi == "B1" or dil_seviyesi == "B2":
        print("dil seviyeniz uygun vize alabilirsinz")
    else:
        print("uzgunum dil gecerliliginiz B1 den dusuk alamam")
else:
    print("uzgunum butce rakami dusuk veya sponsorlugunuz yok giris reddedildi ") 
```
##### --- ikinci bolum 
```py
yas = 18
sabika_kaydi = True
tecrube_yili = 2
ustun_yetenek = True

if yas == 18:
    print("yasiniz 18 veya 18 den yukarida vizeye devam edelim ")
    if sabika_kaydi == False and (tecrube_yili >= 2 or ustun_yetenek):
        print("sabika kaydiniz yok ve tecrube_yili/ustun_yetenigiz oldugu belli vize kabul edildi")
    else:
        if sabika_kaydi == True:
            print("uzgunum sabika kaydiniz var vize reddedildi")
        elif tecrube_yili < 2 or ustun_yetenek == False:
            print("uzgunum tecrube_yiliniz/ustun_yeteginiz yok bu yuzden vize reddedildi")
else:
    print("18 yasdan kucuksunuz vize reddedildi")
```
##### --- ucuncu bolum
```py
yas = 18
sabika_kaydi = True
tecrube_yili = 2
ustun_yetenek = True

if yas == 18:
    print("yasiniz 18 veya 18 den yukarida vizeye devam edelim ")
    if sabika_kaydi == False and (tecrube_yili >= 2 or ustun_yetenek):
        print("sabika kaydiniz yok ve tecrube_yili/ustun_yetenigiz oldugu belli vize kabul edildi")
    else:
        if sabika_kaydi == True:
            print("uzgunum sabika kaydiniz var vize reddedildi")
        elif tecrube_yili < 2 or ustun_yetenek == False:
            print("uzgunum tecrube_yiliniz/ustun_yeteginiz yok bu yuzden vize reddedildi")
else:
    print("18 yasdan kucuksunuz vize reddedildi")
```
##### --- dorduncu bolum karmasik
```py
GPA = 2.9
IELTS = 6.4
disiplin_cezasi = True

if disiplin_cezasi == False:
    print("disiplin cezasi yok diger onemli kurallara devam edelim")
    if GPA >= 4.0 and IELTS >= 6.5:
        print("GPA ve IELTS ortalamasi karsiliyor universiteye kabul edildiniz")
    elif GPA >= 5.0 and IELTS < 6.5:
        print("GPA Durumu yeterli ama IELTS yetersiz universitede iyice hazirlanmalisinz istisna olarak GPA normalden yuksek universite kabul edildiniz")
    elif GPA < 3.0 and IELTS >= 6.5:
        print("IELTS yuksek olsada GPA dusuk bu yuzden bir dahaki sefere universite kabul edilmedi")
    elif GPA < 3.0 and IELTS < 6.5:
        print("uzgunum GPA ve IELTS yetersiz bu yuzden universite bolumu kabul edilmedi")
    else:
        print("Akademik sartlar tam saglanamadi")
else:
    print("disiplin cezasi yuzunden reddedildi")
```
##### --- dorduncu bolum sade
```py
GPA = 3.0
IELTS = 6.5
disiplin_cezasi = True

if disiplin_cezasi:
    print("disiplin cezasi kabul edilmesi")
else:

    normal_kabul = (GPA >= 3.0 and IELTS >= 6.5)
    istisna_kabul = (GPA >= 4.0 and IELTS >= 6.0)

    if normal_kabul or istisna_kabul:
        print("universiteye hos geldiniz")
    else:
        print("Sartlar saglanamadi")
```
##### --- ilk sablon bolum
```mermaid
graph LR
    A[Başla] --> B{Almanca var mı?}
    B -- Hayır --> F[RED: Geçemezsiniz]
    B -- Evet --> C{Diploma var mı?}
    C -- Hayır --> F
    C -- Evet --> D[KASA AÇILDI: Devam]
```
##### --- ikinci sablon bolum
```mermaid
graph TD
    Start((Değişken)) --> Check{Değer Kaç?}
    Check -- "Sayı (1, 2, ...)" --> TrueNode[TRUE]
    Check -- "Sıfır (0)" --> FalseNode[FALSE]
    TrueNode --> ActionT[Döngü Devam Eder]
    FalseNode --> ActionF[Döngü Durur]
```
### --- IV BOLUM: DONGULER --- [16.02.2026-21.02.2026] 
#### --- FOR IN RANGE --- [16.02.2026_and_17.02.2026]
##### --- ilk bolum 
```py
#while dongusu
sayi = 10
while sayi >= 0:
    print(f"sayi: {sayi}")
    sayi = sayi - 1
print("bitdi")

# for dongusu
listeler = ["karpuz", "elma", "cilek", "ananas"]
for liste in listeler:
    print(f"meyveler: {liste}")

if liste == "cilek":
        print(f"meyveler: {liste} - Bu benim en sevdiğim!")
    else:
        print(f"meyveler: {liste}")
```
##### --- ikinci bolum
```py
#for dongusu
sayilar = [5, 12, 8, 20, 3, 15, 30]

for sayi in sayilar:
    if sayi > 10:
        print(f"buyuk sayi {sayi}")
    else:
        print(f"kucuk sayi {sayi}")

#while dongusu
while True:
    komut = input("donguyu kapatmak istiyorsaniz 'kapat' diyin: ")

    if komut == 'kapat':
        break

print("dongu kapatildi")
```
##### --- ucuncu bolum
```py
# for birincisi
sayi = 0

for sayi in range(0, 21, 2):
    print(f"{sayi} cift sayilar")

#for ikincisi

uyeler = ["Dawut", "Gus", "Jesse", "Walter", "Skyler"]
kisi = "Walter"
for kisi in uyeler:
    if kisi == "Walter":
        print("walter iceri girmeye calisiyor engelleyin")
    else:
        print(f"hos geldiniz {kisi} iceri girin")

#for ucuncusu

toplam = 20

for gun in range(1, 5):
    toplam = toplam + 5
    print(f"{gun} gun sonra ve 5 lira yatirildiginda para {toplam} ")

print(f"{gun} sonunda mevcut para {toplam}")
```
##### --- sablon ilk bolum
```mermaid
graph TD
    A[Başla: Üyeler Listesi] --> B(Sıradaki Üyeyi Al)
    B --> C{Üye == 'Walter'?}
    C -- Evet --> D[Engelleme Mesajı Yazdır]
    C -- Hayır --> E[Hoş Geldiniz Mesajı Yazdır]
    D --> F{Liste Bitti mi?}
    E --> F
    F -- Hayır --> B
    F -- Evet --> G[Bitti]
```
##### --- sablon ikinci bolum
```mermaid
graph TD
    A[Sonsuz Döngüye Gir: True] --> B[/Kullanıcıdan Komut Al/]
    B --> C{Komut == 'kapat'?}
    C -- Evet --> D[break: Döngüyü Kır]
    C -- Hayır --> B
    D --> E[Döngüden Çık ve 'Kapatıldı' Yazdır]
```
#### --- FOR CONTINUE BREAK --- [18.02.2026_and_19.02.2026]
##### --- ilk bolum
```py
for sayi in range(1, 16):
    if sayi != 7:
        print(f"sayi: {sayi}")
        continue
```
##### --- ikinci bolum
```py
stoklar = [15, 20, 5, 0, 10, 30]

for stok in stoklar:
    if stok == 0:
        break
    print(f"stoklardaki mevcut sayi {stok}")
```
##### --- ucuncu bolum
```py
veriler = [100, 200, "HATA", 300, "VIRUS", 400, 500]

for veri in veriler:
    if veri == "HATA":
        continue
    if veri == "VIRUS":
        break

    print(f"veriler isleniyor {veri}")
```
##### --- dorduncu bolum
```py
kuyruk_q = ["Sivil_1", "HATA", "Diplomat", "KACAKCI", "Sivil_2", "Sivil_3", "Sivil_4", "BOMBACI", "Sivil_5"]
for kuyruk_a in kuyruk_q:
    
    if kuyruk_a == "HATA":
        continue
    
    if kuyruk_a == "Diplomat":
        print(f"ust yetkili bolgesne gonderiliyorsunuz! {kuyruk_a} bey")

    if kuyruk_a == "KACAKCI":
        print(f"Giris reddedildi suphel sahis {kuyruk_a}")
        continue

    if kuyruk_a == "BOMBACI":
        print("GUVENLIK AYARI SISTEM KAPATILDI")
        break

    print(f"kuyruktaki sahis {kuyruk_a}")
```
##### --- ilk sablon bolum
```mermaid
graph TD
    A[Başla: Kuyruk Listesi] --> B(Sıradaki Kişiyi Al: kuyruk_a)
    B --> C{kuyruk_a == 'HATA'?}
    C -- Evet: continue --> B
    C -- Hayır --> D{kuyruk_a == 'Diplomat'?}
    D -- Evet --> E[Üst Yetkili Bölgesine Gönder]
    E --> I
    D -- Hayır --> F{kuyruk_a == 'KACAKCI'?}
    F -- Evet: continue --> G[Giriş Reddedildi Yazdır]
    G --> B
    F -- Hayır --> H{kuyruk_a == 'BOMBACI'?}
    H -- Evet: break --> J[SİSTEM KAPATILDI]
    H -- Hayır --> I[Sahıs Kabul Edildi Yazdır]
    I --> K{Kuyruk Bitti mi?}
    K -- Hayır --> B
    K -- Evet --> L[Bitti]
    J --> L
```
#### --- BREAK FOR RANGE --- [20.02.2026_and_21.02.2026]
##### --- ilk bolum
```py
 Bina_A = ["Kat_1", "Kat_2"]

for Bina_B in Bina_A:
    print(f"suanki bina {Bina_B}")

    for Bina_C in range(1, 4):
        print(f"{Bina_B} - {Bina_C}")
```
##### --- ikinci bolum
```py
gunler = ["Pazartesi", "Sali"]
saatler = ["Sabah", "Aksam"]
for gun in gunler:
    for saat in saatler:
        if gun == "Sali" and saat == "Aksam":
            print(f"{gun} ve {saat} dolasiyla vardiya bitdi sinir kapisi kapatildi")
        else:
            print(f"{gun} ve {saat} kaydi yapildi")
```
##### --- ucuncu bolum
```py
bulundu = False

for x in range(4):
        print(f"Koordinat: ({x}, {y})")
        
        if x == 2 and y == 2: 
            print(f"--- HEDEF BULUNDU ({x},{y}) ---")
            bulundu = True
            break
            
    if bulundu:
        print("Sistem tamamen kapatiliyor...")
        break
```
##### --- dorduncu bolum
```py

Crazy_8_bulundu = False

for evler in range(1, 4):
    for odalar in range(1, 3):
        print(f"ev ve odalar kontrol ediliyor ({evler}, {odalar})")

        if evler == 2 and odalar == 1:
            print(f"HIRSIZ BULUNDU ! ({evler}, {odalar}) Bolgede Yakalandi")
            Crazy_8_bulundu = True
            break
    if Crazy_8_bulundu == True:
        print("Operasyon Sonlaniyor")
        break
```
##### --- besinci bolum 
```py
dogru_sifre = "2025"
girilen_sifre = ""


while girilen_sifre != dogru_sifre:
    girilen_sifre = input("Sifreyi girin: ")
    
    if girilen_sifre != dogru_sifre:
        print("Sifre tekrar yazin")
    else:
        print("Sifre dogru sistem tamamen acildi")
    
sistem_aktif = True
kamyonlar = ["Kamyon_1", "Kamyon_2", "Kamyon_3"]
icerik = ["Normal", "KACAKCI", "Normal", "BOMBACI", "Normal"]

for kamyon in kamyonlar:
    if not sistem_aktif:
        break
    for koli in icerik:
        print(f"{kamyon} ve koli {koli} taraniyor...")
        if koli == "KACAKCI":
            print(F"DIKKAT: {kamyon} daki koli {koli} bulundu denetim aranma yapiliyor")
        elif koli == "BOMBACI":
            print("UYARI SISTEM KAPANIYOR !")
            sistem_aktif = False
            break
```
##### --- ilk sablon bolum
```mermaid
graph TD
    Start([Dış Döngü Başla]) --> Inner([İç Döngü Başla])
    Inner --> Check{Hedef Bulundu mu?}
    Check -- Evet --> Flag[Bayrak = True]
    Flag --> Break1[İç Döngüyü Kır: break]
    Break1 --> OuterCheck{Bayrak True mu?}
    Check -- Hayır --> Inner
    OuterCheck -- Evet --> Break2[Dış Döngüyü Kır: break]
    OuterCheck -- Hayır --> Start
    Break2 --> End([Operasyon Bitti])
```
### --- V BOLUM: SOZLUKLER --- [23.02.2026-07.02.2026]
#### --- V_A BOLUM: TEMEL SOZLUKLER --- [23.02.2026-07.02.2026]
##### --- KEY {} VALUE [] --- [23.01.2026]
###### --- ilk bolum
```py
yolcu = {
    "ad": "Dawut",
    "soyad": "Gociyew",
    "pasaport_no": "123456",
    "yas": "16"
}

print(yolcu["ad"])
print(yolcu["pasaport_no"])

###### --- ilk bolum gelistirilmis hali 

yolcu = {
    "ad": "Dawut",
    "soyad": "Gociyew",
    "pasaport_no": "123456",
    "yas": "16"
}

print(f"Yolcu adi: {yolcu['ad']} | pasaport {yolcu['pasaport_no']}")
```
###### --- ikinci bolum
```py
yolcu = {
    "ad": "Dawut",
    "soyad": "Gociyew",
    "pasaport_no": "123456",
    "yas": "16"
}

print(f"Yolcu adi: {yolcu['ad']} | pasaport {yolcu['pasaport_no']}")
print(f"Yolcunun eski yasi {yolcu['yas']}")
yolcu["yas"] = 19

yolcu["ulke"] = "Turkmenistan"

print(f"yolcunun yeni yasi {yolcu['yas']}  | suanki yasadigi ulke {yolcu['ulke']} ")
```
###### --- ucuncu bolum
```py
yolcu_kart = {
    "ad": "Walter",
    "bagaj_kg": 20,
    "vize": False,
}

print(f"yolcunun ismi {yolcu_kart['ad']} ve bagaj kg {yolcu_kart['bagaj_kg']}")

yolcu_kart["bagaj_kg"] += 5

yolcu_kart["kontrol_noktasi"] = "Terminal-A"


print(f"Yolcunun guncel adi {yolcu_kart['ad']} bagacin agrami {yolcu_kart['bagaj_kg']} ve bulundugu terminal {yolcu_kart['kontrol_noktasi']}") 

yolcu_kart ["yeni_kisi"] = "Pinkman"

yolcu_kart ["kamera_sistemi"] = "Terminal-A_1294"
print(f"{yolcu_kart['ad']} yanindaki sahis {yolcu_kart['yeni_kisi']} terminalin yanindaki {yolcu_kart['kamera_sistemi']} yanindaki kameradan kayitlara karismistir ")
```
###### --- dorduncu bolum
```py
yolcu_kart = {
    "ad": "Walter",
    "bagaj_kg": 20,
    "vize": False,
}

print(f"yolcunun ismi {yolcu_kart['ad']} ve bagaj kg {yolcu_kart['bagaj_kg']}")

yolcu_kart["bagaj_kg"] += 5

yolcu_kart["kontrol_noktasi"] = "Terminal-A"


print(f"Yolcunun guncel adi {yolcu_kart['ad']} bagacin agrami {yolcu_kart['bagaj_kg']} ve bulundugu terminal {yolcu_kart['kontrol_noktasi']}") 

yolcu_kart["yeni_kisi"] = "Pinkman"

yolcu_kart["kamera_sistemi"] = "Terminal-A_1294"
print(f"{yolcu_kart['ad']} yanindaki sahis {yolcu_kart['yeni_kisi']} terminalin yanindaki {yolcu_kart['kamera_sistemi']} yanindaki kameradan kayitlara karismistir ")

yolcu_kart["???"] = "___"

print(f"Walter ve yanindaki sahis pinkmandan sonra {yolcu_kart['???']}k gecmistir kendisi Walter bacanagi oldugu dusunulmekte kamera kaydi {yolcu_kart['kamera_sistemi']} kayiplara karisilmistir")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    A[Başla: yolcu Sözlüğü] --> B[Eski Yaşı Yazdır: 16]
    B --> C["Güncelleme: yolcu['yas'] = 19"]
    C --> D["Ekleme: yolcu['ulke'] = 'Turkmenistan'"]
    D --> E[f-string ile Yeni Verileri Yazdır]
    E --> F[Bitti]
```
###### --- ikinci sablon bolum
```mermaid
graph TD
    A[Başla: yolcu_kart 'Walter'] --> B[Mevcut Bilgileri Yazdır]
    B --> C["Artırma: bagaj_kg += 5"]
    C --> D["Ekleme: 'kontrol_noktasi' = 'Terminal-A'"]
    D --> E["Ekleme: 'yeni_kisi' = 'Pinkman'"]
    E --> F["Ekleme: 'kamera_sistemi' = 'Terminal-A_1294'"]
    F --> G["Ekleme: '???' = '___'"]
    G --> H[Final Senaryosunu f-string ile Yazdır]
    H --> I[Bitti]
```
##### --- POP() GET() DEL() --- [25.01.2026]
###### --- ilk bolum
```py
iste gemini

envanter = {
    "Urun": "Mavi kristal",
    "Miktar": "50 Gram",
    "lokasyon": "Karavan",
}

print("--- BILGILER GUNCELLENIYOR ---")

for deger, miktar in envanter.items():
    print(f"bilgiler araniyor {deger}  {miktar}")
print("UYARI HANK KAYITLARA BAKMAYA CALISIYOR")
envanter["Miktar"] = "100 Gram"
print("")
if "lokasyon" in envanter:

    del envanter["lokasyon"]

print("\n [UYARI] KAYITLAR SILINIYOR")

print(f"suan {envanter['Urun']} var ve miktar olarak {envanter['Miktar']} kadar gram var ")

print("Hank durumu anlamadi ama birakmayacak kotu tarafi mike jessie ariyor")
```
###### --- ikinci bolum
```py
yolcu = {
    "isim": "Saul",
    "vize": "Var",
}

yas_bilgisi = yolcu.get("Yas", "Bilgisi kayitli degil")
print(f"Kullnanici yas bilgisi {yas_bilgisi}")

if "vize" in yolcu:
    silinen_sey = yolcu.pop("vize")
    print("uzgunuz ama vizeniz iptal edildi")

print(f"bay {yolcu['isim']} suan vizeniz iptal edildi geri donmek zorundasiniz")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    A[Başla: yolcu Sözlüğü Tanımlandı] --> B["yolcu.get('Yas') Kontrolü"]
    B --> C{Yaş Bilgisi Var mı?}
    C -- Hayır --> D[Varsayılan Mesajı Ata: 'Bilgisi kayıtlı değil']
    C -- Evet --> E[Yaş Değerini Ata]
    D --> F[Yaş Bilgisini Yazdır]
    E --> F
    F --> G{"'vize' in yolcu? (Kontrol)"}
    G -- Evet --> H["yolcu.pop('vize') (Sil ve Değeri Al)"]
    H --> I[İptal Mesajını Yazdır]
    G -- Hayır --> J[Son Durumu Yazdır]
    I --> J[Bay Saul Geri Dönmek Zorundasınız]
    J --> K[Bitti]
```
##### --- UPDATE() CLEAR() --- [27.01.2026]
###### --- ilk bolum
```py
jessi_evi = {
    "evdeki_konak": "Walter",
    "mavi_stok": 500,
}

yeni_bilgiler = {
    "evin_sahibi": "Jessi",
    "lokasyon": "Colbuquerque",
    "durum": "Gizli"
}

jessi_evi.update(yeni_bilgiler)

jessi_evi["evdeki_konak"] = "Asci"
guvenlik_seviyesi = jessi_evi.get("guvenlik", "Güvenlik seviyesi atanmamiş")
print(f"gecici olarak {guvenlik_seviyesi}")
if "lokasyon" in jessi_evi:
    silinen_lokasyon = jessi_evi.pop("lokasyon")
    print(f"{silinen_lokasyon} lokasyon silindi nerede oldugu bilinmiyor")

print(f"guvenlik durum suan {yeni_bilgiler['durum']} hadi {jessi_evi['evdeki_konak']} biraz met yapalim")

jessi_evi["evdeki_konak"] = "Walter White"
yeni_bilgiler["evin_sahibi"] = "Jessie Pinkman"

print(f" mike elindeki kayitli bilgiler {jessi_evi}")
```
###### --- ikinci bolum
```py
jessi_evi = {
    "evdeki_konak": "Walter",
    "mavi_stok": 500,
}

yeni_bilgiler = {
    "evin_sahibi": "Jessi",
    "lokasyon": "Colbuquerque",
    "durum": "Gizli"
}

jessi_evi.update(yeni_bilgiler)

jessi_evi["evdeki_konak"] = "Asci"
guvenlik_seviyesi = jessi_evi.get("guvenlik", "Güvenlik seviyesi atanmamiş")
print(f"gecici olarak {guvenlik_seviyesi}")
if "lokasyon" in jessi_evi:
    silinen_lokasyon = jessi_evi.pop("lokasyon")
    print(f"{silinen_lokasyon} lokasyon silindi nerede oldugu bilinmiyor")

print(f"guvenlik durum suan {yeni_bilgiler['durum']} hadi {jessi_evi['evdeki_konak']} biraz met yapalim")

jessi_evi["evdeki_konak"] = "Walter White"
yeni_bilgiler["evin_sahibi"] = "Jessie Pinkman"

print(f" mike elindeki kayitli bilgiler {jessi_evi}")

jessi_evi.clear()
print(f"Mike kanitlari yok etdi: {jessi_evi}")
print(f"dis bilgi hala duruyormu: {yeni_bilgiler}")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    Start([Başla]) --> Define[Sözlükler Tanımlandı: jessi_evi ve yeni_bilgiler]
    Define --> Update["jessi_evi.update(yeni_bilgiler)"]
    Update --> Change["evdeki_konak = 'Asci'"]
    Change --> Get["guvenlik_seviyesi = .get('guvenlik')"]
    Get --> Check{lokasyon anahtarı var mı?}
    Check -- Evet --> Pop["silinen_lokasyon = .pop('lokasyon')"]
    Check -- Hayır --> Print[Bilgileri Yazdır]
    Pop --> Print
    Print --> FinalUpdate["Veriler Son Kez Güncellendi"]
    FinalUpdate --> Clear["jessi_evi.clear()"]
    Clear --> End([Bitti: Kanıtlar Yok Edildi])
```
#### --- V_B BOLUM: GELISTIRILMIS SOZLUKLER [02.02.2026-07.02.2026]
##### --- NESTED DICTIONARIES --- [02.03.2026]
###### --- ilk bolum
```py
sehir = {
    "ev_1": {"isim": "Saul", "para": 10000},
    "ev_2": {"isim": "Gus", "para": 50000}
}
para = sehir["ev_2"]["para"]
print(f"{sehir['ev_2']['isim']} parasi {para}")
```
###### --- ikinci bolum
```py
sehir = {
    "ev_1": {"isim": "Saul", "para": 10000},
    "ev_2": {"isim": "Gus", "para": 50000},
}

sokak = {
    "ev_3": {"isim": "Mike", "para": 30000}
}
sehir.update(sokak)
sehir["ev_1"]["para"] = 25000
print(f"Saul mike'dan rusvet aldi suanki para {sehir['ev_1']['para']}")
sehir["ev_3"]["para"] = 15000
print(f"Mike saul rusvet verdi suanki mevcut para {sehir['ev_3']['para']}")

ev_4 = sehir.get("guvenli ev", "guvenli olmayan ev")
print(f"malesef {ev_4} bulunamadi ")


para_1 = sehir["ev_2"]["para"]
print(f"{sehir['ev_2']['isim']} parasi {para_1}")
para_2 = sehir["ev_1"]["para"]
print(f"{sehir['ev_1']['isim']} parasi rusvet sayesinde {para_2}")
para_3 = sehir["ev_3"]["para"]
print(f"{sehir['ev_3']['isim']} parasi saul rusvet verdigi icin {para_3}")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    A[Başla: sehir ve sokak Sözlükleri Tanımlandı] --> B["sehir.update(sokak) <br/>(Mike şehre dahil oldu)"]
    B --> C["Güncelleme: ev_1 (Saul) para = 25000 <br/>(Rüşvet Alındı)"]
    C --> D["Güncelleme: ev_3 (Mike) para = 15000 <br/>(Rüşvet Verildi)"]
    D --> E["sehir.get('guvenli ev') Kontrolü"]
    E --> F{Kayıt Var mı?}
    F -- Hayır --> G["Varsayılan Değer: 'guvenli olmayan ev'"]
    F -- Evet --> H[Kayıtlı Değeri Getir]
    G --> I[f-string ile Güncel Bakiyeleri Yazdır]
    H --> I
    I --> J[Sonuç: Saul, Gus ve Mike'ın Paraları Raporlandı]
    J --> K[Bitti]
```
##### --- LIST DICTIONARIES --- [04.03.2026]
###### --- ilk bolum
```py
yolcular = [
    {"isim": "Mike", "para": 10000}
]

yolcular.append({"isim": "Gus", "para": 50000}) 
yolcular.append({"isim": "Walter", "para": 22000})

print(yolcular)
print(f"Ozel yolcular {yolcular[0]}")
```
###### --- ikinci bolum
```py
yolcular = [
    {"isim": "Mike", "para": 10000}
]

yolcular.append({"isim": "Gus", "para": 50000}) 
yolcular.append({"isim": "Walter", "para": 22000})

for yolcu in yolcular:
    if yolcu["para"] >= 30000:
        print(f"{yolcu['isim']} kisinin {yolcu['para']} fazla meblasi bulunmakta")
    else:
        print(f"{yolcu['isim']} kisi ve suanki meblasi {yolcu['para']}")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    A[Başla: yolcular Listesi Oluşturuldu] --> B["Listeye Gus ve Walter Eklendi (append)"]
    B --> C[Döngü: Liste Elemanlarını Tek Tek Al]
    C --> D{Para >= 30000?}
    D -- Evet --> E["Ekrana Yaz: Yüksek Meblağ (Gus)"]
    D -- Hayır --> F["Ekrana Yaz: Normal Meblağ (Mike/Walter)"]
    E --> G{Başka Yolcu Var mı?}
    F --> G
    G -- Evet --> C
    G -- Hayır --> H[Bitti]
```
##### --- BOSS DICTIONARIES --- [06.03.2026]
###### --- ilk boss bolum
```py
kisiler = {
    "lider": "Mike",
    "yardimci": "Pinkman",
    "ek_yardimci": "Tyrus"
}

laboratuvar_verileri = [
    {"oda": 101, "calisan": "Walter", "kimyasallar": ["Metilamin", "Asit"], "miktar": 50000},
    {"oda": 102, "calisan": "Gale", "kimyasallar": ["Sülfür", "Cam Malzeme"], "miktar": 12000},
    {"oda": 103, "calisan": "Gus", "kimyasallar": ["Fenilasetik_Asit"], "miktar": 85000},
    {"oda": 104, "calisan": "Saul", "kimyasallar": ["Para"], "miktar": 5000}
]
toplam_stok = 0
for laboratuvar_listesi in laboratuvar_verileri:
    if laboratuvar_listesi["miktar"] >= 40000:
        toplam_stok = toplam_stok + laboratuvar_listesi["miktar"]
        print(F"\n KRITIK: {laboratuvar_listesi['oda']} odada ve {laboratuvar_listesi['miktar']} miktar bulunmakta labaravutari yoneten {laboratuvar_listesi['calisan']} Gus'un adamlari ve {kisiler['lider']} gonderiliyor")
        if laboratuvar_listesi["calisan"] == "Walter":
            print(f"{laboratuvar_listesi['oda']} odada {laboratuvar_listesi['calisan']} yonetiyor {kisiler['lider']} yanina destek amacli {kisiler['ek_yardimci']} gonderiliyor ")
    else:
        print(F"\n GUVENLI: {laboratuvar_listesi['oda']} oda guvenli gecici olarak {kisiler['yardimci']} gonderiliyor")
    
    for kimyasal in laboratuvar_listesi["kimyasallar"]:
        print(f" --> Bulunan madde: {kimyasal}")

print(f"toplam stok {toplam_stok}")
```
###### --- ilk boss sablon bolum
```mermaid
graph TD
    A[Başla] --> B[Verileri Tanımla]
    B --> C[Döngü: Her Oda İçin]
    C --> D{Miktar >= 40000?}
    D -- Evet --> E[Stoğa Ekle & Mike'ı Gönder]
    E --> F{Çalışan Walter mı?}
    F -- Evet --> G[Tyrus'u Desteğe Gönder]
    F -- Hayır --> H[İç Döngü: Kimyasalları Yazdır]
    D -- Hayır --> I[Pinkman'ı Gönder]
    G --> H
    I --> H
    H --> J{Tüm Odalar Bitti mi?}
    J -- Hayır --> C
    J -- Evet --> K[Toplam Stoğu Yazdır & Bitir]
```
### --- VI BOLUM: FONKSIYONLAR --- [09.03.2026-03.04.2026]
#### --- VII_A BOLUM: BASLANGIC FONKSIYONLAR --- [09.03.2026-14.03.2026]
##### --- DEF UND RETURN (ANFANG) --- [09.03.2026] 
##### --- ilk bolum
```py
def rapor_sistemi(): 
    print("kimyasallar ayrilistiriliyor")
    print("amac yapiliyor")
    print("Walter ve jessi uyusturucu basliyor")


rapor_sistemi()
```
##### --- ikinci bolum
```py
def kontrol_et(miktar):
    if miktar >= 40000:
        print(f"{miktar} miktar stok cok fazla")
    else:
        print(f"{miktar} stok var az devam")

kontrol_et(40000)
kontrol_et(50000)
kontrol_et(30000)
```
##### --- ucuncu bolum
```py
def mike_payi(toplam_miktar):
    hesap = toplam_miktar * 0.1
    return hesap

kesinti = mike_payi(50000)

print(f"mike kari: {kesinti}")

net_para = 50000 - kesinti

print(f"kesinti ve net para {net_para}") 
```
##### --- dorduncu bolum
```py
odalar = [50000, 12000, 20000]

def oda_islem(miktar):
    if miktar >= 40000:
        durum = "Kritik"
    else:
        durum = "Guvenli"
    mike_payi = miktar * 0.10
    elimizde_kalan = miktar - mike_payi
    return durum, mike_payi, elimizde_kalan

for o in odalar:
    durum, pay, kalan = oda_islem(o)
    print(f"Oda durumu: {durum} |  Mike_payi: {pay}  |  Bize kalan: {kalan}")
```
##### --- ilk ve ikinci sablon bolum
```mermaid
graph TD
    Start([Başla]) --> P1[Bölüm 1: Basit Çıktı - rapor_sistemi]
    P1 --> P2[Bölüm 2: Parametreli Kontrol - kontrol_et]
    
    P2 --> P3[Bölüm 3: Hesaplama ve return - mike_payi]
    P3 --> Var1[Değişken: kesinti = 5000]
    
    Var1 --> P4[Bölüm 4: Liste ve Çoklu return - oda_islem]
    P4 --> Loop[Döngü: Her Oda İçin]
    
    Loop --> Logic{miktar >= 40000?}
    Logic -- Evet --> Crit[Durum: Kritik]
    Logic -- Hayır --> Safe[Durum: Guvenli]
    
    Crit --> Calc[Pay & Kalan Hesapla]
    Safe --> Calc
    
    Calc --> Ret["return Durum, Pay, Kalan"]
    Ret --> Unpack["Değişkenlere Dağıt (Unpacking)"]
    Unpack --> Print[Ekrana Sonuçları Yazdır]
    
    Print --> Next{Başka Oda Var mı?}
    Next -- Evet --> Loop
    Next -- Hayır --> End([Bitti])

    style P1 fill:#f9f,stroke:#333
    style P4 fill:#bbf,stroke:#333
    style Ret fill:#dfd,stroke:#333
```
##### --- DEF --- [11.03.2026]
###### --- ilk bolum
```py
def sevkiyat_hazirla(kisi, malzeme, miktar):

    print(f"--- SEVKIYAT BIRIMI HAZIRLANDI ---")
    print(f"Gonderilen Malzeme {malzeme}")
    print(f"Miktar: {miktar} kg")
    print(f"gonderen kisi: {kisi}")
    if kisi == "GUS":
        print(f"Bay {kisi} tarafindan gonderildiniz Ozel anlasma gecebilirsiniz")
    
    elif miktar >= 500:
        print(F"UYARI: {malzeme} miktar {miktar} kg sayisi belirlenen sinirdan asiyor")
    
    else:
        print(f"gonderen kisi: {kisi} malzeme: {malzeme} miktar: {miktar} kg tamam gecebilirsiniz")

sevkiyat_hazirla("WAlTER", "Mavi Kristal", 600) 
```
###### --- ikinci bolum
```py
def laboravutar_durumu(isi, basinc, durum="Stabil"):
    if isi >= 100:
        print(f"UYARI: isi {isi} yuksek")
        if basinc >= 50:
            print(f"UYARI: basinc {basinc} yuksek")
    elif isi <= 99:
        print(f"DURUM: isi {isi} dusuk")
        if basinc <= 49:
            print(f"DURUM: basinc {basinc} dusuk")
    else:
        print("Hata")
    print(f"suanki durum: {durum}")

laboravutar_durumu(125, 75, "KRITIK")
laboravutar_durumu(50, 25)
```
###### --- ilk sablon bolum
```mermaid
graph TD
    Start([Fonksiyon Çağrıldı]) --> Input[Parametreler: isi, basinc, durum='Stabil']
    Input --> TempCheck{isi >= 100?}
    
    TempCheck -- Evet --> HighTemp[UYARI: Isı Yüksek Yazdır]
    HighTemp --> PressCheck1{basinc >= 50?}
    PressCheck1 -- Evet --> HighPress[UYARI: Basınç Yüksek Yazdır]
    PressCheck1 -- Hayır --> Status
    
    TempCheck -- Hayır --> LowTempCheck{isi <= 99?}
    LowTempCheck -- Evet --> LowTemp[DURUM: Isı Düşük Yazdır]
    LowTemp --> PressCheck2{basinc <= 49?}
    PressCheck2 -- Evet --> LowPress[DURUM: Basınç Düşük Yazdır]
    PressCheck2 -- Hayır --> Status
    
    LowTempCheck -- Hayır --> Error[Hata Yazdır]
    
    HighPress --> Status
    LowPress --> Status
    Error --> Status
    
    Status[suanki durum Yazdır] --> End([Bitti])

    style Input fill:#bbf,stroke:#333
    style TempCheck fill:#f9f,stroke:#333
    style Status fill:#dfd,stroke:#333
```
##### --- RETURN --- [13.03.2026]
###### --- ilk bolum 
```py
def saf_miktar(toplam_kg):
    hesap = toplam_kg * 0.8

    return hesap 

tuco_payi = saf_miktar(1000)

print(f"tuco nun payi {tuco_payi}")
```
###### --- ikinci bolum 
```py
def salamanca_payi(toplam_para):
    Lalo_salamanca = toplam_para * 0.50
    Tuco_salamanca = toplam_para * 0.50

    return Lalo_salamanca, Tuco_salamanca

L_S, T_S = salamanca_payi(50000)

print(f"Salamanca tuco payi: {T_S} |  Salamanca lalo payi: {L_S}")

salamanca_payi = 50000 - (L_S +T_S)

print(f"Geri kalan Salamanca payi {salamanca_payi}")

###### --- ikinci nolum sablon taslagi

def salamanca_payi_hesapla(toplam_para):
    # Fonksiyon ismini 'salamanca_payi_hesapla' yaptık ki değişkenle karışmasın
    lalo_salamanca = toplam_para * 0.50
    tuco_salamanca = toplam_para * 0.50
    return lalo_salamanca, tuco_salamanca

# 1. Fonksiyonu çağır ve değerleri yakala (Unpacking)
L_S, T_S = salamanca_payi_hesapla(50000)

# 2. Sonuçları yazdır (Dışta çift, içte tek tırnak kuralı)
print(f"Salamanca tuco payi: {T_S} | Salamanca lalo payi: {L_S}")

# 3. Kalan parayı hesapla (Değişken ismi: kalan_miktar)
kalan_miktar = 50000 - (L_S + T_S)

print(f"Geri kalan Salamanca payi: {kalan_miktar}")
```
###### --- ilk sablon bolum 
```mermaid
graph TD
    Start([Başla]) --> Call[Fonksiyon Çağrısı: 50000]
    Call --> Logic[Hesapla: 50% Lalo + 50% Tuco]
    Logic --> Return[return 25000, 25000]
    Return --> Unpack[Değişkenlere Dağıt: L_S ve T_S]
    Unpack --> Print[Ekrana Payları Yazdır]
    Print --> Calc[Hesapla: Kalan Miktar]
    Calc --> End([Bitti])

    style Call fill:#bbf,stroke:#333
    style Return fill:#dfd,stroke:#333
    style Unpack fill:#f9f,stroke:#333
```
#### --- VII_B BOLUM: TEMEL FONKSIYONLAR --- [16.03.2026-18.03.2026]
##### --- SOZLUK UND FONKSIYON --- [16.03.2026]
###### --- ilk bolum
```py
def envanter_ekle(isim, miktar, tur, kisi):
    envanter = {
        "ad": isim, 
        "adet": miktar, 
        "tip": tur,
        "ismi": kisi
    }
    
    return envanter 

depo = []

depo.append(envanter_ekle("Maske", "10", "Ekipman", "Walter"))
print("--- DEPO MALZEMELERI")
for urun in depo:
    print(f"ESYA: {urun['ad']}  |  MIKTAR: {urun['adet']}  |  TIP: {urun['tip']}  |  KISI: {urun['ismi']}")
```
###### --- ikinci bolum 
```py
def hasta_kaydet(isim, ates, yakini):
    liste = {
        "kisi": isim,
        "derece": ates,
        "tanidigi": yakini
    }

    return liste 

hastane_listesi = []

hastane_listesi.append(hasta_kaydet("Hank", 38, "Gomez"))

for hasta in hastane_listesi:
    if hasta["derece"] >= 38:
        print(f"UYARI: {hasta['kisi']} cok hasta sadece tanidik aliyoruz")
    else:
        print(f"Hasta suan iyi taburcu olabilir {hasta['tanidigi']} ")

for bilgi in hastane_listesi:
    print(f"KISI: {bilgi['kisi']}  |  DERECE: {bilgi['derece']}  |  YAKINI: {bilgi['tanidigi']}")
```
###### --- ilk sablon bolum
```mermaid 
graph TD
    Start([Başla]) --> Call[Fonksiyon Çağrısı: hasta_kaydet]
    Call --> CreateDict[Sözlük Oluştur: isim, ates, yakini]
    CreateDict --> Return[return liste]
    
    Return --> Append[hastane_listesi.append]
    Append --> Loop[Döngü: Liste Elemanlarını Tara]
    
    Loop --> Condition{derece >= 38?}
    Condition -- Evet --> Warning[Yazdır: UYARI ve Tanıdık Mesajı]
    Condition -- Hayır --> Safe[Yazdır: Taburcu Olabilir]
    
    Warning --> FinalPrint[Genel Liste Bilgilerini Yazdır]
    Safe --> FinalPrint
    
    FinalPrint --> End([Bitti])

    style Call fill:#bbf,stroke:#333
    style Return fill:#dfd,stroke:#333
    style Condition fill:#f9f,stroke:#333
```
##### --- THE FILTER LOGIC --- [17.03.2026]
##### --- ilk bolum
```py
def malzeme_ekle(isim, miktar, tip):
    liste = {
        "ad": isim,
        "sayi": miktar,
        "tipi": tip
    }

    return liste

depo = []

depo.append(malzeme_ekle("Mavi kristal", 50, "urun"))
depo.append(malzeme_ekle("Asit", 10, "Kimyasal"))
depo.append(malzeme_ekle("Maske", 5, "Ekipman"))

for depo_listesi in depo:
    if depo_listesi["sayi"] <= 10:
        print(f"UYARI: {depo_listesi['ad']} adli seyin sayi miktari {depo_listesi['sayi']} normal durumdan az")
    else:
        print(f"{depo_listesi['ad']} adli seyin miktari durumu stabil devam edelim")
```
##### --- ilk sablon bolum
```mermaid
graph TD
    Start([Başla]) --> Call1[malzeme_ekle: Mavi Kristal]
    Call1 --> Call2[malzeme_ekle: Asit]
    Call2 --> Call3[malzeme_ekle: Maske]
    
    Call1 & Call2 & Call3 --> DictGen[Sözlük Oluştur ve return Et]
    DictGen --> ListAppend[depo.append: Listeye Ekle]
    
    ListAppend --> Loop[Döngü: Depodaki Her Ürünü Tara]
    
    Loop --> Condition{sayi <= 10?}
    
    Condition -- Evet --> Warning[Yazdır: UYARI - Miktar Az]
    Condition -- Hayır --> Stable[Yazdır: Durum Stabil]
    
    Warning --> Next{Başka Ürün Var mı?}
    Stable --> Next
    
    Next -- Evet --> Loop
    Next -- Hayır --> End([Bitti])

    style Call1 fill:#bbf,stroke:#333
    style DictGen fill:#dfd,stroke:#333
    style Condition fill:#f9f,stroke:#333
```
##### --- hastalandigim icin dinlendim --- [18.03.2026]
#### --- VII_C BOLUM: GELISMIS FONKSIYONLAR --- [23.03.2026-03.04.2026]
##### --- RETURN VS PRINT --- [23.03.2026{and}30.03.2026]
###### --- ilk bolum
```py
def durum_kontrol(ates):
    if ates >= 38:
        return "KRITIK"
    else:
        return "STABIL"

def mudahale_et(durum):
    if durum == "KRITIK":
        print("Acil gonderme")
    else:
        print("Durum stabil")
    
rapor = durum_kontrol(37.5)
mudahale_et(rapor)
```
###### --- ikinci bolum
```py
def envanter_ozeti(esya_adeti, adet):
    if adet <= 5:
        durum = "KRITIK"
    else:
        durum = "STABIL"
    
    return esya_adeti, adet, durum

esya, sayi, sonuc = envanter_ozeti("ILAC", 7)

print(f"esyanin kendisi {esya}  |  esyanin sayisi {sayi}  | ve sonucu {sonuc}")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    Start([Başla]) --> Call1[durum_kontrol: 37.5]
    
    subgraph Karar_Merkezi
    Call1 --> Logic1{ates >= 38?}
    Logic1 -- Evet --> Ret1[return 'KRITIK']
    Logic1 -- Hayır --> Ret2[return 'STABIL']
    end
    
    Ret2 --> Var[Değişken: rapor]
    
    Var --> Call2[mudahale_et: rapor]
    
    subgraph Aksiyon_Merkezi
    Call2 --> Logic2{durum == 'KRITIK'?}
    Logic2 -- Evet --> Print1[Yazdır: Acil Gonderme]
    Logic2 -- Hayır --> Print2[Yazdır: Durum Stabil]
    end
    
    Print2 --> End([Bitti])

    style Call1 fill:#bbf,stroke:#333
    style Var fill:#f9f,stroke:#333
    style Print2 fill:#dfd,stroke:#333
```
###### --- bir hafta hastalandim --- [24.03.2026-29.03.2026]
###### --- ilk bolum 
```py
def muvekkel_isle(ad, durum_kodu):

    if durum_kodu == 1:
        durum = "Masum"
    elif durum_kodu == 2:
        durum = "Suclu"
    elif durum_kodu == 3:
        durum = "supheli"
    else:
        durum = "Bilinmiyor"
    return ad, durum_kodu, durum

isim, bilgi, durum = muvekkel_isle("Micheal", 4)
print(f"Sahsin ismi: {isim}  |  sahsin kodu: {bilgi}  |  ve suanki durumu: {durum}")
```
###### --- ikinci bolum
```py
def muvekkel_isle(ad, durum_kodu):
    
    if durum_kodu == 1:
        durum = "Masum"
    elif durum_kodu == 2:
        durum = "Suclu"
    elif durum_kodu == 3:
        durum = "supheli"
    else:
        durum = "Bilinmiyor"
    return ad, durum_kodu, durum

muvekkil_listesi = [["Mike", 1], ["Gustavo", 4], ["Lalo", 3], ["Nacho", 3]]

for ad_verisi, kod_verisi in muvekkil_listesi:
    isim, sonuc, durum = muvekkel_isle(ad_verisi, kod_verisi)
    print(f"ismi: {isim}  | sonuc: {sonuc}  | ekstra bilgi: {durum}")
```
###### --- ucuncu bolum 
```py
def sevkiyat_kontrol(kova_id, paket_sayisi):
    if paket_sayisi <= 0:
        durum = "TEMIZ  |  RISK_YOK"
    elif paket_sayisi >= 1 and paket_sayisi <= 2:
        durum = "KIRLI  |  RISK_ORTA"
    elif paket_sayisi  >= 3:
        durum = "TEHLIKELI  |  RISK_YUKSEK"
    else:
        durum = "BILINMIYOR  |  RISK_???"

    return kova_id, paket_sayisi, durum

sevkiyat_verisi = [["Kova-A", 0], ["Kova-B", 2], ["Kova-C", 5], ["Kova-D", 1]]

for sev_kontrol, sev_kodu in sevkiyat_verisi:
    ad, sonuc, durum = sevkiyat_kontrol(sev_kontrol, sev_kodu)
    print(f"Sevkiyatin ismi: {ad}  |  sevkiyatin bilgi: {sonuc}  | sevkiyatin sonucu: {durum}")
```
##### --- *ARGS UND **KWARGS --- [01.04.2026]
###### --- ilk bolum
```py
def  francesca_listesi(*isimler):
    for liste in isimler:
        print(f"Iceri giren muvekiller listesi {liste}")


francesca_listesi("Jessi", "Walter", "Skyler")

francesca_listesi("Kisi_1", "Kisi_2", "Kisi_3", "Kisi_4", "Kisi_5", "Kisi_6")
```
###### --- ikinci bolum
```py
yani iste 

def Miami_metro_polisi(Ofis_lideri, *Kisiler, **Detaylar):
    print(f"Ofis Lideri: {Ofis_lideri}")

    print("Supheliler:")

    for tanik in Kisiler:
        print(f"{tanik}")

    print("DETAYLAR:")
    for anahtar, deger in Detaylar.items():
        print(f"{anahtar}  |  {deger}")


Miami_metro_polisi("Dexter", "Angel", "Vince", durum = "Normal", Rozet = "Polis")
```
###### --- ucuncu bolum
```py
def sevkiyat_merkezi(sorumlu, *uyusturucular, **ozellikler):
    print(f"Sevkiyatin Sorumlusu: {sorumlu}")
    
    print("Uyusturucu turleri:")

    for ozel in uyusturucular:
        print(f"{ozel}")
    
    print("Ozellikleri:")
    
    for etki, olayi in ozellikler.items():
        print(f"etkisi: {etki}  |  olayi: {olayi}")


sevkiyat_merkezi("Mike", "Mavi_meth", "Fetametamin", "Sari_meth", Kafa_bulama = "fena_rahatlama", Ishal= "Olumcul")
```
###### --- ilk sablon bolum
```mermaid
graph TD
    Start([Fonksiyon Çağrıldı]) --> Input["Giriş Verileri"]
    
    subgraph Paketleme_Merkezi
    Input --> P1["sorumlu: 'Mike' (Standart)"]
    Input --> P2["*uyusturucular: ('Mavi_meth', 'Fetametamin', 'Sari_meth') (Tuple)"]
    Input --> P3["**ozellikler: {'Kafa_bulama': 'fena_rahatlama', 'Ishal': 'Olumcul'} (Dict)"]
    end
    
    P1 --> Print1[Yazdır: Sorumlu İsmi]
    
    P2 --> Loop1[Döngü: Liste Elemanlarını Tek Tek Yazdır]
    Loop1 --> Next1{Başka Tür Var mı?}
    Next1 -- Evet --> Loop1
    
    P3 --> Loop2["Döngü: Anahtar/Değer (items) Çiftlerini Yazdır"]
    Loop2 --> Next2{Başka Özellik Var mı?}
    Next2 -- Evet --> Loop2
    
    Next1 -- Hayır --> Next2
    Next2 -- Hayır --> End([Bitti])

    style P2 fill:#f9f,stroke:#333
    style P3 fill:#bbf,stroke:#333
    style DictGen fill:#dfd,stroke:#333
```
##### --- HATA VE SON --- [03.04.2026]
###### --- ilk karmasik bolum
```py
Saul_verileri = [
    ["Gustavo", 1],
    ["Walter", 1],
    ["Jessie", 2],
    ["Mike", 2],
    ["Lalo", 3]
]

def Saul_dosyasi(isim, kod):
    if kod == 1:
        durum = "Dosya_Temiz"
    elif kod == 2:
        durum = "Dosya_Supheli"
    elif kod == 3: 
        durum = "Dosya_Riskli"
    else:
        durum = "Bilinmiyor"

    return durum

def saul_arsivi(sorumlu_avukat, *muvekkiller, **ekstra_notlar):
    print(f"muvekkilerin avukati: {sorumlu_avukat}")

    print(f"{sorumlu_avukat}''un Muvekkili: ")

    for kisi in muvekkiller:
        print(f"{kisi}")

    print("Muvekkilin ekstra bilgileri: ")

    for sehir, oncelik in ekstra_notlar.items():
        print(f"{sehir}: {oncelik} ")

for dosya_incele in Saul_verileri:
    isim_verisi = dosya_incele[0]
    kod_verisi = dosya_incele[1]

    durum = Saul_dosyasi(isim_verisi, kod_verisi)

    print(f"Muvekkil: {isim_verisi}  | Durum: {durum}")


saul_arsivi("Saul Goodman", "Gustavo", "Walter", "Jessie", "Mike", "Lalo", sehir="Albuquerque", Oncelik="Kritik")
```
###### --- ikinci karmasik bolum
```py
# --- LISTELER ---

# ["Araç_Tipi", "Yük_Miktarı", "Güvenlik_Seviyesi"]
konvoy_listesi =  [
    ["Normal_Kamyon", 500, "Yuksek"],
    ["Normal_Araba", 300, "Normal"],
    ["Motosiklet", 50, "Dusuk"],
    ["Arazi_araba", 450, "Normal-Yuksek"],
    ["Buyuk_Kamyon", 1000, "Max_Yuksek"],
    ["kucuk_araba", 200, "Normal"]
]

# --- FONKSIYON + KARAR MEKANIZMASI ---

def rota_belirle(Yuk_miktari, Guvenlik_listesi):
    if Yuk_miktari >= 400 and Guvenlik_listesi == "Yuksek" or Guvenlik_listesi == "Max_Yuksek":
        durum = "A Rotali Ana yol"
    elif Yuk_miktari <= 399 and Guvenlik_listesi == "Normal" or Guvenlik_listesi == "Normal-Yuksek":
        durum = "B Rotali Yan yol"
    else:
        durum = "C Rotali Arka yol"

    return durum 

# --- FONKSIYON + RAPOR VERI

def lalo_ozet(K_Lider, *araclar, **Detaylar):
    print(f"Konvoy'un Lideri: {K_Lider}")

    for arac in araclar:
        print(f"Konvoy'daki Araclar: {arac}")

    for ein, zwei in Detaylar.items():
        print(f"Detay -> {ein}: {zwei}")
    
# --- SON DONGU + BUYUK OPERASYON
for bilgi in konvoy_listesi:
    isim = bilgi[0]
    miktar = bilgi[1]
    guvenlik = bilgi[2]
    yol = rota_belirle(miktar, guvenlik)

    print(f"Arac: {isim}  |  miktar: {miktar}  |  guvenlik: {guvenlik}  |  Rota: {yol}")

print("-" * 10)

lalo_ozet("Lalo_Salamanca", "Normal_Kamyon", "Normal_Araba", "Motosiklet", "Arazi_araba" ,"Buyuk_Kamyon", "kucuk_araba",hedef="El_Paso", hava="Gunesli")
```
###### --- ucuncu karmasik bolum
```py
Salamanca_listesi = [
    ["Lalo", 38, "Salamanca",],
    ["Varga", 32, "Nacho"],
    ["Tuco", 31, "Salamanca",],
    ["Hector", 64, "Salamanca",],
    ["Saul", 32, "Goodman"]
]

def Cartel_verisi(isim,yas,soyisim):
    if isim == "Saul" and yas >= 30 and soyisim == "Goodman":
        sonuc = "Salamanca ailesinin Avukati"
    elif isim == "Varga" and yas >= 31 and soyisim == "Nacho":
        sonuc = "Salamanca ailesinin sag kolu"
    else:
        sonuc = ("Salamanca ailesinin uyeleri")

    return sonuc

def Cartel_ozeti(C_Lideri, *kisiler, **Detaylar):
    print(f"Cartelin En Onemli Kisi: {C_Lideri}")

    for kisi in kisiler:
        print(f"Kisiler -> {kisi}")

    for baslik, icerik in Detaylar.items():
        print(f"Detay -> {baslik}: {icerik}")

for bilgi in Salamanca_listesi:
    isim_v = bilgi[0]
    yas_v = bilgi[1]
    soyisim_v = bilgi[2]

    analiz = Cartel_verisi(isim_v, yas_v, soyisim_v)

    print(f"isim: {isim_v}  |  yas: {yas_v}  |  soyisim: {soyisim_v}  |  Rol: {analiz}")

print("-" * 30)
Cartel_ozeti("Hector", "Nacho", "Tuco", "Lalo", "Saul", hedef="Gus Fring", durum="Sili'li tehdit altinda")
```
###### --- ilk karmasik sablon bolum
```mermaid
graph TD
    Start([Operasyon Başladı]) --> List[Konvoy Listesi Tanımlandı]
    List --> Loop[Döngü: Her Araç Bilgisini Al]
    
    subgraph Karar_Mekanizmasi [Rota Belirleme Merkezi]
        Loop --> Calc{Rota Belirle}
        Calc -- "Yük >= 400 & Güvenlik Yüksek" --> RotaA[A Rotası: Ana Yol]
        Calc -- "Yük <= 399 & Güvenlik Normal" --> RotaB[B Rotası: Yan Yol]
        Calc -- "Diğer Durumlar" --> RotaC[C Rotası: Arka Yol]
    end
    
    RotaA & RotaB & RotaC --> Print1[Araç ve Rota Bilgisini Yazdır]
    Print1 --> Loop
    
    Loop -- "Tüm Araçlar Bitti" --> Summary[Fonksiyon: lalo_ozet]
    
    subgraph Dinamik_Raporlama [Args ve Kwargs İşleme]
        Summary --> P1[Lideri Yazdır]
        P1 --> P2["*araclar: Sınırsız Araç Listesi Yazdır"]
        P2 --> P3["**Detaylar: Hedef ve Hava Durumu Yazdır"]
    end
    
    P3 --> End([Görev Tamamlandı])

    style Karar_Mekanizmasi fill:#f5f5f5,stroke:#333
    style Dinamik_Raporlama fill:#e1f5fe,stroke:#01579b
    style Calc fill:#fff9c4,stroke:#fbc02d
```

# --- BIRINCI KISMIN SONU--THE END ?
## ILK BOLUM BITDI VE BIRINCI KISIM YAPILDI
## PYTHON ILK KEZ BASLADIDIGIMDA [01.01.2026] AMA 25 GUN BOYUNCA 2 DEFA BASARIZ OLDUM VE KAYITLARIMI SILDIM GERI GETIREMEDIGIM ICIN 3 KENDIME SON DEFA DIYEREK [26.01.2026] BASLADIM VE IKINCI DEFA 1 KISMI BITIRDIM 
## BUNDAN SONRA ANFANG DOSYA YERINE AUFBAU DOSYADAN DEVAM ETMEK ONUDA KAYDETMEYE BASLIYACAGIM 
## ISIM:DAWUT
## SOYISIM:GOCIYEW
## AMACIM: TURKIYEDE YAZILIM MUHENDISLIGI BITIRIP ALMANYA'DA MAVI KARTLA ORAYA GIDIP CALISAMK VE VATANDASLIGA BASVURMAK
## SUANKI AMACIM: [2026-2028] ARASINDAKI 4 ONEMLI SUTUN OLAN (TKEO) BITIRMEK VE BACKEND GELISTIRICISI OLMAK 
### Temmuz 2026,Python & Algoritma,Temeli Çelik Gibi Yapmak -- T
### Kasım 2026,SQL & Veritabanı,Verinin Kalbine İnmek -- K
### Eylül 2027,Java & Spring Boot,Almanya Bileti (En Kritik Aşama) -- E
### Ocak 2028,Linux & Docker,Sistem Altyapısı (DevOps Giriş) -- O