# Bootstrap gyakorló oldal – dokumentáció

Ez a projekt egy **Bootstrap 5** alapú gyakorló weboldal, amely bemutatja a keretrendszer legfontosabb elemeit: rácsszerkezet (grid), carousel, navigáció, táblázat, képek és segédosztályok használata.

---

## Mi az a Bootstrap?

A **Bootstrap** egy nyílt forráskódú **CSS és JavaScript keretrendszer**, amely segít:

- reszponzív (mobilbarát) weboldalak készítésében  
- egységes kinézet kialakításában  
- az előre elkészített css osztályokat a html-be írjuk bele, ezzel téve gyorsabbá a fejlesztést.

A projekt a **Bootstrap 5.3.x** verziót használja CDN-en keresztül.

---

## Használt Bootstrap elemek az oldalon

### 1. Grid rendszer (oldal felépítése)

Az oldal elrendezése a Bootstrap **12 oszlopos grid rendszerére** épül.

Használt osztályok:
- `container`
- `row`
- `col-12`
- `col-3`, `col-9`
- `col-sm-4`

- Példa HTML szerkezet:
```html
<div class="row">
  <aside class="col-3"></aside>
  <article class="col-9"></article>
</div>
```
- Így két oszlopunk lesz 3:9 arányban

### 2. Carousel (képváltó fejléc)

Az oldal tetején egy **Bootstrap Carousel** található, amely képeket vált automatikusan vagy vezérlőgombokkal.

Használt elemek:
- `carousel`
- `carousel-inner`
- `carousel-item`
- navigációs gombok
- indikátorok

- Példa saját CSS módosításra:
```css
.carousel img {
  max-height: 500px;
  object-fit: cover;
}
```
- saját css-el módosítható minden elem ugyanúgy mint sima css használatánál.

### 3. Navigációs sáv (nav)

Az oldal egy egyszerű Bootstrap navigációs menüt használ.

Használt osztályok:
- `nav`
- `nav-item`
- `nav-link`
- `bg-primary`
- `text-light`

- Példa HTML navigációra:
```html
<nav class="bg-primary p-4">
  <ul class="nav">
    <li class="nav-item">
      <a class="nav-link text-light" href="#">Menüpont</a>
    </li>
  </ul>
</nav>
```
- Ez automatikusan eltűnteti az aláhúzást, és horizontális menüt ad

### 4. Oldalsáv – Listák (list-group)

Az `aside` részben egy Bootstrap **list-group** található.

Használt osztályok:
- `list-group`
- `list-group-item`
- `text-primary`

- Példa lista HTML-re:
```html
<ul class="list-group">
  <li class="list-group-item text-primary">Elem</li>
</ul>
```
- Szebb formázást ad, és eltűnteti a pontokat

### 5. Táblázat (table)

A túraadatok Bootstrap táblázattal jelennek meg.

Használt osztályok:
- `table`
- `table-striped`
- `table-responsive-xl`

- Példa HTML táblázatra:
```html
<div class="table-responsive-xl">
  <table class="table table-striped"></table>
</div>
```
-Ez csíkos reszponzív táblázatot ad.

### 6. Képek kezelése

Bootstrap képosztályok használata:

- `img-fluid` – reszponzív méretezés
- `img-thumbnail` – keretes kép
- `rounded-circle` – kör alakú kép

- Példa HTML képre:
```html
<img src="kep.jpg" class="img-fluid img-thumbnail" alt="">
```
- Reszponzív képek, lekerekítés, alap border

### 7. Flexbox (footer szakasz)

A lábléc Bootstrap **Flex segédosztályokkal** van kialakítva.

Használt osztályok:
- `d-flex`
- `align-items-center`
- `flex-grow-1`
- `flex-shrink-0`
- `ms-3`

- Példa HTML Flex elrendezésre:
```html
<div class="d-flex align-items-center">
  <div class="flex-shrink-0"></div>
  <div class="flex-grow-1 ms-3"></div>
</div>
```
- Egymás mellé helyezés, stb.

### 8. Színek és tipográfia

Bootstrap segédosztályok használata.

**Színek**
- `bg-light`
- `bg-primary`
- `text-primary`
- `text-light`

**Tipográfia**
- `fw-light`, `fw-normal`
- `fst-italic`
- `display-6`

- Példa HTML szövegre:
```html
<p class="fw-light fst-italic text-primary">Szöveg</p>
```
- Ezek előre meghatározott osztályok, különböző hatásokkal. primary például kék. 

