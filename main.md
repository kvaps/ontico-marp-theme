---
marp: true
theme: base
style: |
  @font-face {
    font-family: 'TT Travels';
    font-weight: normal;
    src: url('img/TTTravels-Regular.ttf') format('truetype');
  }
  @font-face {
    font-family: 'TT Travels';
    font-weight: bold;
    src: url('img/TTTravels-DemiBold.ttf') format('truetype');
  }
  section {
    font-family: 'TT Travels';
    background: url(img/body.png);
    background-color: #fff;
    background-size: cover;
    color: #000;
    justify-content: flex-start;
    -webkit-justify-content: flex-start;
  }
  section.front {
    background: url(img/title.png);
    background-color: #005da9;
    background-size: cover;
    color: #fff;
  }
  section.front > h1 {
    width: 850px;
    color: #fff;
    font-size: 52px;
    padding-bottom: 0;
  }
  section.front > h2 {
    color: #fff;
    font-size: 35px;
    font-weight: normal;
    padding-top: 0;
  }
  section.front > h1 strong,
  section.front > h2 strong,
  section.invert > h1 strong,
  section.invert > h2 strong {
    color: #ed1c24;
  }
  section.invert {
    background: url(img/invert.png);
    background-color: #005da9;
    background-size: cover;
    color: #fff;
    text-align: center;
    display: table-cell;
    vertical-align: middle;
  }
  section.invert > h1 {
    color: #fff;
    font-size: 52px;
  }
  section.invert > h2 {
    color: #fff;
    font-size: 35px;
  }
  section a {
    color: #005da9;
  }
  h1,h2,h3,h4,h5,h6 {
    line-height: 1;
    color: #000;
    top: -17px;
    position: relative;
  }
  /* --------------------------- */
  div.version {
    position: absolute;
    right: 0;
    bottom: 0;
    font-size: 15px;
    padding-right: 5px;
  }
  section::after {
    color: #ccc;
    font-weight: bold;
    right: 130px;
    text-align: right;
  }
  img[alt~="center"] {
    display: block;
    margin: 0 auto;
  }
  img[alt~="right"] {
    display: block;
    float: right;
  }
  img[alt~="rightup"] {
    display: block;
    top: 0;
    right: 0;
    padding: 50px 50px 120px;
    position: absolute;
    background-color: transparent;
  }
  img[alt~="rightdown"] {
    display: block;
    bottom: 0;
    right: 0;
    padding: 90px 90px 120px;
    position: absolute;
    background-color: transparent;
  }
---

<!--
$size: 16:9
_class: front
-->

# В поисках идеальной кластерной ФС:<br> опыт использования LINSTOR

## Андрей Квапил

<div class="version">v0.0.1</div>

---

# Что нам было нужно от хранилища

- OpenSource

- Производительность

- Надёжность

- Отказоустойчивость

- Простая интеграция

- Бесшовная миграция и обновление

- Снапшоты

![h:300 rightdown](img/vovka.png)

---

# Типы хранилищ


* POSIX-совместимая файловая система

* Блочное хранилище

* Объектное хранилище

![h:250 rightdown](img/box.png)

---

## Отказоустойчивый NFS-сервер

![center](img/nfsa.svg)

---

## Отказоустойчивый NFS-сервер

![center](img/nfsb.svg)

---

<!-- _backgroundColor: "#000" -->

![bg 74%](img/satana.jpg)

---

# Бэкапы

![w:210px rightup](img/backups.png)

- Resitc — отлично подходит для
  бэкапа блочных устройств

- Дедупликация работает из коробки

- Снапшоты для консистентности

- ZFS DRAID on the backend
  <br>

<small>

> *Бэкап-хранилище для тысяч виртуальных машин свободными инструментами*
> https://habr.com/ru/post/504152/

</small>

---

<!-- _class: invert -->

# Вопросы?

---

![bg](img/contacts.png)
