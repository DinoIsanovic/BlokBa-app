# BlokBa

**Od prvog bloka do pravog Python programa — u jednoj aplikaciji.**

BlokBa je besplatna aplikacija za nastavu programiranja u osnovnoj školi.
Učenici slažu blokove, a blokovi se **uživo prevode u pravi Python kod** koji
se odmah izvršava. Kad dođe vrijeme za tekstualno programiranje, učenici
ostaju u istoj aplikaciji: isti prozor, isti terminal, isti pomoćnik — samo
što sada kod pišu sami.

Radi **potpuno bez interneta**, na Windowsu i Linuxu, i na starijim
računalima.

> [Bosanski](README.md) · **Hrvatski** · [English](README.en.md) · [Deutsch](README.de.md)

<img width="1423" height="892" alt="BlokBa — blokovi i Python kod jedan pored drugoga" src="https://github.com/user-attachments/assets/18916c19-89f8-4980-aeb8-12acf0f05402" />

---

## Preuzimanje

Najnovija verzija: **[BlokBa 2.0.0](../../releases/latest)**

| Sustav | Preuzimanje | Napomena |
|---|---|---|
| Windows 10/11 | **[BlokBa-2.0.0-Setup.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-2.0.0-Setup.exe)** | Preporučeno — instalira se jednom |
| Windows 10/11 | [BlokBa-2.0.0-portable.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-2.0.0-portable.exe) | Bez instalacije, npr. s USB-a |
| Linux (64-bit) | **[BlokBa-2.0.0.AppImage](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-2.0.0.AppImage)** | Jedna datoteka, bez instalacije |
| Linux (Debian/Ubuntu) | [BlokBa_2.0.0_amd64.deb](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa_2.0.0_amd64.deb) | Standardni .deb paket |

