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

**Bas HTNL document**<br>

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

## Semantiska element vs fysiska

https://dbwebb.se/guide/design-med-html5-och-css3/semantisk-html

## ❓ #2

1. Vet du historien bakom och skillnaden mellan fysiska och semantiska taggar i HTML?  
2. Vilka dök upp först, och hur aktuella är semantiska taggar idag?  
3. Kan båda typerna godkännas av HTML-validatorn?  
4. När är det lämpligt att använda fysiska taggar, och när är det lämpligt att använda semantiska?

---

### 🤖 #2A gemma4:31b-cloud

Här är svaren på dina frågor om fysiska och semantiska taggar, Alexander.

### 1. Historien bakom och skillnaden mellan fysiska och semantiska taggar
**Historien:**
I webbens tidiga dagar (HTML 1.0 och 2.0) var HTML främst utformat för att visa vetenskapliga dokument. Man behövde enkla sätt att styra utseendet direkt i koden, eftersom CSS inte existerade eller var utbrett. Därför skapades **fysiska taggar**; om man ville att något skulle vara fetstilt skrev man `<b>` (bold).

Efter hand insåg man att detta var problematiskt. Webbläsare och skärmläsare för synskadade visste *att* texten var fet, men inte *varför* den var fet. Var det för att det var viktigt, eller bara för att det såg snyggt ut? Detta ledde till utvecklingen av **semantiska taggar**, som beskriver innehållets betydelse (mening) snarare än dess utseende.

**Skillnaden:**
*   **Fysiska taggar:** Beskriver **presentation**. De säger till webbläsaren: *"Gör detta så här"*. (Exempel: `<b>` $\rightarrow$ "Gör texten fet").
*   **Semantiska taggar:** Beskriver **struktur och mening**. De säger till webbläsaren: *"Detta är vad innehållet är"*. (Exempel: `<strong>` $\rightarrow$ "Denna text är viktig").

### 2. Vilka dök upp först, och hur aktuella är semantiska taggar idag?
**Vilka kom först?**
De fysiska taggarna kom först. De var grunden i den tidiga HTML-standarden för att man snabbt skulle kunna formatera text.

**Hur aktuella är semantiska taggar idag?**
De är mer aktuella än någonsin. Med lanseringen av **HTML5** blev semantik centralt. Idag använder vi inte bara semantik för text (som `<strong>`), utan för hela sidans layout med taggar som `<header>`, `<footer>`, `<main>`, `<article>` och `<section>`.

Detta är kritiskt av två anledningar:
1.  **Tillgänglighet (Accessibility):** Skärmläsare använder semantiska taggar för att hjälpa användare att navigera på sidan.
2.  **SEO (Sökmotoroptimering):** Googles botar prioriterar semantiska taggar för att förstå vad som är den viktigaste informationen på en sida.

### 3. Kan båda typerna godkännas av HTML-validatorn?
**Ja.** Både fysiska och semantiska taggar är giltig HTML-kod och kommer att godkännas av en HTML-validator (som W3C Validator).

Det är dock viktigt att förstå att "giltig kod" inte nödvändigtvis är "best practice". Att använda `<b>` istället för `<strong>` är tekniskt sett korrekt kod, men det är inte optimalt för tillgänglighet och SEO.

### 4. När är det lämpligt att använda fysiska taggar, och när är det lämpligt att använda semantiska?

**Använd semantiska taggar (Förstavalet):**
I nästan alla fall. Du bör använda semantik när innehållet har en specifik betydelse.
*   Använd `<strong>` när texten är viktig.
*   Använd `<em>` när du vill betona ett ord.
*   Använd `<nav>` för menyer, `<article>` för blogginlägg, etc.
*   **Regel:** Om textens betydelse förändras eller förstärks av formateringen $\rightarrow$ använd semantik.

**Använd fysiska taggar (Undantagen):**
Använd fysiska taggar endast när du vill ändra utseendet av rent estetiska skäl, utan att tillskriva texten någon extra vikt eller betydelse.
*   Använd `<b>` om du vill att ett ord ska vara fetstilt bara för att det ska sticka ut visuellt (t.ex. produktnamn i en lista), men inte för att det är "viktigt" i kontexten.
*   Använd `<i>` för tekniska termer, utländska ord eller tankar som ska stå i kursiv stil utan att vara betonade.

**Proffstips:** I modern webbutveckling flyttar man oftast all visuell formatering till **CSS**. Om du bara vill att något ska se ut på ett visst sätt utan semantisk betydelse, är det ofta bäst att använda en `<span>` eller `<div>` och styra utseendet med en CSS-klass.

*(⏱ 11.28s)*

