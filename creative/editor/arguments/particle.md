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

<table><thead><tr><th width="207">Частица</th><th>Описание</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/splash_water_bottle.png" alt="" data-size="line"> <strong>Дождь</strong><br><code>rain</code></td><td>Частицы дождя.</td></tr><tr><td><img src="../../../.gitbook/assets/prismarine_crystals.png" alt="" data-size="line"> <strong>Подводная пыль</strong><br><code>underwater</code></td><td>Частицы подводной пыли.</td></tr><tr><td><img src="../../../.gitbook/assets/gunpowder.png" alt="" data-size="line"> <strong>Пепел</strong><br><code>ash</code></td><td>Частицы пепла из Незера.</td></tr><tr><td><img src="../../../.gitbook/assets/sugar.png" alt="" data-size="line"> <strong>Белый пепел</strong><br><code>white_ash</code></td><td>Частицы белого пепла из Незера.</td></tr><tr><td><img src="../../../.gitbook/assets/crimson_roots.png" alt="" data-size="line"> <strong>Багровые споры</strong><br><code>crimson_spore</code></td><td>Частицы багровых спор из багрового леса.</td></tr><tr><td><img src="../../../.gitbook/assets/warped_roots.png" alt="" data-size="line"> <strong>Искажённые споры</strong><br><code>warped_spore</code></td><td>Частицы искажённых спор из искажённого леса.</td></tr><tr><td><img src="../../../.gitbook/assets/fermented_spider_eye.png" alt="" data-size="line"> <strong>Дурной знак</strong><br><code>raid_omen</code></td><td>Частицы дурного знака.</td></tr><tr><td><img src="../../../.gitbook/assets/ominous_bottle.png" alt="" data-size="line"> <strong>Испытание</strong><br><code>trial_omen</code></td><td>Частицы испытания.</td></tr><tr><td><img src="../../../.gitbook/assets/light_blue_dye.png" alt="" data-size="line"> <strong>Призыв зловещего испытания</strong><br><code>ominous_spawning</code></td><td>Частицы призыва зловещего испытания.</td></tr><tr><td><img src="../../../.gitbook/assets/cobweb.png" alt="" data-size="line"> <strong>Паутина</strong><br><code>item_cobweb</code></td><td>Частицы паутины.</td></tr></tbody></table>
{% endtab %}

{% tab title="Частицы существ" %}
<img src="../../../.gitbook/assets/zombie_spawn_egg.png" alt="" data-size="line"> **Различные частицы существ.**

***

