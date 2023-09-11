# Vite Dc Comics

## PART 1

Descrizione:
Create un nuovo progetto utilizzando Vite e Vue 3 e definite i componenti necessari per strutturare il layout come da screenshot allegato.
Quando la struttura a macroblocchi è pronta, popolate le voci di menu dinamicamente usando i data del componente.
Per oggi diamo priorità alla struttura: quando è tutto bello solido, passiamo al Sass!
Bonus:
Creare un componente aggiuntivo per gestire la fascia azzurra con le icone.

## PART 2

Continuate a lavorare nella stessa repo di ieri e create un nuovo componente che rappresenterà le card dei fumetti.
Utilizzate i dati presenti nel file json che trovate in allegato e passateli al componente Card tramite props.
Una volta inseriti tutti i contenuti dinamicamente, completate il vostro layout e rifinite i dettagli con Sass.

## STEPS

- Divide the App in five _components_.
  1. Header (NAV)
  2. Content Bar
  3. Products Bar
  4. Footer Links
  5. Footer Socials

## 1. Header

- Header divided in two parts:
  - Logo.
  - Navigation Menu.

The Nav-menù work with an array and a cicle v-for that generate all the items.

## 2. Content Bar

Content Bar is divided in two parts:

- Jumbotron.
- Cards container :
  - The card template is writed in a new component (ComicCard)and generated with the props system inside the ContentBar (Component).

I create a comics.js file inside a new folder "data" for the array of objects (card content) and imported inside ContentBar container.

## 3. Products Bar

The product bar have just a single container that generate the element with a v-for cicle.

## 4. Footer Links

The footer links component have a main container with an background image and two different containers: - Links - Logo

Links are divided in multiple array and generated with a v-for cicle too.

## 5. Footer Socials

Finally here is the FooterSocials(component) divided in two main parts:

- Button
- Follow Us and Icons.

## Extra

I add some visive hover effects all around the app like font color change, buttom color changes and a scale effect for the cards of the comics.

---

### Vue 3 + Vite

This template should help get you started developing with Vue 3 in Vite. The template uses Vue 3 `<script setup>` SFCs, check out the [script setup docs](https://v3.vuejs.org/api/sfc-script-setup.html#sfc-script-setup) to learn more.

### Recommended IDE Setup

- [VS Code](https://code.visualstudio.com/) + [Volar](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (and disable Vetur) + [TypeScript Vue Plugin (Volar)](https://marketplace.visualstudio.com/items?itemName=Vue.vscode-typescript-vue-plugin).
