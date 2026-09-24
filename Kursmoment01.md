# Innehåll
- [Bas HTML document](#Bas-HTML-document)
- [Tags övning](#tags-övning)
- [❓ Figure, hgroup, figcaption]((#-1-figure-hgroup-figcaption))

# Kursmoment 1. ”Grunderna HTML ”

• Internets historia, teknik och utveckling<br>
• Webstandarder<br>
• Introduktion – VS Code<br>
• HTML Basics<br>

**QSTNS och [ANSWRS](https://github.com/WEBD26JON/HTML-CSS/blob/main/ANSWRS.md)**<br>
·        Vad är HTML?<br>
·        Grundstuktur i HTML?<br>
·        Förklara skillnaden mellan taggar och attribut i HTML?<br>
·        Vad är skillnaden mellan fysiska och semantiska element?<br>
·        Vad är skillnaden mellan `<b> och <strong>` ?<br>
·        Vad är skillnaden mellan `<i> och <em>` ?<br>
·        Vad är skillnaden mellan `<blockquote> och <cite>` <br>
·        Vad är skillnaden mellan `UL och OL` ?<br>
·        Hur används DL-taggen i HTML?<br>
·        Vad är URL? Vad är skillnaden mellan en absolut URL och en
·        relativ/lokal URL?<br>
·        Hur skapar du länkar som öppnas i nya flikar?<br>
·        Externa länkar måste innehålla ett protokoll. Vad innebär det?<br>
·        Vilka bildformat används på webben?<br>
·        Vilka attribut är obligatoriska i en img-tagg?<br>
·        I vilket syfte används en GIF-bild på webben?<br>
·        Vilka element bildar upp en tabell i HTML? <br>
·        Hur sammanfogar man tre celler i en rad? Skriv ett exempel.<br>
·        Vilka element behövs för att skapa ett inloggningsformulär i HTML?<br>
·        Vad innebär formulärvalidering? Skriv några exempel!<br>
·        Hur fungerar iframe-taggen?<br>
·        Vilka taggar och attribut är viktiga för att spela upp ljud i HTML?<br>
·        Vilka taggar och attribut är viktiga för att spela upp video i HTML?<br>



- [HTML & CSS Full Course - Beginner to Pro](https://www.youtube.com/watch?v=G3e-cpL7ofc&t=62s) - 
SuperSimpleDev
- [HTML Examples](https://www.w3schools.com/html/html_examples.asp)
- [internetmuseum](https://internetmuseum.se/)
- [Lysator](https://www.lysator.liu.se/)

  Vad består en webbplats av?<br>
  Interaktivitet - Java Script, Utseende - CSS, Innehåll - Innehåll, Struktur - HTML

HTML standart.<br>
  https://www.w3.org/<br>
  https://html.spec.whatwg.org/

https://github.com/Nina3211/Nina3211.github.io
  
W3S validator<br>
https://validator.w3.org/#validate_by_uri+with_options<br>
https://caniuse.com/<br>

## Bas HTML document

HTML tags:<br>
```
https://www.w3schools.com/tags/<br>
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exempel 1</title>
</head>
<body>
    
</body>
</html>
```
[⬆️ Till innehåll](#innehåll)

## Tags övning
```
<!DOCTYPE html>
<html lang="sv">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Fysiska och semantiska element</title>
</head>
<body>
    <h1>Textformatering</h1>
    <h2>Fysiska element</h2>
    <hr>

    <h3>Fet och kursiv</h3>
    <p>
        Text utan stil <br>
        <b>Lite fet stilad text</b><br>
        <i>Lite kursiv text.</i>
    </p>
    <hr>

    <h3>Upphöjd och nedsänkt</h3>
    <p>
        Text utan stil <br>
        Area: 25m<sup>2</sup><br>
        Vatten: H<sub>2</sub>0 
    </p>

    <h2>Semantiska element</h2>
    <h3>Em och Strong</h3>
    <p>
        <em>Betoning av text</em><br>
        I <em>think</em>, she was the first here.<br>
        <strong>Beware:</strong>
        Pickpockets operate in this area.
    </p>
    <hr>
    <h3>Markeringspenna</h3>
    Här kommer lite <mark>viktig info om kursen</mark> HTML och CSS
    <hr>
    <h3>Citat</h3>
    <blockquote cite="www.brainyquote.com">
        "Did you ever stop to think, and forget to start again?"
    </blockquote>

    <p>
        As A.A.Milane sad, <q>Some people talk to animals. Not many listen.</q>
    </p>
    <cite>A Brief History of Time</cite> by Stephen Hawking
    <h3>Address</h3>
    <address>
        <p>
            TUC Sweden <br>
            Gatan 34A <br>
            172 80 Stockholm
        </p>
    </address>
</body>
</html>
```

[⬆️ Till innehåll](#innehåll)

# Lektion 2

Dagens agenda<br>
Interaktiva element, forms och validering<br>
HTML Listor<br>
HTML Länkar<br>
HTML Tabell<br>
HTML Bilder, Video och Ljud<br>
HTML Formulär och form validering<br>

https://emmet.io/<br>
https://picsum.photos/<br>

## Övningar
Övming 1 - [Code](ovningar/ovningar1-4-2026-09-15.html)   -  [www page](https://webd26jon.github.io/HTML-CSS/ovningar/ovningar1-4-2026-09-15.html)

---

[⬆️ Till innehåll](#innehåll)

## ❓#1 Figure, hgroup, figcaption

**Kan du förklara mig användning av `<figure>, <hgroup> och <figcaption>` tagar i den HTML koden?**  
  
        <section class="courses">  
            <article>  
                <figure>  
                    <img src="images/bok-choi.jpg" alt="Bok Choi">  
                    <figcaption>Bok Choi</figcaption>  
                </figure>  
                <hgroup>  
                    <h2>Japanese Vegetarian</h2>  
                    <h3>Five week course in london</h3>  
                </hgroup>  
                <p>A dive week introduction to traditional Japanese vegetarian meals,  
                    teaching you a selection of rice and noodle dishes.  
                </p>  
            </article>  
            <article>  
                <figure>  
                    <img src="images/teriyaki.jpg" alt="Teriyaki sauce">  
                    <figcaption>Teriyaki</figcaption>  
                </figure>  
                <hgroup>  
                    <h2>Sauces Masterclass</h2>  
                    <h3>One day workshop</h3>  
                </hgroup>  
                <p>An intensive one-day course looking at how to create the most   
                    delicious sauces for use in a range of Japanese cookery.  
                </p>  
            </article>  
        </section>

---

### 🤖 #1A glm-5.3-flash:cloud

Absolut! Dessa tre taggar är **semantiska HTML5-element** som ger innehållet struktur och mening. Här är en förklaring av var och en:

## `<figure>` – Självständigt innehåll

```html
<figure>
    <img src="images/bok-choi.jpg" alt="Bok Choi">
    <figcaption>Bok Choi</figcaption>
</figure>
```

`<figure>` används för att omsluta innehåll som är **självständigt** – t.ex. bilder, diagram, illustrationer eller kodexempel. Innehållet hör till sidans ämne, men kan flyttas (t.ex. till sidan av texten) utan att dokumentets mening förändras. I din kod innehåller figuren en bild av rätten som kursen handlar om.

## `<figcaption>` – Bildtext till figuren

```html
<figcaption>Bok Choi</figcaption>
```

`<figcaption>` definierar en **rubrik/beskrivning** för innehållet i `<figure>`. Den fungerar som en bildtext. Regeln är att den ska vara **det första eller sista elementet** inuti `<figure>` – i din kod ligger den sist. Fördelen är att kopplingen mellan bild och text blir tydlig, både för webbläsare, skärmläsare och sökmotorer.

## `<hgroup>` – Gruppering av rubriker

```html
<hgroup>
    <h2>Japanese Vegetarian</h2>
    <h3>Five week course in london</h3>
</hgroup>
```

`<hgroup>` grupperar flera rubrikelement (h1–h6) som hör ihop, t.ex. en **huvudrubrik** (h2) med en **underrubrik** (h3). Det signalerar att de två raderna tillsammans utgör en enda rubrik.

**Värt att veta:** `<hgroup>` har en omdiskuterad historik – det togs bort ur W3C:s HTML5-specifikation 2014 men finns sedan 2016 i WHATWG:s HTML Living Standard. Idag är det ett relativt ovanligt element, och samma struktur kan lika gärna skrivas utan det:

```html
<h2>Japanese Vegetarian</h2>
<p class="subtitle">Five week course in London</p>
```

## Så fungerar strukturen i din kod

```html
<article>                  <!-- Varje kurs är en egen artikel -->
    <figure>               <!-- Bild med bildtext -->
        <img ...>
        <figcaption>Bok Choi</figcaption>
    </figure>
    <hgroup>               <!-- Kursnamn + underrubrik -->
        <h2>...</h2>
        <h3>...</h3>
    </hgroup>
    <p>...</p>             <!-- Kursbeskrivning -->
</article>
```

Fördelen med dessa semantiska taggar jämfört med enbart `<div>` är att sidans struktur blir **begriplig för maskiner** – sökmotorer kan förstå vad som är rubriker, bilder och beskrivningar, vilket förbättrar tillgänglighet och SEO.

*(⏱ 13.93s)*

---

### 🤖 #1B gemma4:31b-cloud

Hej Alexander. Här är en förklaring av hur dessa taggar används i din kod:

### `<figure>`
Taggens syfte är att gruppera ett självständigt innehåll, oftast en bild, ett diagram eller ett kodexempel, tillsammans med en beskrivning. 
*   **I din kod:** Den används för att kapsla in bilden (`<img>`) och dess bildtext (`<figcaption>`) så att webbläsaren och skärmläsare förstår att dessa två hör ihop.

### `<figcaption>`
Detta är en bildtext (caption) till innehållet i en `<figure>`. 
*   **I din kod:** Den används för att ge bilden ett synligt namn eller en beskrivning, till exempel "Bok Choi" eller "Teriyaki". Den placeras alltid inuti en `<figure>`-tagg.

### `<hgroup>`
Denna tagg används för att gruppera flera rubriker som hör ihop, vanligtvis en huvudrubrik (`<h2>`) och en underrubrik (`<h3>`). 
*   **I din kod:** Den används för att samla kursens namn ("Japanese Vegetarian") och kursens detaljer ("Five week course in london"). Detta talar om för sökmotorer och hjälpmedel att dessa rubriker tillsammans utgör en enhetlig rubriksektion för artikeln.

**Sammanfattning:**
*   `<figure>` = Behållaren för bild och text.
*   `<figcaption>` = Själva texten som beskriver bilden.
*   `<hgroup>` = Gruppering av rubrik och underrubrik.

*(⏱ 2.35s)*

[⬆️ Till innehåll](#innehåll)

