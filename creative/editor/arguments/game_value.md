---
description: >-
  Автоматически определённое значение, которое зависит от текущего состояния
  игры (например, местоположение игрока).
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

# Игровое значение

<figure><img src="../../../.gitbook/assets/name_tag.png" alt="" width="150"><figcaption><p>Значение</p></figcaption></figure>

**Команда получения:** [`/gamevalue`](#user-content-fn-1)[^1]\
**Текстовый идентификатор:** `game_value`

***

## Использование

Возьмите значение в активный слот и нажмите ПКМ. В открывшемся меню перейдите в нужную категорию и выберите игровое значение.

### Каталог игровых значений

{% tabs %}
{% tab title="Статистика" %}
<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> **Числовые значения параметров цели.**

***

| Значение                                                                                                                                                                 | Описание                                                                                 | Возвращаемое значение                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> <strong>Текущее здоровье</strong><br><code>current_health</code></p>                           | Получает оставшееся количество единиц здоровья цели.                                     | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **0 (мёртв) до максимального количества здоровья (20 по умолчанию)** |
| <p><img src="../../../.gitbook/assets/golden_apple.png" alt="" data-size="line"> <strong>Максимальное здоровье</strong><br><code>max_health</code></p>                   | Получает максимальное количество единиц здоровья цели.                                   | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Максимальное количество здоровья (от 1)**                          |
| <p><img src="../../../.gitbook/assets/honey_bottle.png" alt="" data-size="line"> <strong>Дополнительное здоровье</strong><br><code>absorption_health</code></p>          | Получает количество единиц поглощательного (золотого) здоровья цели.                     | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Количество поглощательного здоровья**                              |
| <p><img src="../../../.gitbook/assets/cooked_beef.png" alt="" data-size="line"> <strong>Уровень голода</strong><br><code>food_level</code></p>                           | Получает оставшееся количество единиц еды цели.                                          | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (голод) до 20 (сытость)**                                     |
| <p><img src="../../../.gitbook/assets/beef.png" alt="" data-size="line"> <strong>Уровень насыщения</strong><br><code>food_saturation</code></p>                          | Получает количество единиц насыщения едой цели, которое зависит от видов отъеденной еды. | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 до текущего количества единиц еды игрока**                    |
| <p><img src="../../../.gitbook/assets/rotten_flesh.png" alt="" data-size="line"> <strong>Уровень истощения</strong><br><code>food_exhaustion</code></p>                  | Получает уровень истощения цели, который увеличивается от выполненных действий игрока.   | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (нет истощения) до 4 (полное истощение)**                     |
| <p><img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> <strong>Урон от атаки</strong><br><code>attack_damage</code></p>                          | Получает количество единиц урона от атак цели, которое можно изменить предметами.        | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (по умолчанию 1)**                                            |
| <p><img src="../../../.gitbook/assets/golden_sword.png" alt="" data-size="line"> <strong>Скорость атаки</strong><br><code>attack_speed</code></p>                        | Получает скорость атаки цели, которую можно изменить предметами.                         | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (чем больше - тем быстрее)**                                  |
| <p><img src="../../../.gitbook/assets/diamond_sword.png" alt="" data-size="line"> <strong>Кулдаун атаки</strong><br><code>attack_cooldown_strength</code></p>            | Получает текущий кулдаун атаки цели.                                                     | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Текущий кулдаун атаки (от 0 до 1)**                                |
| <p><img src="../../../.gitbook/assets/netherite_sword.png" alt="" data-size="line"> <strong>Кулдаун атаки в тиках</strong><br><code>attack_cooldown_ticks</code></p>     | Получает текущий кулдаун атаки цели в тиках.                                             | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Текущий кулдаун атаки в тиках**                                    |
| <p><img src="../../../.gitbook/assets/iron_chestplate.png" alt="" data-size="line"> <strong>Очки защиты</strong><br><code>armor_points</code></p>                        | Получает количество единиц брони цели, которое можно изменить предметами.                | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (брони нет) до 20 (полная полоска брони)**                    |
| <p><img src="../../../.gitbook/assets/golden_chestplate.png" alt="" data-size="line"> <strong>Твёрдость брони</strong><br><code>armor_toughness</code></p>               | Получает количество единиц твёрдости брони цели, которое можно изменить предметами.      | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (незеритовая броня имеет 12 твёрдости)**                      |
| <p><img src="../../../.gitbook/assets/diamond_helmet.png" alt="" data-size="line"> <strong>Время бессмертия</strong><br><code>invulnerability_ticks</code></p>           | Получает оставшееся количество тиков неуязвимости цели.                                  | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Если больше 0, то цель неуязвима**                                 |
| <p><img src="../../../.gitbook/assets/diamond_helmet.png" alt="" data-size="line"> <strong>Общее время бессмертия</strong><br><code>max_invulnerability_ticks</code></p> | Получает количество тиков на которое выдана неуязвимость для цели.                       | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Количество тиков неуязвимости**                                    |
| <p><img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> <strong>Уровень опыта</strong><br><code>experience_level</code></p>                | Получает количество уровней опыта цели.                                                  | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Количество уровней опыта**                                         |
| <p><img src="../../../.gitbook/assets/turtle_scute.png" alt="" data-size="line"> <strong>Прогресс опыта</strong><br><code>experience_progress</code></p>                 | Получает процентный прогресс текущего уровня опыта цели.                                 | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0% (нет прогресса) до 100% (следующий уровень)**                |
| <p><img src="../../../.gitbook/assets/blaze_powder.png" alt="" data-size="line"> <strong>Время горения</strong><br><code>fire_ticks</code></p>                           | Получает оставшееся количество тиков горения цели.                                       | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Если больше 0, то цель горит**                                     |
| <p><img src="../../../.gitbook/assets/powder_snow_bucket.png" alt="" data-size="line"> <strong>Время заморозки</strong><br><code>freeze_ticks</code></p>                 | Получает текущее время заморозки цели.                                                   | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Время заморозки в тиках**                                          |
| <p><img src="../../../.gitbook/assets/glass_bottle.png" alt="" data-size="line"> <strong>Оставшийся воздух</strong><br><code>remaining_air</code></p>                    | Получает оставшееся количество тиков воздуха цели.                                       | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **От 0 (утопает) до 300 (полная полоска воздуха)**                   |
| <p><img src="../../../.gitbook/assets/damaged_anvil.png" alt="" data-size="line"> <strong>Дистанция падения</strong><br><code>fall_distance</code></p>                   | Получает дистанцию падения цели в блоках.                                                | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Если больше 0, то цель падает**                                    |
| <p><img src="../../../.gitbook/assets/light_blue_dye.png" alt="" data-size="line"> <strong>Выбранный слот в хот-баре</strong><br><code>held_slot</code></p>              | Получает выбранный слот хот-бара цели.                                                   | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Номер выбранного слота (от 0 до 8, слева направо)**                |
| <p><img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> <strong>Скорость ходьбы</strong><br><code>walking_speed</code></p>                        | Получает текущую скорость ходьбы цели (атрибут).                                         | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Скорость ходьбы цели**                                             |
| <p><img src="../../../.gitbook/assets/elytra.png" alt="" data-size="line"> <strong>Скорость полёта</strong><br><code>flying_speed</code></p>                             | Получает текущую скорость полёта цели (атрибут).                                         | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](number.md) **Скорость полёта цели**                                             |
{% endtab %}
{% endtabs %}

