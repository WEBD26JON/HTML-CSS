# CSS

[HTML Styles - CSS w3schools](https://www.w3schools.com/html/html_css.asp)

Saved: 2026-09-21T22:46:15.804604

## ❓ #1

Vad är CSS? Varför behövs CSS? Hur skrivs en CSS-Regel?  
Vad innebär begreppet Cascading i CSS?  
Vad är skillnaden mellan en ID-Selektor och en Klass-Selektor? Skapa två olika exempel.   
Hur används Google Fonts på en sida. Visa några exempel.   
Vad gör följande selektor a:hover?  
Vad innebär Boxmodellen i CSS?   
Vad är skillnaden mellan margin och padding?  
Vad är skillnaden mellan inline, block och inline-block?   
Vad är span och div? Hur fungerar dessa element med CSS?   
Varför ska vi använda automatiska marginaler i CSS?  
Hur lägger du till runda hörn på en bild i CSS?  
Hur formaterar du en enkel navigeringslista med CSS?

---

### 🤖 #1A gemma4:31b-cloud

Hej Alexander. Här är svaren på dina frågor om CSS.

### Vad är CSS? Varför behövs CSS?
CSS står för **Cascading Style Sheets**. Det är ett språk som används för att bestämma utseendet och layouten på ett dokument skrivet i HTML.
CSS behövs för att separera innehållet (HTML) från designen. Detta gör det enklare att underhålla webbplatsen, eftersom du kan ändra utseendet på hela sajten genom att bara redigera en enda CSS-fil istället för varje enskild HTML-sida.

### Hur skrivs en CSS-Regel?
En CSS-regel består av en **selektor** och ett **deklarationsblock**.
```css
selektor {
  egenskap: värde;
}
```
*Exempel:*
```css
p {
  color: blue;
  font-size: 16px;
}
```

### Vad innebär begreppet Cascading i CSS?
"Cascading" (kaskad) innebär att CSS följer en viss hierarki för att bestämma vilken stil som ska gälla om det finns motstridiga regler. Prioriteringen styrs av:
1. **Viktighet** (`!important`).
2. **Specificitet** (en ID-selektor väger tyngre än en klass-selektor).
3. **Källordning** (regler som skrivs längre ner i filen skriver över tidigare regler).

### Skillnad mellan ID-Selektor och Klass-Selektor
*   **ID-selektor (`#`):** Används för ett unikt element på sidan. Varje ID får bara användas en gång.
*   **Klass-selektor (`.`):** Används för grupper av element. Samma klass kan användas på flera olika element.

**Exempel:**
```css
/* ID-selektor för en unik header */
#main-header {
  background-color: grey;
}

/* Klass-selektor för alla knappar */
.button-style {
  border-radius: 5px;
  padding: 10px;
}
```

### Hur används Google Fonts på en sida?
Du använder Google Fonts genom att hämta en länk från Google Fonts och lägga in den i HTML-dokumentets `<head>`, eller genom att använda `@import` i CSS. Sedan anropar du typsnittet via `font-family`.

**Exempel:**
1. I HTML: `<link href="https://fonts.googleapis.com/css2?family=Roboto&display=swap" rel="stylesheet">`
2. I CSS:
```css
body {
  font-family: 'Roboto', sans-serif;
}
```

### Vad gör selektorn `a:hover`?
`a:hover` är en **pseudoklass**. Den används för att definiera hur en länk (`<a>`) ska se ut när användaren håller muspekaren över den.

### Vad innebär Boxmodellen i CSS?
Boxmodellen innebär att alla HTML-element betraktas som rektangulära boxar. Boxmodellen består av fyra lager (inifrån och ut):
1. **Content:** Själva innehållet (text, bild).
2. **Padding:** Utrymmet mellan innehållet och ramen.
3. **Border:** Ramen runt padding och innehåll.
4. **Margin:** Utrymmet utanför ramen som skapar avstånd till andra element.

### Vad är skillnaden mellan margin och padding?
*   **Padding** skapar utrymme *inuti* elementet (mellan innehållet och kanten).
*   **Margin** skapar utrymme *utanför* elementet (avstånd till grann-element).

### Skillnad mellan inline, block och inline-block
*   **Block:** Tar upp hela bredden på sidan och startar alltid på en ny rad (t.ex. `<div>`, `<h1>`, `<p>`).
*   **Inline:** Tar bara upp så mycket plats som innehållet kräver och startar inte på ny rad. Man kan inte sätta bredd eller höjd på dessa (t.ex. `<span>`, `<a>`).
*   **Inline-block:** Fungerar som inline (ligger på samma rad), men man kan sätta bredd, höjd, margin och padding.

### Vad är span och div?
*   **`<div>`** är ett block-element. Det används som en container för att gruppera större delar av innehållet.
*   **`<span>`** är ett inline-element. Det används för att styla små delar av text inuti ett annat element.
*   **Med CSS:** Båda elementen har ingen egen inbyggd design, vilket gör dem perfekta för att stylas helt fritt med CSS via klasser eller ID:n.

### Varför ska vi använda automatiska marginaler i CSS?
Automatiska marginaler (`margin: auto;`) används främst för att centrera ett block-element horisontellt i dess förälderelement. För att det ska fungera måste elementet ha en definierad bredd (`width`).

### Hur lägger du till runda hörn på en bild i CSS?
Det görs med egenskapen `border-radius`.
```css
img {
  border-radius: 15px; /* För mjuka hörn */
  /* border-radius: 50%; för en helt rund bild */
}
```

### Hur formaterar du en enkel navigeringslista med CSS?
För att göra en horisontell meny tar man bort punktlistans markörer och ändrar listelementen till `inline` eller `inline-block`.

```css
nav ul {
  list-style-type: none; /* Tar bort punkterna */
  margin: 0;
  padding: 0;
  overflow: hidden;
  background-color: #333;
}

nav li {
  float: left; /* Eller display: inline-block; */
}

nav li a {
  display: block;
  color: white;
  text-align: center;
  padding: 14px 16px;
  text-decoration: none;
}

nav li a:hover {
  background-color: #111;
}
```

*(⏱ 5.87s)*

## ❓ #2

Vilken skillnad är mellan em och rem i CSS?

---

### 🤖 #2A gemma4:31b-cloud

Skillnaden mellan `em` och `rem` handlar om vad enheten baseras på (referenspunkten) för att beräkna storleken. Båda är relativa enheter, till skillnad från `px` som är en absolut enhet.

### 1. rem (Root em)
`rem` baseras alltid på **rot-elementets** (oftast `<html>`) typsnittsstorlek.
*   Standard i de flesta webbläsare är att rot-storleken är **16px**.
*   Om rot-storleken är 16px, innebär `1rem` = 16px och `2rem` = 32px.
*   **Fördel:** Det är konsekvent. Oavsett var på sidan elementet finns, kommer `1rem` alltid att vara samma storlek.

### 2. em
`em` baseras på **föräldraelementets** typsnittsstorlek.
*   Om ett föräldraelement har en storlek på 20px, kommer `1em` inuti det elementet att vara 20px och `2em` att vara 40px.
*   **Fördel:** Det är användbart när du vill att utrymmen (som padding eller margin) ska skala proportionellt i förhållande till textstorleken i just den komponenten.

---

### Sammanfattning och exempel

| Enhet | Baseras på | Karaktär |
| :--- | :--- | :--- |
| **rem** | Rot-elementet (`<html>`) | Stabil och förutsägbar över hela sidan. |
| **em** | Närmaste förälder | Hierarkisk och kan "ärvas" (kumulativ). |

**Exempel på "problemet" med em (kumulativ effekt):**
Om du har en lista i listan och båda har `font-size: 0.5em`, kommer den inre listan bli extremt liten eftersom den tar 50% av förälderns 50%.

```css
/* Exempel */
html {
  font-size: 16px;
}

.box-rem {
  font-size: 2rem; /* Alltid 32px (16 * 2) */
}

.parent-em {
  font-size: 20px;
}

.child-em {
  font-size: 2em; /* Blir 40px (20 * 2) */
}
```
**Rekommendation:** Använd generellt `rem` för typsnitt och layout för att behålla kontrollen, och använd `em` för detaljer (som padding i en knapp) som ska ändras om du ändrar knappens textstorlek.

*(⏱ 2.64s)*

---

# CSS Selectors

| Selector | Example | Example description |
|---|---|---|
| `.class` | `.intro` | Selects all elements with `class="intro"` |
| `.class1.class2` | `.name1.name2` | Selects all elements with both `name1` and `name2` set within its class attribute |
| `.class1 .class2` | `.name1 .name2` | Selects all elements with `name2` that is a descendant of an element with `name1` |
| `#id` | `#firstname` | Selects the element with `id="firstname"` |
| `*` | `*` | Selects all elements |
| `element` | `p` | Selects all `<p>` elements |
| `element.class` | `p.intro` | Selects all `<p>` elements with `class="intro"` |
| `element,element` | `div, p` | Selects all `<div>` elements and all `<p>` elements |
| `element element` | `div p` | Selects all `<p>` elements inside `<div>` elements |
| `element>element` | `div > p` | Selects all `<p>` elements where the parent is a `<div>` element |
| `element+element` | `div + p` | Selects the first `<p>` element that is placed immediately after `<div>` elements |
| `element1~element2` | `p ~ ul` | Selects every `<ul>` element that is preceded by a `<p>` element |
| `[attribute]` | `[target]` | Selects all elements with a `target` attribute |
