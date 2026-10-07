# BlokBa

**Od prvog bloka do pravog Python programa — u jednoj aplikaciji.**

BlokBa je besplatna aplikacija za nastavu programiranja u osnovnoj školi.
Đaci slažu blokove, a blokovi se **uživo prevode u pravi Python kod** koji se
odmah izvršava. Kad dođe vrijeme za tekstualno programiranje, đaci ostaju u
istoj aplikaciji: isti prozor, isti terminal, isti pomoćnik — samo što sada
kod pišu sami.

Radi **potpuno bez interneta**, na Windowsu i Linuxu, i na starijim
računarima.

> **Bosanski** · [Hrvatski](README.hr.md) · [English](README.en.md) · [Deutsch](README.de.md)

<img width="1423" height="892" alt="BlokBa — blokovi i Python kod jedan pored drugog" src="https://github.com/user-attachments/assets/18916c19-89f8-4980-aeb8-12acf0f05402" />

---

## Preuzimanje

Najnovija verzija: **[BlokBa 2.0.0](../../releases/latest)**

| Sistem | Preuzimanje | Napomena |
|---|---|---|
| Windows 10/11 | **[BlokBa-2.0.0-Setup.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-2.0.0-Setup.exe)** | Preporučeno — instalira se jednom |
| Windows 10/11 | [BlokBa-2.0.0-portable.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-2.0.0-portable.exe) | Bez instalacije, npr. sa USB-a |
| Linux (64-bit) | **[BlokBa-2.0.0.AppImage](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-2.0.0.AppImage)** | Jedan fajl, bez instalacije |
| Linux (Debian/Ubuntu) | [BlokBa_2.0.0_amd64.deb](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa_2.0.0_amd64.deb) | Standardni .deb paket |

