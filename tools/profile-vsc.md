# VSC profiles

Det är egentligen två separata saker i VS Code: **GitHub-inloggningen** och **VS Code Profiles**. 
Profilerna kan sedan synkroniseras via ditt GitHub/Microsoft-konto.

### 1. Logga in i VS Code med ditt GitHub-konto

På den stationära datorn:

1. Öppna VS Code.
2. Klicka på **Accounts**-ikonen nere till vänster.
3. Välj **Sign in to Sync Settings**.
4. Välj **GitHub**.
5. Webbläsaren öppnas → logga in med ditt skol-GitHub-konto.
6. Godkänn anslutningen till VS Code.
7. Gå tillbaka till VS Code.

När du är inloggad kan VS Code synkronisera bland annat:

- Settings
- Keyboard shortcuts
- Extensions
- User snippets
- UI state
- **Profiles**

Kontrollera gärna efteråt via:

**Accounts → Settings Sync is On**

---

### 2. Skapa eller byta VS Code Profile

Klicka på **Manage**-kugghjulet nere till vänster och välj:

**Profiles**

Där kan du se dina profiler och skapa nya.

Ett exempel:

```
DefaultHTML-CSSJavaScriptPython
```

Varje profil kan ha egna:

- extensions
- settings
- keyboard shortcuts
- UI-inställningar
- tema
- färger
- snippets

Det passar ganska bra för dina olika kursprojekt.

---

### 3. Snabbt byta profil

Det enklaste är:

**Ctrl + Shift + P**

skriv:

```
Profiles
```

och välj:

**Profiles: Switch Profile**

Sedan väljer du exempelvis:

```
HTML-CSSJavaScriptPython
```

Du kan också klicka på **Profile-ikonen** nere till vänster och välja profilen direkt.

---

### 4. Viktigt: Profile ≠ GitHub repository

Det här är lätt att blanda ihop.

Din profil:

```
VS Code Profile       ↓Settings / Extensions / Theme / Shortcuts
```

är inte samma sak som:

```
Git repository       ↓GitHub repository
```

GitHub används här bland annat för att **synkronisera din VS Code-konfiguration mellan datorer**.

Så på din laptop kan du ha:

```
VS Code   ↓GitHub school account   ↓Settings Sync   ↓HTML-CSS Profile
```

Och på den stationära datorn gör du samma inloggning. Då kan VS Code hämta din synkroniserade konfiguration.

### 5. En sak att kontrollera på den stationära

Eftersom du verkar ha flera GitHub-konton är det särskilt viktigt att kontrollera 
**vilket konto VS Code faktiskt är inloggat med**.

Klicka på: **Accounts → GitHub** och kontrollera användarnamnet.

Det behöver vara samma konto som du använde på laptopen om du vill få exakt samma synkroniserade profiler och inställningar.
