---
description: Используется для указания аргументов типа зелье.
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

# Зелье

<figure><img src="../../../.gitbook/assets/dragon_breath.png" alt=""><figcaption></figcaption></figure>

**Команда получения:** `/potion`\
**Ячейка:** <img src="../../../.gitbook/assets/magenta_stained_glass_pane.png" alt="" data-size="line">\
**Текстовый идентификатор:** `potion`

***

## Использование

Возьмите значение в активный слот и нажмите <kbd>ПКМ</kbd>. В открывшемся меню выберите нужное зелье.

Можно изменить параметры зелья, введя их в чат: [`amplifier`](#user-content-fn-1)[^1] [`duration`](#user-content-fn-2)[^2].

* Нажатие <kbd>ЛКМ</kbd> накладывает эффект зелья на вас.
* Нажатие <kbd>Shift</kbd> + <kbd>ЛКМ</kbd> снимает эффект зелья.

### Каталог зелий

{% tabs %}
{% tab title="Положительные" %}
| Зелье                                                                                                                                                                       | Описание                                                                                                            |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/code_potion_absorption.png" alt="" data-size="line"> <strong>Поглощение</strong><br><code>absorption</code></p>                       | Даёт `4 × уровень` единиц поглощения (дополнительного здоровья).                                                    |
| <p><img src="../../../.gitbook/assets/code_potion_conduit_power.png" alt="" data-size="line"> <strong>Морская сила</strong><br><code>conduit_power</code></p>               | Улучшает видимость под водой, скорость добычи и предотвращает утопление.                                            |
| <p><img src="../../../.gitbook/assets/code_potion_dolphins_grace.png" alt="" data-size="line"> <strong>Грация дельфина</strong><br><code>dolphins_grace</code></p>          | Увеличивает скорость плавания на `40%`.                                                                             |
| <p><img src="../../../.gitbook/assets/code_potion_fire_resistance.png" alt="" data-size="line"> <strong>Огнестойкость</strong><br><code>fire_resistance</code></p>          | Даёт иммунитет к огню и урону от лавы.                                                                              |
| <p><img src="../../../.gitbook/assets/code_potion_haste.png" alt="" data-size="line"> <strong>Спешка</strong><br><code>haste</code></p>                                     | Увеличивает скорость добычи на `20% × уровень` и скорость атаки на `10% × уровень`.                                 |
| <p><img src="../../../.gitbook/assets/code_potion_health_boost.png" alt="" data-size="line"> <strong>Прилив здоровья</strong><br><code>health_boost</code></p>              | Увеличивает максимальное здоровье на `4 × уровень`.                                                                 |
| <p> <img src="../../../.gitbook/assets/code_potion_hero_of_the_village.png" alt="" data-size="line"> <strong>Герой деревни</strong><br><code>hero_of_the_village</code></p> | Заставляет ближайших жителей бросать подарки и предлагать скидку на торговлю в размере `23.75 + (6.25 × уровень)%`. |
| <p><img src="../../../.gitbook/assets/code_potion_heal.png" alt="" data-size="line"> <strong>Исцеление</strong><br><code>heal</code></p>                                    | Мгновенно восполняет `2 × 2 ^ уровень` единиц здоровья.                                                             |
| <p><img src="../../../.gitbook/assets/code_potion_invisibility.png" alt="" data-size="line"> <strong>Невидимость</strong><br><code>invisibility</code></p>                  | Заставляет сущность стать невидимой.                                                                                |
| <p><img src="../../../.gitbook/assets/code_potion_jump.png" alt="" data-size="line"> <strong>Прыгучесть</strong><br><code>jump</code></p>                                   | Увеличивает высоту прыжка на `0.5 + уровень`.                                                                       |
| <p><img src="../../../.gitbook/assets/code_potion_luck.png" alt="" data-size="line"> <strong>Удача</strong><br><code>luck</code></p>                                        | Увеличивает навык рыбалки в зависимости от значения `уровень`.                                                      |
| <p><img src="../../../.gitbook/assets/code_potion_night_vision.png" alt="" data-size="line"> <strong>Ночное зрение</strong><br><code>night_vision</code></p>                | Усиливает способность игрока видеть в темноте и под водой.                                                          |
| <p><img src="../../../.gitbook/assets/code_potion_regeneration.png" alt="" data-size="line"> <strong>Регенерация</strong><br><code>regeneration</code></p>                  | Восстанавливает `1` единицу здоровья каждые `2.5 ÷ уровень` секунд.                                                 |
| <p><img src="../../../.gitbook/assets/code_potion_damage_resistance.png" alt="" data-size="line"> <strong>Сопротивление</strong><br><code>damage_resistance</code></p>      | Уменьшает количество получаемого урона на `20% × уровень`.                                                          |
| <p><img src="../../../.gitbook/assets/code_potion_saturation.png" alt="" data-size="line"> <strong>Насыщение</strong><br><code>saturation</code></p>                        | Мгновенно восполняет `1 × уровень` единиц сытости и `2 × уровень` единиц насыщения.                                 |
| <p><img src="../../../.gitbook/assets/code_potion_slow_falling.png" alt="" data-size="line"> <strong>Медленное падение</strong><br><code>slow_falling</code></p>            | Уменьшает скорость падения на `70%` и предотвращает урон от падения.                                                |
| <p><img src="../../../.gitbook/assets/code_potion_speed.png" alt="" data-size="line"> <strong>Скорость</strong><br><code>speed</code></p>                                   | Увеличивает скорость передвижения на `20% × уровень`.                                                               |
| <p><img src="../../../.gitbook/assets/code_potion_increase_damage.png" alt="" data-size="line"> <strong>Сила</strong><br><code>increase_damage</code></p>                   | Увеличивает урон от ближнего боя на `3 × уровень`.                                                                  |
| <p><img src="../../../.gitbook/assets/code_potion_water_breathing.png" alt="" data-size="line"> <strong>Подводное дыхание</strong><br><code>water_breathing</code></p>      | Предотвращает потерю единиц воздуха под водой.                                                                      |
{% endtab %}

{% tab title="Нейтральные" %}
| Зелье                                                                                                                                                        | Описание                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/code_potion_glowing.png" alt="" data-size="line"> <strong>Свечение</strong><br><code>glowing</code></p>                | Рисует обводку вокруг сущности и заставляет светиться через стены.                     |
| <p><img src="../../../.gitbook/assets/code_potion_bad_omen.png" alt="" data-size="line"> <strong>Дурное знамение</strong><br><code>bad_omen</code></p>       | Провоцирует начало рейда, если рядом два и более жителя.                               |
| <p><img src="../../../.gitbook/assets/code_potion_trial_omen.png" alt="" data-size="line"> <strong>Зловещее знамение</strong><br><code>trial_omen</code></p> | Превращает рассадники испытаний в зловещие рассадники испытаний вокруг сущности.       |
| <p><img src="../../../.gitbook/assets/code_potion_raid_omen.png" alt="" data-size="line"> <strong>Рейдерское знамение</strong><br><code>raid_omen</code></p> | Провоцирует рейд через 30 секунд после входа в деревню, если рядом два и более жителя. |
{% endtab %}

{% tab title="Негативные" %}

{% endtab %}
{% endtabs %}

[^1]: Уровень.

[^2]: Длительность (в тиках).
