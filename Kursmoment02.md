# CSS

## Innehåll
- [Fråga #1](#fråga-1)
- [Fråga #2](#fråga-2)
- [CSS Selectors](#css-selectors)
- [External Fonts](#external-fonts)
- [Text-transform och Radavstånd](#text-transform)
- [Block](#block)
- [Margins](#margins)
- [Box sizing](#box-sizing)
- [Block- och inline-element](#block-och-inline-element)

[HTML Styles - CSS w3schools](https://www.w3schools.com/html/html_css.asp)

Saved: 2026-09-21T22:46:15.804604

## ❓Fråga #1

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

[⬆️ Till innehåll](#innehåll)

## ❓Fråga #2

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

[⬆️ Till innehåll](#innehåll)

# CSS Selectors

| Selektor | Exempel | Beskrivning |
|---|---|---|
| `.class` | `.intro`       | Väljer alla element med `class="intro"` |
| `.class1.class2` | `.name1.name2` | Väljer alla element som har både `name1` och `name2` i sitt `class`-attribut |
| `.class1 .class2` | `.name1 .name2` | Väljer alla element med `name2` som finns inuti ett element med `name1` |
| `#id` | `#firstname` | Väljer elementet med `id="firstname"` |
| `*` | `*` | Väljer alla element |
| `element` | `p` | Väljer alla `<p>`-element |
| `element.class` | `p.intro` | Väljer alla `<p>`-element med `class="intro"` |
| `element,element` | `div, p` | Väljer alla `<div>`-element och alla `<p>`-element |
| `element element` | `div p` | Väljer alla `<p>`-element som finns inuti `<div>`-element |
| `element > element` | `div > p` | Väljer alla `<p>`-element som är direkta barn till ett `<div>`-element |
| `element + element` | `div + p` | Väljer det första `<p>`-elementet som kommer direkt efter ett `<div>`-element |
| `element1 ~ element2` | `p ~ ul` | Väljer alla `<ul>`-element som kommer efter ett `<p>`-element |
| `[attribute]` | `[target]` | Väljer alla element som har attributet `target` |

### Kort förklaring

Det är lätt att blanda ihop några av CSS-selektorerna:

- `.class1.class2` – elementet har **båda klasserna**.
- `.class1 .class2` – `.class2` finns **inuti** `.class1`.
- `div p` – alla `<p>` som finns **någonstans inuti** `<div>`.
- `div > p` – `<p>` är ett **direkt barn** till `<div>`.
- `div + p` – det första `<p>` som kommer **direkt efter** `<div>`.
- `p ~ ul` – alla `<ul>` som kommer **efter** en `<p>` på samma nivå.

**Kort sagt:** mellanslag, `>`, `+` och `~` beskriver olika relationer mellan element.


[⬆️ Till innehåll](#innehåll)

---

### Text-transform
```html
h1 {
text-transform: uppercase;
}
h2 {
text-transform: capitalize;
}
h3 {
text-transform: lowercase;
}
```
### Radavstånd
```html
p {
line-height: 2em;
}
```

---

### External Fonts

You probably don't like falling back on the fonts stored locally. Luckily, we can always use an external font with the [`@font-face`](https://www.w3schools.com/cssref/css3_pr_font-face_rule.php) rule. Just need to specify the font's name and its path:

`@font-face { font-family: CustomFont; src: url(fonts/custom_font.woff); } html { font-family: CustomFont; }`

Programmers, like everyone else, like freebies, and the go-to place for free fonts is [Google Fonts](https://fonts.google.com/). Here's how to use them:

- Choose the desired font and style.
- Copy the tags displayed on the right and paste them into the `<head>` of your page:

```html
<head>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&display=swap" rel="stylesheet">
</head>
```
Woohooo! This font is now available in your CSS:

```css
body { font-family: 'Roboto', sans-serif; }
```

---
[⬆️ Till innehåll](#innehåll)

# Block 

## Egenskapen display

Med hjälp av egenskapen display kan du t.ex. ändra inline till block.
```css
a {
width: 50px;
height: 50px;
background-color: black;
color: white;
display: block;
}
```

`display: block` placerar varje länk på en egen rad och låter oss ange `width` och `height`. 

## Inline-block

Du kan visa blocken bredvid varandra med display: inline-block
```css
a {
width: 50px;
height: 50px;
background-color: black;
color: white;
display: inline-block;
}
```

```html
<a href="#">Länk</a>
<a href="#">Länk</a>
```

`display: inline-block` låter länkarna ligga bredvid varandra samtidigt som `width` och `height` kan anges.


### Skillnaden mellan block och inline-block

`display: block` gör att varje länk tar upp hela raden, så länkarna placeras under varandra.  
`display: inline-block` gör att länkarna kan placeras bredvid varandra, samtidigt som man kan ange `width` och `height`.

På så sätt kan man ändra hur inline-elementen placeras och hur mycket utrymme de tar på sidan.

---

[⬆️ Till innehåll](#innehåll)

## Margins 

### margin collapse

När två element ligger nära varandra utan att det finns `border`, `padding` eller innehåll som separerar deras vertikala marginaler kan marginalerna **slås ihop**. Detta kallas **margin-kollaps** (*margin collapse*).

För att undvika detta kan man använda `padding` på det överordnade elementet. Man kan också ange `margin` endast på ena sidan längs varje axel: `top` och `bottom` för vertikalt avstånd eller `left` och `right` för horisontellt avstånd.

Både `margin` och `padding` kan anges i procent (`%`) i stället för pixlar. Procentvärdet beräknas utifrån förälderelementets bredd, även för `top` och `bottom`.

Man kan också använda `em` som enhet. Då kopplas avståndet till elementets `font-size`. Det kan skapa en mer harmonisk relation mellan textens storlek och utrymmet runt texten.

## Box sizing  

Egenskapen [**`box-sizing`**](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing) påverkar elementets bredd och höjd. Den kan ha två olika värden:

1. `content-box` – **exkluderar** `padding` och `border` från elementets angivna bredd och höjd.
2. `border-box` – **inkluderar** `padding` och `border` i elementets angivna bredd och höjd.

Här använder vi `box-sizing: border-box`, vilket innebär att själva innehållets bredd blir mindre än `300px`. Det beror på att `border` och `padding` räknas bort från varje sida


```css
.content {
  box-sizing: border-box;
  width: 300px;
  height: 150px;

  margin: 40px;
  border: 15px solid blue;
  padding: 30px;
}
````

## Block- och inline-element

Det vi har gått igenom ovan fungerar för `div`-element, men inte på samma sätt för `span`. Det beror på att `div` är ett **blockelement** (en rektangulär yta som innehåller innehåll), medan `span` är ett **inline-element** (en del av text som kan sträcka sig över en eller flera rader).

### 1. Blockelement

- Placeras på en egen rad.
- Tar som standard upp hela bredden av sitt förälderelement.
- Vi kan ange `width` och `height`.
- `padding`, `margin` och `border` påverkar det totala utrymmet som elementet tar upp.
- Exempel är `div`, `p`, `ul`, `li` och `h1`.

### 2. Inline-element

- Placeras på samma rad som andra inline-element.
- Tar bara upp så mycket bredd som innehållet behöver.
- Vi kan inte ange `width` och `height` på samma sätt som för blockelement.
- `padding`, `margin` och `border` ökar inte elementets höjd på samma sätt som för blockelement. Rader intill kan därför överlappa.
- Exempel är `span`, `a` och `em`.

## Inline-block-element

Ibland behöver vi ange en egen storlek och spacing för ett element som finns inne i texten, till exempel en länk. Då kan vi använda **inline-block**:

```
.nav__link {  display: inline-block;}
```

`inline-block` kombinerar egenskaper från både `inline` och `block`.

**Inline** eftersom elementet bara tar upp den bredd som behövs och kan placeras på samma rad som andra element.

**Block** eftersom vi kan ange `width` och `height`, och eftersom `padding`, `border` och `margin` påverkar det utrymme som elementet tar upp i alla riktningar.

**Som standard är `<img>` ett inline-block-element.**

För att bättre förstå skillnaden mellan `inline-block`, `block` och `inline` kan du titta på [**det här exemplet**](https://www.w3schools.com/css/tryit.asp?filename=trycss_inline-block_span1)

[⬆️ Till innehåll](#innehåll)

---