| Частица                                                                                                                                                                     | Описание                                | Дополнительные поля                                           |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------- | ------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/string.png" alt="" data-size="line"> <strong>Дымок от смерти</strong><br><code>poof</code></p>                                        | Частицы дымка, возникающего при смерти. | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/gunpowder.png" alt="" data-size="line"> <strong>Взрыв</strong><br><code>explosion</code></p>                                          | Частицы взрыва.                         |                                                               |
| <p><img src="../../../.gitbook/assets/tnt_minecart.png" alt="" data-size="line"> <strong>Большой взрыв</strong><br><code>explosion_emitter</code></p>                       | Частицы большого взрыва.                |                                                               |
| <p><img src="../../../.gitbook/assets/firework_rocket.png" alt="" data-size="line"> <strong>След фейерверка</strong><br><code>firework</code></p>                           | Частицы следа от фейерверка.            | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> <strong>Капли воды</strong><br><code>splash</code></p>                                     | Частицы капель воды.                    | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/tropical_fish_bucket.png" alt="" data-size="line"> <strong>Рыба плывёт к крючку</strong><br><code>fishing</code></p>                  | Частицы подплывания рыбы к крючку.      | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/iron_axe.png" alt="" data-size="line"> <strong>Критический удар</strong><br><code>crit</code></p>                                     | Частицы от критического удара.          | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/diamond_axe.png" alt="" data-size="line"> <strong>Магический удар</strong><br><code>enchanted_hit</code></p>                          | Частицы магического удара.              | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/potion_of_invisibility.png" alt="" data-size="line"> <strong>Зелье</strong><br><code>effect</code></p>                                | Частицы зелья.                          |                                                               |
| <p><img src="../../../.gitbook/assets/splash_potion_of_invisibility.png" alt="" data-size="line"> <strong>Моментальное зелье</strong><br><code>instant_effect</code></p>    | Частицы моментального зелья.            |                                                               |
| <p><img src="../../../.gitbook/assets/potion.png" alt="" data-size="line"> <strong>Цветное зелье</strong><br><code>entity_effect</code></p>                                 | Частицы цветного зелья.                 | **Цвет**                                                      |
| <p><img src="../../../.gitbook/assets/particle_witch.png" alt="" data-size="line"> <strong>Ведьма</strong><br><code>witch</code></p>                                        | Частицы ведьмы.                         |                                                               |
| <p><img src="../../../.gitbook/assets/shroomlight.png" alt="" data-size="line"> <strong>Житель злится</strong><br><code>angry_villager</code></p>                           | Частицы злого жителя.                   |                                                               |
| <p><img src="../../../.gitbook/assets/emerald.png" alt="" data-size="line"> <strong>Житель радуется</strong><br><code>happy_villager</code></p>                             | Частицы счастливого жителя.             |                                                               |
| <p><img src="../../../.gitbook/assets/light_gray_dye.png" alt="" data-size="line"> <strong>Облако</strong><br><code>cloud</code></p>                                        | Частицы облака.                         | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/snowball.png" alt="" data-size="line"> <strong>Снежок</strong><br><code>snowball</code></p>                                           | Частицы разбивающегося снежка.          |                                                               |
| <p><img src="../../../.gitbook/assets/powder_snow_bucket.png" alt="" data-size="line"> <strong>Снежинка</strong><br><code>snowflake</code></p>                              | Частица рыхлого снега.                  | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Слизь</strong><br><code>slime</code></p>                                             | Частицы слизи.                          |                                                               |
| <p><img src="../../../.gitbook/assets/red_glazed_terracotta.png" alt="" data-size="line"> <strong>Сердце</strong><br><code>heart</code></p>                                 | Частицы сердец.                         |                                                               |
| <p><img src="../../../.gitbook/assets/cookie.png" alt="" data-size="line"> <strong>Разрушение предмета</strong><br><code>item</code></p>                                    | Частицы разрушения предмета.            | <p><strong>Движение</strong><br><strong>Материал</strong></p> |
| <p><img src="../../../.gitbook/assets/elder_guardian_spawn_egg.png" alt="" data-size="line"> <strong>Утомление</strong><br><code>elder_guardian</code></p>                  | Частицы утомления (на экране).          |                                                               |
| <p><img src="../../../.gitbook/assets/dragon_head.png" alt="" data-size="line"> <strong>Дыхание дракона</strong><br><code>dragon_breath</code></p>                          | Частицы дыхания дракона.                | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/fermented_spider_eye.png" alt="" data-size="line"> <strong>Индикатор урона</strong><br><code>damage_indicator</code></p>              | Частицы индикатора урона.               | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> <strong>Взмах удара</strong><br><code>sweep_attack</code></p>                                | Частицы взмаха от удара.                | **Размер**                                                    |
| <p><img src="../../../.gitbook/assets/totem_of_undying.png" alt="" data-size="line"> <strong>Тотем бессмертия</strong><br><code>totem_of_undying</code></p>                 | Частицы тотема бессмертия (на экране).  | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/llama_spawn_egg.png" alt="" data-size="line"> <strong>Плевок</strong><br><code>spit</code></p>                                        | Частицы плевка.                         | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/ink_sac.png" alt="" data-size="line"> <strong>Чернила спрута</strong><br><code>squid_ink</code></p>                                   | Частицы чернил спрута.                  | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/glow_ink_sac.png" alt="" data-size="line"> <strong>Чернила светящегося спрута</strong><br><code>glow_squid_ink</code></p>             | Частицы чернил светящегося спрута.      | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/glowstone_dust.png" alt="" data-size="line"> <strong>Свечение спрута</strong><br><code>glow</code></p>                                | Частица светящегося спрута.             |                                                               |
| <p><img src="../../../.gitbook/assets/tube_coral_block.png" alt="" data-size="line"> <strong>Пузырьки</strong><br><code>bubble</code></p>                                   | Частицы пузырьков.                      |                                                               |
| <p><img src="../../../.gitbook/assets/dead_tube_coral_block.png" alt="" data-size="line"> <strong>Лопание пузырьков воздуха</strong><br><code>bubble_pop</code></p>         | Частицы лопания пузырьков воздуха.      | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/dolphin_spawn_egg.png" alt="" data-size="line"> <strong>Дельфин</strong><br><code>dolphin</code></p>                                  | Частица всплеска воды от дельфина.      |                                                               |
| <p><img src="../../../.gitbook/assets/panda_spawn_eggg.png" alt="" data-size="line"> <strong>Чих</strong><br><code>sneeze</code></p>                                        | Частицы чиха.                           | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/white_stained_glass.png" alt="" data-size="line"> <strong>Вспышка</strong><br><code>flash</code></p>                                  | Частицы вспышки от фейерверка.          |                                                               |
| <p><img src="../../../.gitbook/assets/bee_spawn_egg.png" alt="" data-size="line"> <strong>Падающий мёд</strong><br><code>falling_honey</code></p>                           | Частицы падающего мёда.                 |                                                               |
| <p><img src="../../../.gitbook/assets/echo_shard.png" alt="" data-size="line"> <strong>Ударная волна</strong><br><code>sonic_boom</code></p>                                | Частицы дальней атаки Надзирателя.      |                                                               |
| <p><img src="../../../.gitbook/assets/sculk_vein.gif" alt="" data-size="line"> <strong>Скалковые души</strong><br><code>sculk_soul</code></p>                               | Частицы души скалк-катализатора.        | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/sculk_sensor.gif" alt="" data-size="line"> <strong>Скалковое заражение</strong><br><code>sculk_charge</code></p>                      | Частицы заражения скалк-катализатором.  | <p><strong>Движение</strong><br><strong>Размер</strong></p>   |
| <p><img src="../../../.gitbook/assets/sculk_catalyst.png" alt="" data-size="line"> <strong>Скалковые пузырьки</strong><br><code>sculk_charge_pop</code></p>                 | Частицы пузырей скалк-катализатора.     | **Движение**                                                  |
| <p><img src="../../../.gitbook/assets/sculk_shrieker.gif" alt="" data-size="line"> <strong>Визг</strong><br><code>shriek</code></p>                                         | Частицы скалк-крикуна.                  | **Размер**                                                    |
| <p><img src="../../../.gitbook/assets/wind_charge.png" alt="" data-size="line"> <strong>Заряд ветра</strong><br><code>gust</code></p>                                       | Частицы заряда ветра.                   |                                                               |
| <p><img src="../../../.gitbook/assets/white_glazed_terracotta.png" alt="" data-size="line"> <strong>Маленький выстрел вихря</strong><br><code>gust_emitter_small</code></p> | Частицы маленького выстрела вихря.      |                                                               |
| <p><img src="../../../.gitbook/assets/light_gray_dye.png" alt="" data-size="line"> <strong>Большой выстрел вихря</strong><br><code>gust_emitter_large</code></p>            | Частицы большого выстрела вихря.        |                                                               |
| <p><img src="../../../.gitbook/assets/iron_nugget.png" alt="" data-size="line"> <strong>Маленький заряд ветра</strong><br><code>small_gust</code></p>                       | Частицы маленького заряда ветра.        |                                                               |
| <p><img src="../../../.gitbook/assets/dead_tube_coral_block.png" alt="" data-size="line"> <strong>Заражение</strong><br><code>infested</code></p>                           | Частицы заражения камня чешуйницей.     |                                                               |
{% endtab %}
{% endtabs %}

[^1]: Можно заменить на: `/part`

[^2]: Количество отображаемых частиц.

[^3]: Разброс по ширине.

[^4]: Разброс по высоте.
