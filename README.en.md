# BlokBa

**Hybrid block-based programming for the classroom.**

Students snap blocks together and see them **translated live into real Python**
that runs immediately. The code sits next to the blocks, line by line. Works
fully offline.

## What "hybrid" means

In most block-based tools the block is a metaphor. A command like
`say [Hello]` has nothing to do with how that is written in a real
programming language — the child learns to snap blocks, then starts over.

In BlokBa the block shows the **actual syntax**:

    ⌨ WHOLE NUMBER INPUT  [x]  = int( input( "enter a number: " ))

which produces:

```python
x = int(input("enter a number: "))
```

The brackets, quotes and `int()` aren't decoration — that is the Python
that runs.

Three steps, inside one application:

1. **Snapping** — younger students drag blocks and watch the code beside them
2. **Typing** — expressions are typed straight into a block field, e.g. `x + a`
   instead of assembling separate blocks for addition
3. **Exporting** — `File → Export as .py` produces a file that opens in
   PyCharm and behaves identically

So moving to text-based programming isn't a leap but a step: the student has
been reading that code all year, line by line.
> [Bosanski](README.md) · **English** · [Deutsch](README.de.md)

<!-- IMAGE: main screen screenshot goes here -->

---

## Download

Latest version: **[Releases](../../releases/latest)**

| System | Download | Note |
|---|---|---|
| Windows 10/11 | **[BlokBa-1.1.0-Setup.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-1.1.0-Setup.exe)** | Recommended — install once, starts instantly |
| Windows 10/11 | [BlokBa-1.1.0-portable.exe](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-1.1.0-portable.exe) | No installation — for a quick try, slower to start |
| Linux (64-bit) | **[BlokBa-1.1.0.AppImage](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa-1.1.0.AppImage)** | Single file, no installation for Linux |
| Linux (Debian/Ubuntu) | [BlokBa_1.1.0_amd64.deb](https://github.com/DinoIsanovic/BlokBa-app/releases/latest/download/BlokBa_1.1.0_amd64.deb) | Standard .deb package |

---

## First run

### Windows

On first launch Windows shows a blue dialog:

> **Windows protected your PC**

**This is not a virus.** The message appears for any program that isn't
digitally signed, and signing costs several hundred euros a year — hard to
justify for a free school application.

Click **More info**, then **Run anyway**.

Python is **not required** — it ships inside the program.

### Linux

The downloaded AppImage file has no execute permission. In a terminal:

```bash
chmod +x BlokBa-1.1.0.AppImage
./BlokBa-1.1.0.AppImage
```

Or right-click → *Properties* → *Permissions* → *Is executable*.

For Debian/Ubuntu and related distributions, you can install the `.deb`
package instead of the AppImage:

```bash
sudo dpkg -i BlokBa_1.1.0_amd64.deb
```

**Python 3.10 or newer must be installed.** Most distributions already have it.
If not, BlokBa will tell you and print the exact install command for your
system.

---
<img width="1421" height="890" alt="image" src="https://github.com/user-attachments/assets/2e25d786-4a20-4316-a548-12685bf52036" />





## What BlokBa does

- **In-app guide (BoT)** — 10 step-by-step lessons, from the first "print
  to screen" through more advanced statements, with a friendly robot
  tracking progress
- **11 block categories** — start, variables, input/output, maths, conditions,
  loops, text, lists, drawing, sound, functions
- **Live Python code** beside the blocks, so students see what each block means
- **Variable table** that updates while the program runs, showing data types
- **Robot assistant** that explains errors in plain language, no internet needed
- **Turtle graphics** on a coordinate grid
- **Export to `.py`** — the program opens in PyCharm and behaves the same
- **Five interface languages:** Bosnian, Croatian, English, German, Cyrillic

---

## BoT — the learning assistant

BlokBa ships with an assistant that works on **two levels**.

### Offline — always available

When a program crashes, BoT translates the Python error into plain language:
what happened, on which line, and how to fix it. It also detects runaway loops
and explains why they occur.

This needs **nothing at all** — no internet, no key, no setup. It's how BlokBa
works in a classroom with no network.

### With a real AI model — optional

If you want students to ask questions in their own words, BoT can connect to a
real language model:

| Service | Requires |
|---|---|
| Anthropic (Claude) | API key, internet |
| OpenAI (GPT) | API key, internet |
| Google (Gemini) | API key, internet |
| **Ollama** | a locally installed model, **no internet** |

Set it up under **AI Asistent → Postavi API ključ**. The key is stored **on that
computer only** and is never sent anywhere except the service you chose.

BoT knows which blocks exist in BlokBa, so it advises using their real names
instead of inventing Python that can't be built from blocks. It won't solve the
task for the student — it walks them through it.

### Before you turn it on

**Cost.** Anthropic, OpenAI and Google bill per use, on your own account. Google
offers a free tier that is usually enough to try it out.

**Privacy.** With an online service enabled, the questions and code a student
writes are sent to that provider. When working with children this deserves a
deliberate decision, and a look at your school's policy. **Ollama keeps
everything on the machine** — nothing leaves it.

**Ollama needs a capable computer.** A decent model takes several gigabytes of
memory, ideally on a graphics card. On older classroom machines this isn't
realistic — there, the offline assistant is the one that works.

The online assistant stays **off until you switch it on.**

---

## Bugs and suggestions

<!-- LINK: Discord channel link goes here -->

Please **always include the version number** (*Help → About*) and your operating
system. Without it there's no way to tell whether the bug is already fixed.

A screenshot helps more than a description.

---

## Supporting the project

BlokBa is free and will stay free. If you'd like to support further work:

Paypal: nodi_bih@yahoo.de
---

## Terms of use

BlokBa may be **used and shared free of charge in unmodified form**, in schools
and at home.

Modifying, repackaging, or distributing modified versions is not permitted.

---

## Authors

Dino Isanović · Jasmin Suljkanović · Elvir Čajić
