# Kort info om Git/GitHub

<img src="bilder/git-basics.jpg" width="768">

---

# Git & GitHub – snabbguide

## Grundmodell

```text
LOCAL:  Working directory → Stage (git add) → Commit → Local repository → Push → GitHub

REMOTE: GitHub → Fetch → origin/main → Pull/Merge → Local repository → Working directory
```

## Terminal

Kommandona i den här guiden körs i en terminal. Du kan använda:

- VS Codes inbyggda terminal
- en separat terminal, till exempel PowerShell, Command Prompt eller Git Bash

VS Code har dessutom ett grafiskt gränssnitt för många Git-kommandon, till exempel Stage, Commit, Pull och Push. Motsvarande terminalkommandon visas i exemplen nedan.

---

## Scenario 1 – Repository finns redan på GitHub

**Utgångsläge:**  
Repositoryt skapas först på GitHub. Du vill klona det till din dator och börja arbeta lokalt.

Öppna terminalen i den mapp där du vill spara projektet, eller navigera dit med `cd`:

```bash
cd sökväg/till/mappen
```

Därefter klonar du repositoryt:

```bash
git clone https://github.com/WEBD26JON/golfklubb-centar.git
cd golfklubb-centar
```

`git clone` skapar den lokala arbetsmappen, ett lokalt Git-repository och kopplingen till remote `origin`.

Kontrollera kopplingen:

```bash
git remote -v

Svar:

origin  https://github.com/WEBD26JON/golfklubb-centar.git (fetch)
origin  https://github.com/WEBD26JON/golfklubb-centar.git (push)
```

`origin` är namnet på remote-repositoryt. `fetch` visar adressen som används för att hämta ändringar och `push` adressen som används för att skicka ändringar.

### När andra har gjort ändringar

```bash
git pull
```

### När du har gjort egna ändringar

```bash
git add index.html       # en fil
git add css/             # en mapp
git add .                # alla ändringar

git commit -m "Beskriv ändringen"
git push
```

**VS Code:**

```text
Changes → Stage Changes → Commit → Sync / Push
```

---

## Scenario 2 – Repository börjar lokalt

**Utgångsläge:**  
Projektet finns först bara på din dator.

Skapa projektmappen och initiera Git:

```bash
mkdir golfklubb-centar
cd golfklubb-centar

git init
```

Lägg till filer och skapa den första commiten:

```bash
git add .
git commit -m "Initial commit"
```

Skapa sedan ett repository på GitHub och koppla det till det lokala repositoryt:

```bash
git remote add origin https://github.com/WEBD26JON/golfklubb-centar.git
```

Kontrollera:

```bash
git remote -v
```

`git remote add origin` skapar själva kopplingen. Det skickar eller hämtar inga filer.

Skicka sedan den lokala branchen till GitHub:

```bash
git branch -M main
git push -u origin main
```

Efter detta är det ett normalt Git/GitHub-arbetsflöde:

```text
ändra → Stage → Commit → Push
```

---

## Scenario 3 – Hämta ändringar från GitHub

**Utgångsläge:**  
Någon annan har gjort `push` till GitHub.

### Bara kontrollera vad som finns på remote

```bash
git fetch
```

`fetch` hämtar information om nya commits från remote utan att ändra dina lokala arbetsfiler.

### Hämta och integrera ändringar

```bash
git pull
```

`git pull` hämtar nya commits från remote och integrerar dem i din aktuella branch.

Det motsvarar normalt:

```bash
git fetch
git merge
```

---

## Scenario 4 – Skicka lokala ändringar till GitHub

**Utgångsläge:**  
Du har ändrat filer lokalt.

```bash
git status
git add .
git commit -m "Beskriv ändringen"
git push
```

Eller staga bara det du vill committa:

```bash
git add index.html
git add css/
```

I VS Code:

```text
Changes
 ├── index.html
 ├── css/
 └── images/

        ↓ Stage Changes

Staged Changes
 └── index.html
```

Endast staged ändringar kommer med i nästa commit.

---

## Scenario 5 – Push avvisas

**Utgångsläge:**  
Någon annan har hunnit göra `push` före dig.

```text
git push → REJECTED
```

Hämta först ändringarna:

```bash
git pull
```

Lös eventuella konflikter och gör sedan:

```bash
git push
```

**Använd inte `git push --force` som standardlösning.**

---

## Git och VS Code – terminologi

| Git CLI | VS Code / Source Control | Svenska |
|---|---|---|
| `git status` | Source Control → Changes | Ändringar |
| `git add fil.html` | Stage Changes | Staga filen |
| `git add css/` | Stage Changes | Staga mappen |
| `git add .` | Stage All Changes | Staga alla ändringar |
| `git restore fil.html` | Discard Changes | Kasta ändringar |
| `git commit` | Commit | Skapa commit |
| `git push` | Push / Sync | Skicka till remote |
| `git pull` | Pull / Sync | Hämta och integrera |

---

## Snabbval

| Situation | Kommando |
|---|---|
| Hämta ett nytt GitHub-repository | `git clone` |
| Skapa Git lokalt | `git init` |
| Koppla till GitHub | `git remote add origin ...` |
| Se ändringar | `git status` |
| Staga en fil | `git add fil` |
| Staga en mapp | `git add mapp/` |
| Staga allt | `git add .` |
| Skapa commit | `git commit -m "..."` |
| Hämta utan att integrera | `git fetch` |
| Hämta + integrera | `git pull` |
| Skicka commits till GitHub | `git push` |
| Visa remote | `git remote -v` |
