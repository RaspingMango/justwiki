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

### Опции

{% tabs %}
{% tab title="Параметры" %}
<img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> **Изменение параметров существа, такие как здоровье, эффекты, горение и другое.**

***

| Опция                                                                                                                                                                                         | Описание                                                     | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| <p><img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> <strong>Исцелить существо</strong><br><code>entity_heal</code></p>                                                  | Исцеляет существо.                                           | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](../arguments/number.md) **Количество половинок сердец для излечения**                                                                                                                                                                                                                                                                      |
| <p><img src="../../../.gitbook/assets/golden_apple.png" alt="" data-size="line"> <strong>Установить здоровье существа</strong><br><code>entity_set_current_health</code></p>                  | Устанавливает здоровье существа на выбранное количество.     | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](../arguments/number.md) **Количество здоровья**                                                                                                                                                                                                                                                                                            |
| <p><img src="../../../.gitbook/assets/honey_bottle.png" alt="" data-size="line"> <strong>Установить дополнительное здоровье</strong><br><code>entity_set_absorption_health</code></p>         | Устанавливает дополнительное здоровье существа.              | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](../arguments/number.md) **Количество дополнительного здоровья**                                                                                                                                                                                                                                                                            |
| <p><img src="../../../.gitbook/assets/silverfish_spawn_egg.png" alt="" data-size="line"> <strong>Установить максимальное здоровье существа</strong><br><code>entity_set_max_health</code></p> | Устанавливает максимальное количество здоровья для существа. | <p><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Максимальное количество здоровья</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Исцелить существо</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p> |
| <p><img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> <strong>Нанести урон</strong><br><code>entity_damage</code></p>                                                | Наносит урон существу.                                       | <p><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество урона</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Источник урона (имя или UUID существа)</strong></p>                                                                                            |
| <p><img src="../../../.gitbook/assets/blaze_powder.png" alt="" data-size="line"> <strong>Поджечь существо</strong><br><code>entity_set_fire_ticks</code></p>                                  | Поджигает существо на выбранное время.                       | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](../arguments/number.md) **Длительность (в тиках)**                                                                                                                                                                                                                                                                                         |
{% endtab %}
{% endtabs %}

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

[^1]: * Да
    * Нет