### Селекторы

Нажатием Shift + ЛКМ/ПКМ откроется меню селекторов, в котором можно выбрать цель игрового значения.

| Селектор                                                                                           | Описание                                                                                                                                         |
| -------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| <img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> **Текущая цель**      | Цель, выбранная с помощью [<img src="../../../.gitbook/assets/purpur_block.png" alt="" data-size="line"> **Выбрать цель**](../blocks/select.md). |
| <img src="../../../.gitbook/assets/potato.png" alt="" data-size="line"> **По умолчанию**           | Цель, которая была выбрана по умолчанию.                                                                                                         |
| <img src="../../../.gitbook/assets/carrot.png" alt="" data-size="line"> **Существо по умолчанию**  | Существо, которое было выбрано по умолчанию.                                                                                                     |
| <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Убийца**             | Цель, которая убила жертву.                                                                                                                      |
| <img src="../../../.gitbook/assets/stone_sword.png" alt="" data-size="line"> **Атакующий**         | Цель, которая атаковала жертву.                                                                                                                  |
| <img src="../../../.gitbook/assets/skeleton_skull.png" alt="" data-size="line"> **Жертва**         | Цель, которая получила урон или умерла.                                                                                                          |
| <img src="../../../.gitbook/assets/bow.png" alt="" data-size="line"> **Стрелок**                   | Цель, которая выстрелила.                                                                                                                        |
| <img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> **Снаряд**                  | Сущность, которая была запущена стрелком.                                                                                                        |
| <img src="../../../.gitbook/assets/turtle_egg.png" alt="" data-size="line"> **Последняя сущность** | Сущность, которая появилась в мире последней.                                                                                                    |

[^1]: Можно заменить на: `/gv`
