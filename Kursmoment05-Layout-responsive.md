# Kursmoment 5 - "Layout och responsive webb"

•	Web Content Accessibility Guidelines (WCAG)<br> 
•	HTML5 Layout, Arbeta med flexbox<br>
•	Responsive webb -https://www.w3schools.com/css/css3_mediaqueries.asp<br>
        https://interactivecss.com/css-media-queries-interactive-tutorial/

## Inför kursmoment 5

**Flexbox - Kolla material publicerad i Flex under denna kursmoment, sen:**
- [Learn CSS Flexbox in 20 Minutes (Video-Course)](https://www.youtube.com/watch?v=wsTv9y931o8) - https://coding2go.com/
- Prova dessa interaktiva övningar först : 
[Flexbox Froggy - Ett spel för att lära sig CSS flexbox](https://flexboxfroggy.com/#sv)  
[Grid Garden - Ett spel för att lära sig CSS grid](https://cssgridgarden.com/#sv)  

Eller denna resurs;  
[Introduction to Flexbox | The Odin Project](https://www.theodinproject.com/lessons/foundations-introduction-to-flexbox)  

För att träna på det kan ni göra följande projekt:  
[Project: Landing Page | The Odin Project](https://www.theodinproject.com/lessons/foundations-landing-page)  

Eller [CSS Flexbox Project for Complete Beginners (Testimonial Grid)](https://www.youtube.com/watch?v=n0QmD2i90_c&list=PL12XW6i6zqKtwRpElrrP3tpH4hdSgsRAb)

**Responsive webb**<br> 
https://www.w3schools.com/css/css3_mediaqueries.asp  
https://interactivecss.com/css-media-queries-interactive-tutorial/

**WCAG Guidelines**  
https://www.w3.org/WAI/standards-guidelines/wcag/glance/  
WCAG Guidelines - referens lista  
https://www.w3.org/WAI/WCAG22/quickref/?showtechniques=314#compatible

---

## Instudieringsfrågor

• Vad är skillnaden mellan statisk och relativ positionering?  
• Hur fungerar absolut positionering i CSS?  
Vilka egenskaper är viktiga?  
• Vad innebär fixerad positionering i CSS?  
• Floatmodellen har ett problem med alla element som hamnar efter flytande element.  
Förklara och beskriv minst en lösning till detta!  
• Vilka är de viktigaste layout-elementen i HTML5?


### 🤖 Svar på instudieringsfrågor

Här är svaren på dina instuderingsfrågor frågor om CSS-positionering och HTML5-layout.

### Statisk vs. Relativ positionering

*   **Statisk (`position: static`):** Detta är standardvärdet för alla element. Elementet följer det normala dokumentflödet. Egenskaperna `top`, `right`, `bottom`, `left` och `z-index` har ingen effekt.
*   **Relativ (`position: relative`):** Elementet behåller sin plats i det normala dokumentflödet, men kan flyttas i förhållande till sin ursprungliga position med hjälp av `top`, `right`, `bottom` och `left`. Viktigt är att utrymmet där elementet ursprungligen låg kvarstår; det lämnar alltså ett "tomrum" efter sig.

### Absolut positionering i CSS

**Hur det fungerar:**
Ett element med `position: absolute` tas helt ur dokumentflödet. Det betyder att andra element beter sig som om det absoluta elementet inte finns. Det positioneras i förhållande till sin **närmaste positionerade förälder** (ett element som har `position` satt till något annat än `static`, till exempel `relative`, `absolute` eller `fixed`). Om ingen sådan förälder finns, positioneras det i förhållande till webbläsarfönstret (`body`).

**Viktiga egenskaper:**
*   `top`, `bottom`, `left`, `right`: Bestämmer avståndet från referenspunkten.
*   `z-index`: Bestämmer i vilket lager elementet ligger (vilket element som hamnar "överst" om de överlappar).

### Fixerad positionering i CSS

**Fixerad positionering (`position: fixed`):**
Elementet tas ur dokumentflödet och låses till en specifik position i förhållande till **webbläsarfönstret (viewporten)**. Det betyder att elementet stannar kvar på samma ställe på skärmen även när användaren scrollar på sidan. Det används ofta för navigationsmenyer (headers) eller "tillbaka till toppen"-knappar.

### Floatmodellen och dess problem

**Problemet:**
När ett element ges `float: left` eller `float: right`, tas det delvis ut ur flödet. Element som kommer efter det i HTML-koden kommer att flyta upp och fylla utrymmet bredvid det flytande elementet. Om det flytande elementet är det sista i en behållare (container), kan behållaren "kollapsa" (få höjden 0) eftersom den inte räknar med höjden på det flytande elementet.

**Lösning: Clearfix**
Den vanligaste lösningen är att använda `clear`. Man kan antingen lägga till ett tomt element med `clear: both` efter det flytande elementet, eller använda en "clearfix"-klass på föräldraelementet:

```css
.clearfix::after {
  content: "";
  display: table;
  clear: both;
}
```
Detta tvingar föräldraelementet att expandera för att inkludera alla sina flytande barn.

### Viktigaste layout-elementen i HTML5

HTML5 introducerade semantiska element som beskriver innehållet för både webbläsaren och sökmotorer, istället för att bara använda `<div>`. De viktigaste är:

*   `<header>`: Sidans eller en sektions huvuddel (ofta logotyp och meny).
*   `<nav>`: Innehåller navigeringslänkar.
*   `<main>`: Det dominerande och unika innehållet på sidan.
*   `<section>`: En tematisk gruppering av innehåll.
*   `<article>`: Självständigt innehåll som kan distribueras separat (t.ex. ett blogginlägg).
*   `<aside>`: Innehåll som är indirekt relaterat till huvudtexten (t.ex. en sidomeny).
*   `<footer>`: Sidans eller en sektions botten (ofta kontaktinfo och copyright).

*(⏱ 5.40s)*

