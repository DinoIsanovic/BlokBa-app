# BlokBa

**Hibridno blokovsko programiranje za nastavu informatike.**

Đaci slažu blokove, a oni se **uživo prevode u pravi Python kod** koji se odmah
izvršava. Kod se vidi pored blokova, red po red. Radi potpuno offline.

## Šta znači „hibridno"

U većini blokovskih alata blok je metafora. Naredba tipa `reci [Zdravo]`
nema nikakve veze sa tim kako se to piše u pravom programskom jeziku —
dijete nauči slagati blokove, a poslije kreće ispočetka.

U BlokBa blok pokazuje **stvarnu sintaksu**:

    ⌨ UNOS CIJELOG BROJA  [x]  = int( input( "unesi broj: " ))

iz čega nastaje:

```python
x = int(input("unesi broj: "))
```

Zagrade, navodnici i `int()` nisu ukras — to je Python koji se izvršava.

Tri stepenika, unutar iste aplikacije:

1. **Slaganje** — mlađi đaci samo prevlače blokove i gledaju kod pored njih
2. **Upisivanje** — u polje bloka se kuca izraz preko tastature, npr. `x + a`
   umjesto slaganja posebnih blokova za sabiranje
3. **Izvoz** — `Datoteka → Izvezi kao .py` daje fajl koji se otvori u
   PyCharmu i radi identično

Zato prelazak na tekstualno programiranje u VII ili VIII razredu nije skok
nego korak: dijete je taj kod već čitalo cijelu godinu, red po red.

> **Bosanski** · [English](README.en.md) · [Deutsch](README.de.md)

<!-- SLIKA: ovdje ubaci screenshot glavnog ekrana -->

---

## Preuzimanje

Najnovija verzija: **[Izdanja](../../releases/latest)**

| Sistem | Preuzimanje | Napomena |
|---|---|---|
| Windows 10/11 | **[BlokBa-1.1.0-Setup.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-1.1.0-Setup.exe)** | Preporučeno — instalira se jednom, pokreće se odmah |
| Windows 10/11 | [BlokBa-1.1.0-portable.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-1.1.0-portable.exe) | Bez instalacije — za brzu probu, sporije se pokreće |
| Linux (64-bit) | **[BlokBa-1.1.0.AppImage](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-1.1.0.AppImage)** | Jedan fajl, bez instalacije za Linux |
| Linux (Debian/Ubuntu) | [BlokBa_1.1.0_amd64.deb](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa_1.1.0_amd64.deb) | Standardni .deb paket |

---

## Prvo pokretanje

### Windows

Pri prvom pokretanju Windows će prikazati plavi prozor:

> **Windows je zaštitio vaš računar**

**To nije virus.** Poruka se javlja kod svakog programa koji nije digitalno
potpisan, a potpisivanje košta nekoliko stotina eura godišnje — što za
besplatnu školsku aplikaciju nema smisla.

Klikni **More info** (Više informacija), pa **Run anyway** (Pokreni svejedno).

Python **nije potreban** — zapakovan je u sam program.

### Linux

Preuzeti AppImage fajl nema dozvolu za izvršavanje. U terminalu:

```bash
chmod +x BlokBa-1.1.0.AppImage
./BlokBa-1.1.0.AppImage
```

Ili desni klik → *Properties* → *Permissions* → *Is executable*.

Za Debian/Ubuntu i srodne distribucije, umjesto AppImage-a možeš instalirati
`.deb` paket:

```bash
sudo dpkg -i BlokBa_1.1.0_amd64.deb
```

**Potreban je Python 3.10 ili noviji** na sistemu. Većina distribucija ga već
ima. Ako ga nema, BlokBa će ti javiti i ispisati tačnu komandu za instalaciju.

---
<img width="1742" height="1034" alt="image" src="https://github.com/user-attachments/assets/fd814f62-a2a9-4c7e-b93d-f58e91acab59" />


## Šta BlokBa radi

- **Vodič kroz aplikaciju (BoT)** — 10 lekcija korak-po-korak, od prvog
  ispisa na ekran do naprednijih naredbi, sa robotićem koji prati napredak
- **11 kategorija blokova** — start, varijable, ulaz/izlaz, matematika,
  provjera, petlje, tekst, liste, crtanje, zvuk, funkcije
- **Živi Python kod** pored blokova — dijete vidi šta svaki blok znači
- **Tabela varijabli** koja se mijenja dok program radi, sa tipovima podataka
- **Robot-asistent** koji objašnjava greške dječijim jezikom, bez interneta
- **Kornjača** za crtanje, na mreži sa koordinatama
- **Izvoz u `.py`** — program se otvara u PyCharmu i radi isto
- **Pet jezika sučelja:** bosanski, hrvatski, engleski, njemački, ćirilica

---

## BoT — pomoćnik u učenju

BlokBa ima ugrađenog pomoćnika koji radi na **dva nivoa**.

### Bez interneta — uvijek radi

Kad program pukne, BoT prevede Python grešku na dječiji jezik: šta se desilo, u
kojem redu, i kako se popravlja. Prepoznaje i beskonačnu petlju i objasni zašto
se javila.

Za ovo **nije potrebno ništa** — ni internet, ni ključ, ni podešavanje. Tako
BlokBa radi u učionici bez mreže.

### Sa pravim AI modelom — po želji

Ako želiš da đak može pitati vlastitim riječima, BoT se može povezati sa pravim
jezičkim modelom. Podržani su:

| Servis | Potrebno |
|---|---|
| Anthropic (Claude) | API ključ, internet |
| OpenAI (GPT) | API ključ, internet |
| Google (Gemini) | API ključ, internet |
| **Ollama** | lokalno instaliran model, **bez interneta** |

Podešava se u meniju **AI Asistent → Postavi API ključ**. Ključ se čuva **samo
na tom računaru** i ne šalje se nigdje osim izabranom servisu.

BoT zna koji blokovi postoje u BlokBa, pa savjetuje njihovim imenima umjesto da
izmišlja Python koji se blokovima ne može složiti. Ne rješava zadatak umjesto
đaka — vodi ga korak po korak.

### Šta treba znati prije uključivanja

**Cijena.** Anthropic, OpenAI i Google naplaćuju po korištenju, na tvoj račun.
Google nudi besplatan nivo koji je za probu obično dovoljan.

**Privatnost.** Ako uključiš mrežni servis, pitanja i kod koje đak napiše odlaze
tom servisu. Za rad sa djecom to je odluka koju treba donijeti svjesno — i
provjeriti šta o tome kaže školska politika. **Ollama sve drži na računaru** i
ništa ne izlazi napolje.

**Ollama traži jači računar.** Model pristojnog kvaliteta zauzima nekoliko
gigabajta memorije, najbolje na grafičkoj kartici. Na starim učioničkim
mašinama to nije izvodljivo — tamo ostaje pomoć koja radi bez interneta.

Mrežni pomoćnik je **isključen dok ga sam ne uključiš.**

---

## Prijava grešaka i prijedlozi

<!-- LINK: ovdje ubaci link na Discord kanal -->

Uz prijavu **obavezno navedi broj verzije** (*Pomoć → O programu*) i operativni
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