Upute za prvo pokretanje su [niže](#prvo-pokretanje).

---

## Od bloka do koda

U većini blokovskih alata blok je metafora: naredba tipa `reci [Zdravo]`
nema veze sa tim kako se to piše u pravom jeziku. U BlokBa blok pokazuje
**stvarnu Python sintaksu**:

    ⌨ UNOS CIJELOG BROJA  [x]  = int( input( "unesi broj: " ))

```python
x = int(input("unesi broj: "))
```

Zagrade, navodnici i `int()` nisu ukras — to je kod koji se izvršava. Zato
put do tekstualnog programiranja ide u tri koraka, bez promjene alata:

| Korak | Šta đak radi |
|---|---|
| 🧩 **Slaganje** | Prevlači blokove i gleda kako uz njih nastaje Python kod, red po red. |
| ✏️ **Upisivanje** | U polje bloka kuca izraz tastaturom (`x + a`, `broj % 2 == 0`) umjesto da ga slaže iz manjih blokova. |
| 🐍 **Pisanje koda** | U Python editoru piše cijeli program sam. Program napravljen od blokova otvara se u editoru kao kod, a kod se može vratiti u blokove. |

---

## Šta BlokBa nudi

### 🧩 Blokovi koji su Python
- 11 kategorija: varijable, ulaz i izlaz, matematika, provjera, petlje,
  tekst, liste, crtanje, zvuk, funkcije i start
- Python kod se gradi uživo pored blokova
- Ime varijable se upiše olovkom direktno u blok — varijabla se napravi sama
- Uslov u bloku AKO i DOK je pravi blok: izvuče se, zamijeni ili upiše

### 🤖 Vodič kroz aplikaciju
**10 lekcija** korak po korak — od prvog ispisa na ekran do petlji i
uslova. Robotić BoT pokazuje gdje se klikne i provjerava svaki korak. Na kraju
lekcije đak dobija **samostalni zadatak**.

### 🐍 Python editor
- Programi se čuvaju kao obični `.py` fajlovi u đakovoj fascikli
- **Red se provjerava dok se kuca** — greška se označi odmah, ne tek pri
  pokretanju
- Editor sam drži uvlaku poslije `if`, `for`, `while` i `def`
- Sve se sprema samo, uz ranije verzije za povratak

### ✅ Vježbe sa provjerom
**53 vježbe** u pet oblasti: ispis, varijable, unos, uslovi i petlje.
Vrste zadataka:
- **dopuni praznine** u gotovom programu
- **ispravi grešku** u programu koji ne radi
- **napiši program** prema opisu
- **složi redove** pomiješanog programa u ispravan redoslijed i uvlaku

Dugme **✔ Provjeri** pokreće đakov program sa zadanim ulazima i poredi ispis
sa rješenjem. Kad nešto ne valja, savjet zavisi od vrste greške. Urađene
vježbe se pamte u đakovoj fascikli.

### 👀 Vidi se šta program radi
- **Tabela varijabli** se mijenja uživo dok program radi, sa tipom podatka
- **Korak po korak:** program se izvršava red po red, a trenutni red je
  osvijetljen
- **Kornjača** crta na mreži sa koordinatama; **zvuk** svira note
- Ulaz i izlaz idu kroz terminal, kao u pravom Pythonu

### 💬 Pomoć kad program pukne
Robot-asistent prevodi Python grešku na jednostavan jezik: šta se desilo, u
kojem redu i kako se popravlja. Prepoznaje i beskonačnu petlju. Radi **bez
interneta** i bez ikakvog podešavanja. Po želji se može uključiti i pravi AI
pomoćnik — vidi [BoT sa AI modelom](#bot-sa-ai-modelom).

### 🌍 Jezici
Sučelje na **bosanskom** (latinica i ćirilica), **hrvatskom**, **engleskom** i
**njemačkom**. Vodič i vježbe su prevedeni.

---

## Primjena u nastavi

**Učionica bez interneta i stari računari.** BlokBa ništa ne traži sa mreže.
Windows verzija nosi svoj Python, pa na školskim računarima ne treba ništa
instalirati osim same aplikacije.

**Jedan alat od VI do IX razreda.** Đaci počinju blokovima, prelaze na
upisivanje izraza u polje bloka, pa na Python editor. Okruženje se ne mijenja,
pa se vrijeme ne troši na upoznavanje novog programa.

**Prikaz na projektoru.** Kod pored blokova, korak po korak i tabela
varijabli pokazuju šta se dešava unutar programa dok se izvršava — šta
računar radi u svakom redu i kako se mijenjaju vrijednosti.

**Samostalan rad.** Vodič uvodi u aplikaciju bez nastavnikovog objašnjavanja
svakog klika. Vježbe se same provjeravaju, a robot objašnjava grešku, pa
nastavnik ostaje slobodan za đake kojima zaista treba pomoć.

**Svaki đak u svojoj fascikli.** Dijalozi za otvaranje i spremanje polaze od
`Documents`, gdje đaci imaju svoje fascikle (npr. `6aG1`, `6aG2`). Programi i
urađene vježbe ostaju tamo.

**Rad kod kuće.** Aplikacija je besplatna i radi isto kod kuće kao u školi.
Program se izvozi kao `.py` fajl i otvara u svakom Python okruženju.

---

## Prvo pokretanje

### Windows

Pri prvom pokretanju Windows može prikazati plavi prozor **„Windows je
zaštitio vaš računar"**. To nije virus — poruka se javlja kod svakog programa
koji nije digitalno potpisan. Klikni **More info** (Više informacija), pa
**Run anyway** (Pokreni svejedno).

Python **nije potreban** — zapakovan je u program. Ako je na računaru već
instaliran Python, BlokBa koristi njega.

### Linux

AppImage treba dozvolu za izvršavanje: desni klik → *Properties* →
*Permissions* → *Is executable*, ili u terminalu:

```bash
chmod +x BlokBa-2.0.0.AppImage
./BlokBa-2.0.0.AppImage
```

Na Debianu i Ubuntuu može se instalirati i `.deb` paket:

```bash
sudo dpkg -i BlokBa_2.0.0_amd64.deb
```

Potreban je **Python 3.10 ili noviji**. Većina distribucija ga već ima; ako
ga nema, BlokBa javi i ispiše komandu za instalaciju.

---

## BoT sa AI modelom

Pored pomoći koja uvijek radi bez interneta, BoT se može povezati sa pravim
jezičkim modelom, pa đak može pitati vlastitim riječima — i u blokovima i u
Python editoru. BoT vidi đakov program i zna koji blokovi postoje, ali **ne
rješava zadatak umjesto đaka**: vodi ga pitanjima, korak po korak.

| Servis | Potrebno |
|---|---|
| Anthropic (Claude) | API ključ, internet |
| OpenAI (GPT) | API ključ, internet |
| Google (Gemini) | API ključ, internet |
| **Ollama** | lokalno instaliran model, **bez interneta** |

Podešava se u meniju **AI Asistent → Postavi API ključ**. Ključ ostaje samo na
tom računaru. AI pomoćnik je **isključen dok ga sam ne uključiš.**

**Prije uključivanja treba znati:**
- **Cijena.** Anthropic, OpenAI i Google naplaćuju korištenje na tvoj račun;
  Google ima besplatan nivo za probu.
- **Privatnost.** Kod mrežnih servisa pitanja i đakov kod odlaze tom servisu.
  To je odluka koju treba donijeti svjesno, uz školsku politiku. **Ollama sve
  drži na računaru.**
- **Ollama traži jači računar** — nekoliko gigabajta memorije, najbolje na
  grafičkoj kartici. Na starim učioničkim mašinama ostaje pomoć bez interneta.

---

## Prijava grešaka i prijedlozi

<!-- LINK: ovdje ubaci link na Discord kanal -->

Uz prijavu **obavezno navedi broj verzije** (*Pomoć → O programu BlokBa*) i operativni
sistem. Bez toga se ne može utvrditi da li je greška već ispravljena.

Screenshot pomaže više od opisa.

---

## Podrška projektu

BlokBa je i ostaje besplatna. Ako želiš podržati dalji rad:

Paypal: nodi_bih@yahoo.de

---

## Uslovi korištenja

BlokBa se smije **besplatno koristiti i dijeliti u neizmijenjenom obliku**, u
školama i kod kuće.

Izmjena, prepakivanje i distribucija izmijenjenih verzija nisu dozvoljeni.

---

## Autori

Dino Isanović · Jasmin Suljkanović · Elvir Čajić
