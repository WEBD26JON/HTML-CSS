## ❓ #1 QSTNS i Kursmoment01.md

---

### 🤖 #1A gemma4:31b-cloud

Här är svaren på dina frågor, Alexander.

**Vad är HTML?**
HTML står för HyperText Markup Language. Det är ett märkspråk som används för att strukturera innehållet på en webbsida genom att definiera element som rubriker, stycken, länkar och bilder.

**Grundstruktur i HTML?**
En grundläggande HTML-fil ser ut så här:
```html
<!DOCTYPE html>
<html lang="sv">
<head>
    <meta charset="UTF-8">
    <title>Sidans titel</title>
</head>
<body>
    <!-- Innehållet här -->
</body>
</html>
```

**Förklara skillnaden mellan taggar och attribut i HTML?**
*   **Taggar:** Används för att markera början och slutet av ett element (t.ex. `<p>` och `</p>`).
*   **Attribut:** Ger extra information om ett element och placeras alltid i starttaggen (t.ex. `href` i en länk eller `src` i en bild).

**Vad är skillnaden mellan fysiska och semantiska element?**
*   **Fysiska element:** Beskriver hur något ska *se ut* rent visuellt (t.ex. `<b>` för fetstil).
*   **Semantiska element:** Beskriver innehållets *betydelse* eller syfte (t.ex. `<article>`, `<nav>` eller `<strong>`). Detta är viktigt för tillgänglighet och sökmotorer.

**Vad är skillnaden mellan `<b>` och `<strong>`?**
*   `<b>` gör texten fet utan att tillskriva den någon extra vikt (visuellt).
*   `<strong>` gör texten fet men signalerar också att innehållet är viktigt eller brådskande (semantiskt).

**Vad är skillnaden mellan `<i>` och `<em>`?**
*   `<i>` gör texten kursiv (visuellt).
*   `<em>` (emphasis) gör texten kursiv men signalerar att orden ska betonas (semantiskt).

**Vad är skillnaden mellan `<blockquote>` och `<cite>`?**
*   `<blockquote>` används för längre citat som tas från en annan källa och visas ofta indraget.
*   `<cite>` används för att referera till titeln på ett verk (t.ex. en bok eller en artikel) som citeras.

**Vad är skillnaden mellan UL och OL?**
*   `<ul>` (Unordered List): En punktlista (oftast med bullets).
*   `<ol>` (Ordered List): En numrerad lista.

**Hur används DL-taggen i HTML?**
`<dl>` (Description List) används för listor med termer och beskrivningar. Den innehåller `<dt>` (term) och `<dd>` (beskrivning).

**Vad är URL? Vad är skillnaden mellan en absolut URL och en relativ/lokal URL?**
URL står för Uniform Resource Locator (en webbadress).
*   **Absolut URL:** Hela adressen inklusive protokoll (t.ex. `https://www.google.com`).
*   **Relativ/Lokal URL:** En adress i förhållande till den nuvarande filens plats (t.ex. `/bilder/logo.png` eller `index.html`).

**Hur skapar du länkar som öppnas i nya flikar?**
Genom att lägga till attributet `target="_blank"` i `<a>`-taggen.
Exempel: `<a href="https://google.com" target="_blank">Google</a>`

**Externa länkar måste innehålla ett protokoll. Vad innebär det?**
Ett protokoll definierar hur data ska överföras. För webbsidor är de vanligaste `http://` eller `https://` (S står för secure). Utan protokoll tror webbläsaren att länken är en lokal fil.

**Vilka bildformat används på webben?**
De vanligaste är JPEG, PNG, GIF, SVG och WebP.

**Vilka attribut är obligatoriska i en img-tagg?**
`src` (källan till bilden) och `alt` (alternativ text för tillgänglighet och om bilden inte kan laddas).

**I vilket syfte används en GIF-bild på webben?**
GIF används främst för enkla animationer eller bilder med få färger och transparent bakgrund.

**Vilka element bildar upp en tabell i HTML?**
*   `<table>`: Själva tabellen.
*   `<tr>`: Tabellrad (Table Row).
*   `<th>`: Tabellrubrik (Table Header).
*   `<td>`: Tabellcell (Table Data).

**Hur sammanfogar man tre celler i en rad? Skriv ett exempel.**
Man använder attributet `colspan="3"`.
```html
<tr>
    <td colspan="3">Denna cell sträcker sig över tre kolumner</td>
</tr>
```

**Vilka element behövs för att skapa ett inloggningsformulär i HTML?**
*   `<form>`: Inramningen av formuläret.
*   `<label>`: Textetiketter för fälten.
*   `<input type="text">` eller `<input type="email">`: För användarnamn/mejl.
*   `<input type="password">`: För lösenordet.
*   `<button type="submit">` eller `<input type="submit">`: För att skicka formuläret.

**Vad innebär formulärvalidering? Skriv några exempel!**
Det innebär att kontrollera att användaren har fyllt i informationen korrekt innan den skickas.
Exempel:
*   `required`: Fältet får inte vara tomt.
*   `type="email"`: Kontrollerar att innehållet följer formatet för en e-postadress.
*   `minlength="8"`: Kräver att texten är minst 8 tecken lång.

**Hur fungerar iframe-taggen?**
`<iframe>` (Inline Frame) används för att bädda in en annan HTML-sida inuti den nuvarande sidan (t.ex. en Google Maps-karta eller en YouTube-video).

**Vilka taggar och attribut är viktiga för att spela upp ljud i HTML?**
Tagg: `<audio>`.
Viktiga attribut: `src` (filvägen), `controls` (visar play/pause-knappar), `autoplay` och `loop`.

**Vilka taggar och attribut är viktiga för att spela upp video i HTML?**
Tagg: `<video>`.
Viktiga attribut: `src`, `controls`, `width`, `height`, `autoplay` och `muted` (nödvändigt för att autoplay ska fungera i många webbläsare).

*(⏱ 4.85s)*
