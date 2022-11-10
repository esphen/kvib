---
id: tilleggskomponenterID
title: Tilleggskomponenter (Historiske kart)
description: Komponenter som ligger utenfor Figma-KVIB, og som ikke har noen godkjent design. Likvel er det tenkt at disse kan bli en del av KVIB etterhvert.
---

***OBS! Disse er IKKE GODKJENT av designer. Det mangler godkjent design i Figma-KVIB for disse komponentene, og de er dermed under konstruksjon.
De nåværende komponentene på siden er basert på en blanding av design fra kartverket.no, Figma-KVIB og Kartverket sin løsning for historiske kart.
De er i utgangspunktet tiltenkt å brukes i historiske kart, men kan bli del av KVIB når de er godkjent.***

***
## Vis/Skjul



<button class="button button__blue--secondary button--xs button--icon-left">Vis info
    <span class="material-symbols-outlined ">chevron_right</span></button>

<button class="button button__blue--secondary button--xs button--icon-left">Skjul info
    <span class="material-symbols-outlined ">chevron_left</span></button>

<button class="button button__blue--secondary button--xs button--icon-right">Vis filter
    <span class="material-symbols-outlined ">chevron_left</span></button>

<button class="button button__blue--secondary button--xs button--icon-right">Skjul filter
    <span class="material-symbols-outlined">chevron_right</span></button>


```markup
<button class="button button__blue--secondary button--xs button--icon-left">Vis info
    <span class="material-symbols-outlined ">chevron_right</span></button>

<button class="button button__blue--secondary button--xs button--icon-left">Skjul info
    <span class="material-symbols-outlined ">chevron_left</span></button>

<button class="button button__blue--secondary button--xs button--icon-right">Vis filter
    <span class="material-symbols-outlined ">chevron_left</span></button>

<button class="button button__blue--secondary button--xs button--icon-right">Skjul filter
    <span class="material-symbols-outlined">chevron_right</span></button>
```


### Tilhørende tertiærknapper med ikon

<button class="button button__blue--tertiary button--xs button--icon-right ">Fjern valgt kart
    <span class="material-symbols-outlined--filled material-symbols-outlined">cancel</span>
</button>


<button class="button button__blue--tertiary button--xs button--icon-right">Nullstill filter
    <span class="material-symbols-outlined--filled material-symbols-outlined">cancel</span>
</button>

```markup
<button class="button button__blue--tertiary button--xs button--icon-right ">Fjern valgt kart
    <span class="material-symbols-outlined--filled material-symbols-outlined">cancel</span>
</button>

<button class="button button__blue--tertiary button--xs button--icon-right">Nullstill filter
    <span class="material-symbols-outlined--filled material-symbols-outlined">cancel</span>
</button>
```

## Knapper med kun ikon (eks. zoom-knapp)
Disse knappene inneholder kun ikon, og er dermed mindre enn vanlig knapper som vanligvis også inneholder tekst.
Hittil er dette tiltenkt eksempelvis zoom-knapper, som brukes i kartløsninger.
CSS-klassen <code>.button--zoom</code> endrer størrelsen og margin til knappen.

OBS! Det er meningen at <code>.button--zoom</code> skal brukes generelt for alle knapper som kun skal inneholde ikon.
<button class="button button__blue--primary button--zoom">
    <span class="material-symbols-outlined">add</span></button>

<button class="button button__blue--primary button--zoom">
    <span class="material-symbols-outlined">remove</span></button>

```markup
<button class="button button__blue--primary button--zoom">
    <span class="material-symbols-outlined">add</span></button>

<button class="button button__blue--primary button--zoom">
    <span class="material-symbols-outlined">remove</span></button>
```

## Kort

<div class="result__content__container">
    <img class="result__image" src="https://source.unsplash.com/random" alt="random unsplash"/>
    <div class="result__content__desc">
        <h3 class="result__title">Tittel</h3>
        <span class="result__desc">Årstall</span>
    </div>
</div>


