# Övningsrepo för flexbox

Jobba med [flexbox cheat sheet](https://yoksel.github.io/flex-cheatsheet/).

Gör kopior eller skapa egna startdokument för att testa olika layouter, du kan alltig utgå från [base](base.html).

## Övningar

Använd base.html. Först ska vi arbeta med att göra en enkel layout med flexbox.
De element vi ska ändra på är header, main och footer.

För att göra det lite enklare för oss så kommer vi att skapa en utilityklass som heter `d-flex` som vi kan använda för att sätta flexbox på element.

D står för display och flex är flexbox. Så `d-flex` betyder `display: flex`.

```css
.d-flex {
  display: flex;
}
```

Vi kan sedan använda klassen på elementen vi vill ha flexbox på.

```html
<header class="d-flex">
  <h1>Header</h1>
</header>
```

När detta är klart så kan vi börja anpassa layouten för varje element.

### Header

Headern innehåller en h1 och en logo. Vi vill att logon ska ligga till höger och h1:an till vänster. Använd justify-content och align-items för att placera elementen rätt.

### Main

Main elementets innehåll är ett antal kort. Vi vill placera korten i en rad och att de ska vara lika stora. Använd flexbox för att placera korten i en rad.

Du kan sedan justera storleken på korten genom att använda flex-grow. Kolla även wrap. Testa gärna att byta direction.

### Footer

Footern är ganska lika headern. Vi vill att texten ska vara till vänster och länkarna till höger. Använd justify-content och align-items för att placera elementen rätt.

## Luft

Glöm inte att använda luft mellan elementen. Använd margin och padding för att skapa detta! För flex-box kan du också använda `gap` för att skapa luft mellan elementen.

´´´css
.d-flex {
  display: flex;
  gap: 1rem;
}
´´´

## Undantag

Ibland kan vi behöva göra undantag för att visa/dölja element på olika skärmstorlekar. 
Vi kan då använda oss av media queries för att göra detta.

```css
@media screen and (max-width: 600px) {
  .d-flex {
    flex-direction: column;
  }
}
```


## Kort

Kort eller cards är en vanlig layout som används på många webbsidor.

Om du är klar med den första delen så kan du nu arbeta med att skapa kortens layout med flexbox. Du kan använda `d-flex` klassen för att sätta flexbox på korten.

Styr sedan hur elementen placeras. Ett tips är att försöka göra så att korten är lika stora. Att korten med bild är lika stora som de utan bild, samt att bilden kanske är kvadratisk och att texten hamnar ovanpå bilden.

### Länkar

https://m3.material.io/components/cards/overview
https://devdevout.com/css/css-cards

## Nav

Om du provar att göra flera sidor så kan du även testa att göra en navigationsmeny. Använd flexbox för att placera elementen i en rad.

Använd nav elementet och ersätt header. Använd listor för att skapa länkar.
Formatera sedan detta med flexbox.

## Hosting

När du är klar med övningen så kan du publicera den på GitHub Pages. Se till att pages är aktiverat på ditt repo och att du har en index.html fil i rotmappen.