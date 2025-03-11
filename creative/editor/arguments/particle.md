---
description: Используется для указания аргументов типа частица.
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

# Эффект частиц

<figure><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" width="150"><figcaption></figcaption></figure>

**Команда получения:** [`/particle`](#user-content-fn-1)[^1]\
**Ячейка:** <img src="../../../.gitbook/assets/pink_stained_glass_pane.png" alt="" data-size="line">\
**Текстовый идентификатор:** `particle`

***

## Использование

Возьмите значение в активный слот и нажмите <kbd>ПКМ</kbd>. В открывшемся меню перейдите в нужную категорию и выберите частицу.

Можно изменить параметры частицы, введя их в чат: [`amount`](#user-content-fn-2)[^2] [`spread_xz`](#user-content-fn-3)[^3] [`spread_y`](#user-content-fn-4)[^4].

Нажатие <kbd>ЛКМ</kbd> призовёт эффект частиц перед вами.

### Каталог частиц

{% tabs %}
{% tab title="Частицы окружения" %}
<img src="../../../.gitbook/assets/warped_fungus.png" alt="" data-size="line"> **Различные частицы окружения.**

***

| Частица                                                                                                                                                             | Описание                                     |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------- |
| <p><img src="../../../.gitbook/assets/splash_water_bottle.png" alt="" data-size="line"> <strong>Дождь</strong><br><code>rain</code></p>                             | Частицы дождя.                               |
| <p><img src="../../../.gitbook/assets/prismarine_crystals.png" alt="" data-size="line"> <strong>Подводная пыль</strong><br><code>underwater</code></p>              | Частицы подводной пыли.                      |
| <p><img src="../../../.gitbook/assets/gunpowder.png" alt="" data-size="line"> <strong>Пепел</strong><br><code>ash</code></p>                                        | Частицы пепла из Незера.                     |
| <p><img src="../../../.gitbook/assets/sugar.png" alt="" data-size="line"> <strong>Белый пепел</strong><br><code>white_ash</code></p>                                | Частицы белого пепла из Незера.              |
| <p><img src="../../../.gitbook/assets/crimson_roots.png" alt="" data-size="line"> <strong>Багровые споры</strong><br><code>crimson_spore</code></p>                 | Частицы багровых спор из багрового леса.     |
| <p><img src="../../../.gitbook/assets/warped_roots.png" alt="" data-size="line"> <strong>Искажённые споры</strong><br><code>warped_spore</code></p>                 | Частицы искажённых спор из искажённого леса. |
| <p><img src="../../../.gitbook/assets/fermented_spider_eye.png" alt="" data-size="line"> <strong>Дурной знак</strong><br><code>raid_omen</code></p>                 | Частицы дурного знака.                       |
| <p><img src="../../../.gitbook/assets/ominous_bottle.png" alt="" data-size="line"> <strong>Испытание</strong><br><code>trial_omen</code></p>                        | Частицы испытания.                           |
| <p><img src="../../../.gitbook/assets/light_blue_dye.png" alt="" data-size="line"> <strong>Призыв зловещего испытания</strong><br><code>ominous_spawning</code></p> | Частицы призыва зловещего испытания.         |
| <p><img src="../../../.gitbook/assets/cobweb.png" alt="" data-size="line"> <strong>Паутина</strong><br><code>item_cobweb</code></p>                                 | Частицы паутины.                             |
{% endtab %}

{% tab title="Частицы существ" %}
<img src="../../../.gitbook/assets/zombie_spawn_egg.png" alt="" data-size="line"> **Различные частицы существ.**

***

| Частица                                                                                                                                                                  | Описание                                | Дополнительные поля |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | --------------------------------------- | ------------------- |
| <p><img src="../../../.gitbook/assets/string.png" alt="" data-size="line"> <strong>Дымок от смерти</strong><br><code>poof</code></p>                                     | Частицы дымка, возникающего при смерти. | **Движение**        |
| <p><img src="../../../.gitbook/assets/gunpowder.png" alt="" data-size="line"> <strong>Взрыв</strong><br><code>explosion</code></p>                                       | Частицы взрыва.                         |                     |
| <p><img src="../../../.gitbook/assets/tnt_minecart.png" alt="" data-size="line"> <strong>Большой взрыв</strong><br><code>explosion_emitter</code></p>                    | Частицы большого взрыва.                |                     |
| <p><img src="../../../.gitbook/assets/firework_rocket.png" alt="" data-size="line"> <strong>След фейерверка</strong><br><code>firework</code></p>                        | Частицы следа от фейерверка.            | **Движение**        |
| <p><img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> <strong>Капли воды</strong><br><code>splash</code></p>                                  | Частицы капель воды.                    | **Движение**        |
| <p><img src="../../../.gitbook/assets/tropical_fish_bucket.png" alt="" data-size="line"> <strong>Рыба плывёт к крючку</strong><br><code>fishing</code></p>               | Частицы подплывания рыбы к крючку.      | **Движение**        |
| <p><img src="../../../.gitbook/assets/iron_axe.png" alt="" data-size="line"> <strong>Критический удар</strong><br><code>crit</code></p>                                  | Частицы от критического удара.          | **Движение**        |
| <p><img src="../../../.gitbook/assets/diamond_axe.png" alt="" data-size="line"> <strong>Магический удар</strong><br><code>enchanted_hit</code></p>                       | Частицы магического удара.              | **Движение**        |
| <p><img src="../../../.gitbook/assets/potion_of_invisibility.png" alt="" data-size="line"> <strong>Зелье</strong><br><code>effect</code></p>                             | Частицы зелья.                          |                     |
| <p><img src="../../../.gitbook/assets/splash_potion_of_invisibility.png" alt="" data-size="line"> <strong>Моментальное зелье</strong><br><code>instant_effect</code></p> | Частицы моментального зелья.            |                     |
| <p><img src="../../../.gitbook/assets/potion.png" alt="" data-size="line"> <strong>Цветное зелье</strong><br><code>entity_effect</code></p>                              | Частицы цветного зелья.                 | **Цвет**            |
{% endtab %}
{% endtabs %}

[^1]: Можно заменить на: `/part`

[^2]: Количество отображаемых частиц.

[^3]: Разброс по ширине.

[^4]: Разброс по высоте.
