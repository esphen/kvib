---
id: navID
title: Navigasjon
description: Navigasjon
slug: /designsystem/komponenter/navigasjon
displayed_sidebar: designsystemSidebar
---

## Header
Navigasjonsbar-elementet tilpasser seg til skjermstørrelsen siden er åpnet i.
Hvis det er nødvendig med spesifikk størrelse på navigasjonsbaren, må elementet bli plassert i en <code><div\></code> med ønsket width.

### Header med ikon

<nav class="nav__header">
<img src="../../img/logo/KV_M.svg" alt="Kartverket Logo"/>
<span class="material-symbols-outlined">person</span>
</nav>

### Header uten ikon

<nav class="nav__header">
<img src="../../img/logo/KV_M.svg" alt="Kartverket Logo"/>
</nav>

<br/>

```markdown
<nav class="nav__header">
<img src="../../img/logo/KV_M.svg" alt="Kartverket Logo"/>
<span class="material-symbols-outlined">person</span>
</nav>

<nav class="nav__header">
<img src="../../img/logo/KV_M.svg" alt="Kartverket Logo"/>
</nav>
```

## Ankermeny
Ankermeny kan brukes på sider med mye innhold. Ved å trykke på menyen scroller man ned til overskriften.

<div class="display__nav">
    <div class="display__nav__item">
        <div class="display__nav__container">
                <div class="anker--xs">
                <span class="material-symbols-outlined material-symbols-outlined--xs">arrow_downward</span>
                <a href="#id" class="heading heading__h3--xs">Input</a>
                </div>
        </div>
        <div class="display__nav__desc">anker--xs</div>
    </div>
 <div class="display__nav__item">
        <div class="display__nav__container">
                <div class="anker--s">
                <span class="material-symbols-outlined">arrow_downward</span>
                <a href="#id" class="heading heading__h3--sm">Input</a>
                </div>
        </div>
        <div class="display__nav__desc">anker--s</div>
    </div>
 <div class="display__nav__item">
        <div class="display__nav__container">
                <div class="anker--m">
                <span class="material-symbols-outlined">arrow_downward</span>
                <a href="#id" class="heading heading__h3--sm">Input</a>
                </div>
        </div>
        <div class="display__nav__desc">anker--m</div>
    </div>
 <div class="display__nav__item">
        <div class="display__nav__container">
                <div class="anker--l">
                <span class="material-symbols-outlined">arrow_downward</span>
                <a href="#id" class="heading heading__h3--l">Input</a>
                </div>
        </div>
        <div class="display__nav__desc">anker--l</div>
    </div>
</div>

<br/>

### Eksempelbruk

Størrelsen endres ved å bytte klassen <code>anker--xs</code> til <code>anker--m</code>.

```markdown
<div class="anker--xs">
<span class="material-symbols-outlined">arrow_downward</span>
<a href="#id">Input</a>
</div>
```


## Tabs
Følgende element bruker <code>active__link--demo</code>-klasse for å demonstrere et valgt eller aktivt side. Dette må justeres i hvert prosjekt.

<div class="tab">
  <button class="tab__links active__link--demo" onclick="#function()">En</button>
  <button class="tab__links" onclick="#function()">To</button>
  <button class="tab__links" onclick="#function()">Tre</button>
</div>

<br/>

```markdown
<div class="tab">
  <button class="tab__links" onclick="#function()">En</button>
  <button class="tab__links" onclick="#function()">To</button>
  <button class="tab__links" onclick="#function()">Tre</button>
</div>
```

## Stegvise prosesser

### Visning på liten skjerm (Extra small/small)
Stegvise prosesser visning på liten skjerm bruker <code>--s</code>-klasse. <code>aria-current="step"</code> settes på <code><li\></code>-elementet eller nåværende steg der bruker er på. Ved fullført steg, settes <code>data-status="complete"</code> på <code><li\></code>-elementet.

<div class="stepper--s">
    <ol role="list" aria-label="Stegnavn">
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li aria-current="step">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
    </ol>
</div>

<br/>

```markdown
<div class="stepper--s">
    <ol role="list" aria-label="Stegnavn">
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li aria-current="step">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
    </ol>
</div>
```


### Visning på stor skjerm (medium/large)
Stegvise prosesser visning på stor skjerm bruker <code>stepper--l</code>-klasse. <code>aria-current="step"</code> settes på <code><li\></code>-elementet eller nåværende steg der bruker er på. Ved fullført steg, settes <code>data-status="complete"</code> på <code><li\></code>-elementet.

<div class="stepper--l">
    <ol role="list" aria-label="Stegnavn">
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li aria-current="step">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
    </ol>
</div>

<br/>

```markdown
<div class="stepper--l">
    <ol role="list" aria-label="Stegnavn">
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="label label--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li data-status="complete">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li aria-current="step">
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
        <li>
            <div class="stepper__circle label label--sml"></div>
            <label class="detail detail--sml">Input Tekst</label>
        </li>
    </ol>
</div>
```



