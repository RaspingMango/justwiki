---
description: Выполняет действия над сущностью или над группой сущностей.
layout:
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: false
---

# Действие над сущностью

<figure><img src="../../../.gitbook/assets/mossy_cobblestone.png" alt="" width="150"><figcaption><p>Блок кода</p></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `entity_action`

***

## Использование

Поставьте блок в строку и нажмите ПКМ по нему, чтобы открыть меню опций блока. Перейдите в нужную категорию и выберите действие, которое необходимо выполнить.

При выборе действия, над его блоком может появиться хранилище (по умолчанию: сундук), в котором содержатся [аргументы](../arguments/) действия.

### Селекторы

Нажатием Shift + ПКМ по блоку кода открывается меню селекторов, позволяющее выбрать цель, по отношению к которой будет воспроизведено действие.

| Селектор                                                                                             | Описание                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> **Текущая цель**        | Игроки, мобы и существа выбранные с помощью [<img src="../../../.gitbook/assets/purpur_block.png" alt="" data-size="line"> **Выбрать цель**](select.md). |
| <img src="../../../.gitbook/assets/potato.png" alt="" data-size="line"> **Сущность по умолчанию**    | Сущность, которая спровоцировала данное событие.                                                                                                         |
| <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Убийца**               | Сущность, которая убила жертву в данном событии.                                                                                                         |
| <img src="../../../.gitbook/assets/stone_sword.png" alt="" data-size="line"> **Атакующая сущность**  | Сущность, которая атаковала жертву в данном событии.                                                                                                     |
| <img src="../../../.gitbook/assets/bow.png" alt="" data-size="line"> **Стрелок**                     | Сущность, которая выстрелила в данном событии.                                                                                                           |
| <img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> **Снаряд стрелка**            | Выбирает сущность, которую запустил стрелок.                                                                                                             |
| <img src="../../../.gitbook/assets/skeleton_skull.png" alt="" data-size="line"> **Жертва**           | Сущность, которая получила урон или умерла в данном событии.                                                                                             |
| <img src="../../../.gitbook/assets/eye_of_ender.png" alt="" data-size="line"> **Случайная сущность** | Случайная сущность в мире.                                                                                                                               |
| <img src="../../../.gitbook/assets/diamond_block.png" alt="" data-size="line"> **Все мобы**          | Все мобы в мире.                                                                                                                                         |
| <img src="../../../.gitbook/assets/beacon.png" alt="" data-size="line"> **Все сущности**             | Все сущности в мире.                                                                                                                                     |
| <img src="../../../.gitbook/assets/turtle_egg.png" alt="" data-size="line"> **Последняя сущность**   | Последняя появившаяся сущность в мире.                                                                                                                   |