Upute za prvo pokretanje su [niže](#prvo-pokretanje).

---

## Od bloka do koda

U većini blokovskih alata blok je metafora: naredba tipa `reci [Bok]` nema
veze s time kako se to piše u pravom jeziku. U BlokBa blok pokazuje
**stvarnu Python sintaksu**:

    ⌨ UNOS CIJELOG BROJA  [x]  = int( input( "unesi broj: " ))

```python
x = int(input("unesi broj: "))
```

Zagrade, navodnici i `int()` nisu ukras — to je kod koji se izvršava. Zato
put do tekstualnog programiranja ide u tri koraka, bez promjene alata:

| Korak | Što učenik radi |
|---|---|
| 🧩 **Slaganje** | Povlači blokove i gleda kako uz njih nastaje Python kod, redak po redak. |
| ✏️ **Upisivanje** | U polje bloka tipkovnicom upisuje izraz (`x + a`, `broj % 2 == 0`) umjesto da ga slaže iz manjih blokova. |
| 🐍 **Pisanje koda** | U Python editoru sam piše cijeli program. Program napravljen od blokova otvara se u editoru kao kod, a kod se može vratiti u blokove. |

---

## Što BlokBa nudi

### 🧩 Blokovi koji su Python
- 11 kategorija: varijable, ulaz i izlaz, matematika, provjera, petlje,
  tekst, liste, crtanje, zvuk, funkcije i start
- Python kod nastaje uživo pored blokova
- Ime varijable upiše se olovkom izravno u blok — varijabla se napravi sama
- Uvjet u bloku AKO i DOK pravi je blok: izvuče se, zamijeni ili upiše

### 🤖 Vodič kroz aplikaciju
**10 lekcija** korak po korak — od prvog ispisa na zaslon do petlji i
uvjeta. Robotić BoT pokazuje gdje treba kliknuti i provjerava svaki korak. Na
kraju lekcije učenik dobiva **samostalni zadatak**.

### 🐍 Python editor
- Programi se spremaju kao obične `.py` datoteke u učenikovoj mapi
- **Redak se provjerava dok se tipka** — pogreška se označi odmah, ne tek pri
  pokretanju
- Editor sam drži uvlaku nakon `if`, `for`, `while` i `def`
- Sve se sprema samo, uz ranije verzije za povratak

### ✅ Vježbe s provjerom
**53 vježbe** u pet područja: ispis, varijable, unos, uvjeti i petlje.
Vrste zadataka:
- **dopuni praznine** u gotovom programu
- **ispravi pogrešku** u programu koji ne radi
- **napiši program** prema opisu
- **složi retke** izmiješanog programa u ispravan redoslijed i uvlaku

Gumb **✔ Provjeri** pokreće učenikov program sa zadanim ulazima i uspoređuje
ispis s rješenjem. Kad nešto ne valja, savjet ovisi o vrsti pogreške.
Riješene vježbe pamte se u učenikovoj mapi.

### 👀 Vidi se što program radi
- **Tablica varijabli** mijenja se uživo dok program radi, s tipom podatka
- **Korak po korak:** program se izvršava redak po redak, a trenutni redak je
  istaknut
- **Kornjača** crta na mreži s koordinatama; **zvuk** svira note
- Ulaz i izlaz idu kroz terminal, kao u pravom Pythonu

### 💬 Pomoć kad program pukne
Robot-asistent prevodi Python pogrešku na jednostavan jezik: što se dogodilo,
u kojem retku i kako se popravlja. Prepoznaje i beskonačnu petlju. Radi **bez
interneta** i bez ikakvog podešavanja. Po želji se može uključiti i pravi AI
pomoćnik — vidi [BoT s AI modelom](#bot-s-ai-modelom).

### 🌍 Jezici
Sučelje na **bosanskom** (latinica i ćirilica), **hrvatskom**, **engleskom** i
**njemačkom**. Vodič i vježbe su prevedeni.

---

## Primjena u nastavi

**Učionica bez interneta i stara računala.** BlokBa ništa ne traži s mreže.
Windows verzija nosi svoj Python, pa na školskim računalima ne treba ništa
instalirati osim same aplikacije.

**Jedan alat od prvog bloka do pisanja koda.** Učenici počinju blokovima,
prelaze na upisivanje izraza u polje bloka, pa na Python editor. Okruženje se
ne mijenja, pa se vrijeme ne troši na upoznavanje novog programa.

**Prikaz na projektoru.** Kod pored blokova, korak po korak i tablica
varijabli pokazuju što se događa unutar programa dok se izvršava — što
računalo radi u svakom retku i kako se mijenjaju vrijednosti.

**Samostalan rad.** Vodič uvodi u aplikaciju bez učiteljeva objašnjavanja
svakog klika. Vježbe se same provjeravaju, a robot objašnjava pogrešku, pa
učitelj ostaje slobodan za učenike kojima pomoć zaista treba.

**Svaki učenik u svojoj mapi.** Dijalozi za otvaranje i spremanje polaze od
`Documents`, gdje učenici imaju svoje mape (npr. `6aG1`, `6aG2`). Programi i
riješene vježbe ostaju ondje.

**Rad kod kuće.** Aplikacija je besplatna i radi isto kod kuće kao u školi.
Program se izvozi kao `.py` datoteka i otvara u svakom Python okruženju.

---

## Prvo pokretanje

### Windows

Pri prvom pokretanju Windows može prikazati plavi prozor **„Windows je
zaštitio vaše računalo"**. To nije virus — poruka se javlja kod svakog
programa koji nije digitalno potpisan. Klikni **More info** (Više
informacija), pa **Run anyway** (Ipak pokreni).

Python **nije potreban** — zapakiran je u program. Ako je na računalu već
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
ga nema, BlokBa to javi i ispiše naredbu za instalaciju.

---

## BoT s AI modelom

Osim pomoći koja uvijek radi bez interneta, BoT se može povezati s pravim
jezičnim modelom, pa učenik može pitati vlastitim riječima — i u blokovima i
u Python editoru. BoT vidi učenikov program i zna koji blokovi postoje, ali
**ne rješava zadatak umjesto učenika**: vodi ga pitanjima, korak po korak.

| Servis | Potrebno |
|---|---|
| Anthropic (Claude) | API ključ, internet |
| OpenAI (GPT) | API ključ, internet |
| Google (Gemini) | API ključ, internet |
| **Ollama** | lokalno instaliran model, **bez interneta** |

Podešava se u izborniku **AI Asistent → Postavi API ključ**. Ključ ostaje
samo na tom računalu. AI pomoćnik je **isključen dok ga sam ne uključiš.**

**Prije uključivanja treba znati:**
- **Cijena.** Anthropic, OpenAI i Google naplaćuju korištenje na tvoj račun;
  Google ima besplatnu razinu za probu.
- **Privatnost.** Kod mrežnih servisa pitanja i učenikov kod odlaze tom
  servisu. To je odluka koju treba donijeti svjesno, u skladu sa školskim
  pravilima. **Ollama sve drži na računalu.**
- **Ollama traži jače računalo** — nekoliko gigabajta memorije, najbolje na
  grafičkoj kartici. Na starim učioničkim računalima ostaje pomoć bez
  interneta.

---

## Prijava pogrešaka i prijedlozi

<!-- LINK: ovdje ubaci link na Discord kanal -->

Uz prijavu **obavezno navedi broj verzije** (*Pomoć → O programu BlokBa*) i
operacijski sustav. Bez toga se ne može utvrditi je li pogreška već
ispravljena.

Snimka zaslona pomaže više od opisa.

---

## Podrška projektu

BlokBa je i ostaje besplatna. Ako želiš podržati daljnji rad:

Paypal: nodi_bih@yahoo.de

---

## Uvjeti korištenja

BlokBa se smije **besplatno koristiti i dijeliti u neizmijenjenom obliku**, u
školama i kod kuće.

Izmjena, prepakiravanje i distribucija izmijenjenih verzija nisu dopušteni.

---

## Autori

Dino Isanović · Jasmin Suljkanović · Elvir Čajić
