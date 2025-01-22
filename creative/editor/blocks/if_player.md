---
description: >-
  Выполняет код внутри поршней, если игрок соблюдает условие, указанное на
  табличке.
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

# Если игрок

<figure><img src="../../../.gitbook/assets/oak_planks.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Условие\
**Текстовый идентификатор:** `if_player`

***

## Использование

Поставьте блок в строку и нажмите <kbd>ПКМ</kbd> по нему, чтобы открыть меню опций блока. Перейдите в нужную категорию и выберите условие, которое необходимо поставить.

Внутри поршней выполняется код, который подчиняется поставленному условию. Код, расположенный после поршней, не будет подчиняться условию.

При выборе условия, над его блоком может появиться хранилище (по умолчанию: сундук), в котором содержатся [аргументы](../arguments/) условия.

Условие можно заменить на обратное (инвертировать). Для этого нужно взять предмет <img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> **НЕ стрела** в активный слот и нажать <kbd>ПКМ</kbd> по табличке на блоке условия.

### Опции

{% tabs %}
{% tab title="Бинарные условия" %}
<img src="../../../.gitbook/assets/redstone.png" alt="" data-size="line"> **Если крадётся, если плавает, если бежит и т.д.**

***

| Опция                                                                                                                                                                                         | Описание                                                            |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/chainmail_leggings.png" alt="" data-size="line"> <strong>Крадётся</strong><br><code>if_player_is_sneaking</code></p>                                    | Проверяет, крадётся ли игрок.                                       |
| <p><img src="../../../.gitbook/assets/golden_boots.png" alt="" data-size="line"> <strong>Бежит</strong><br><code>if_player_is_sprinting</code></p>                                            | Проверяет, бежит ли игрок или использует клавишу бега при плавании. |
| <p><img src="../../../.gitbook/assets/elytra.png" alt="" data-size="line"> <strong>Парит</strong><br><code>if_player_is_gliding</code></p>                                                    | Проверяет, парит ли игрок на элитрах.                               |
| <p><img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> <strong>Летит</strong><br><code>if_player_is_flying</code></p>                                                    | Проверяет, летит ли игрок.                                          |
| <p><img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> <strong>Плавает</strong><br><code>if_player_is_swimming</code></p>                                           | Проверяет, плавает ли игрок в воде или лаве.                        |
| <p><img src="../../../.gitbook/assets/grass_block.png" alt="" data-size="line"> <strong>Стоит на земле</strong><br><code>if_player_is_on_ground</code></p>                                    | Проверяет, не находится ли игрок в воздухе.                         |
| <p><img src="../../../.gitbook/assets/shield.png" alt="" data-size="line"> <strong>Использует щит</strong><br><code>if_player_is_blocking</code></p>                                          | Проверяет, использует ли игрок щит.                                 |
| <p><img src="../../../.gitbook/assets/red_bed.png" alt="" data-size="line"> <strong>Спит</strong><br><code>if_player_is_sleeping</code></p>                                                   | Проверяет, спит ли игрок.                                           |
| <p><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Замаскирован для всех</strong><br><code>if_player_is_disguised</code></p>                             | Проверяет, замаскирован ли игрок для остальных игроков.             |
| <p><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Замаскирован для себя</strong><br><code>if_player_is_self_disguised</code></p>                        | Проверяет, замаскирован ли игрок для себя.                          |
| <p><img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> <strong>Имеет лицензионный аккаунт</strong><br><code>if_player_is_online_mode</code></p>                      | Проверяет, имеет ли игрок лицензионный аккаунт.                     |
| <p><img src="../../../.gitbook/assets/tinted_glass.png" alt="" data-size="line"> <strong>Отображается в списке игроков сервера</strong><br><code>if_player_is_allow_server_listing</code></p> | Проверяет, включена ли настройка "Показывать в списках" у игрока.   |
| <p><img src="../../../.gitbook/assets/yellow_dye.png" alt="" data-size="line"> <strong>Имеет цвета в чате</strong><br><code>if_player_chat_colors_enabled</code></p>                          | Проверяет, включена ли настройка "Цвета в чате" у игрока.           |
| <p><img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> <strong>Имеет фильтр слов</strong><br><code>if_player_text_filtering_enabled</code></p>                            | Проверяет, включен ли фильтр слов от Mojang у игрока.               |
{% endtab %}

{% tab title="Условия местоположения" %}
<img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"> **Если рядом, если стоит на блоке, если смотрит на блок и т.д.**

***

| Опция                                                                                                                                                                                   | Описание                                                                                                    | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/iron_ore.png" alt="" data-size="line"> <strong>Смотрит на блок</strong><br><code>if_player_is_looking_at_block</code></p>                         | Проверяет, смотрит ли игрок на определённый блок или местоположение.                                        | <p><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок(и) для проверки</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение(я) для проверки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Максимальное расстояние до проверяемого блока</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим жидкости</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                         |
| <p><img src="../../../.gitbook/assets/heavy_weighted_pressure_plate.png" alt="" data-size="line"> <strong>Стоит на блоке</strong><br><code>if_player_is_standing_on_block</code></p>    | Проверяет, стоит ли игрок на блоке определённом блоке или местоположении.                                   | <p><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блоки для проверки</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Учитывать проходимые блоки</strong> <a data-footnote-ref href="#user-content-fn-2"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| <p><img src="../../../.gitbook/assets/compass.png" alt="" data-size="line"> <strong>Рядом с местоположением</strong><br><code>if_player_is_near</code></p>                              | Проверяет, находится ли игрок рядом с указанным местоположением (По умолчанию: 5 блоков).                   | <p><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Игнорировать ось Y</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение для проверки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Радиус проверки</strong></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <p><img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> <strong>Внутри региона</strong><br><code>if_player_in_area</code></p>                                | Проверяет, находится ли игрок в определённом регионе.                                                       | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Первый угол региона</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Второй угол региона</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Игнорировать ось Y</strong> <a data-footnote-ref href="#user-content-fn-4"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип пересечения</strong> <a data-footnote-ref href="#user-content-fn-5"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип проверки хитбокса</strong> <a data-footnote-ref href="#user-content-fn-6"><strong><code>-></code></strong></a></p> |
| <p><img src="../../../.gitbook/assets/empty_map.png" alt="" data-size="line"> <strong>Сталкивается на местоположении</strong><br><code>if_player_collides_at_location</code></p>        | Проверяет, сталкивается ли игрок с блоками, шалкерами, лодками и границей мира на указанном местоположении. | [<img src="../../../.gitbook/assets/paper.png" alt="" data-size="line">](../arguments/location.md) **Местоположение для проверки**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| <p><img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> <strong>Сталкивается используя кастомный хитбокс</strong><br><code>if_player_collides_using_hitbox</code></p> | Проверяет, сталкивается ли игрок с блоками, шалкерами, лодками и границей мира используя кастомный хитбокс. | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Первый угол хитбокса</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Второй угол хитбокса</strong></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| <p><img src="../../../.gitbook/assets/glass_pane.png" alt="" data-size="line"> <strong>Сталкивается с сущностью</strong><br><code>if_player_collides_with_entity</code></p>             | Проверяет, сталкивается ли хитбокс игрока с хитбоксом указанной сущности.                                   | <p><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID сущности</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип проверки столкновения</strong> <a data-footnote-ref href="#user-content-fn-7"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
{% endtab %}

{% tab title="Предметные условия" %}
<img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> **Если имеет предмет, если держит предмет, если надет предмет и т.д.**

***

| Опция                                                                                                                                                                                  | Описание                                                                                     | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Держит предмет</strong><br><code>if_player_is_holding</code></p>                                     | Проверяет, держит ли игрок предмет в своих руках.                                            | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Рука</strong> <a data-footnote-ref href="#user-content-fn-8"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-9"><strong><code>-></code></strong></a></p>                             |
| <p><img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> <strong>Имеет предмет</strong><br><code>if_player_has_item</code></p>                                  | Проверяет, имеет ли игрок предмет в своём инвентаре.                                         | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим проверки</strong> <a data-footnote-ref href="#user-content-fn-10"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-11"><strong><code>-></code></strong></a></p>                 |
| <p><img src="../../../.gitbook/assets/hopper_minecart.png" alt="" data-size="line"> <strong>Имеет предмет в количестве</strong><br><code>if_player_has_item_at_least</code></p>        | Проверяет, имеет ли игрок предмет в определённом количестве.                                 | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для проверки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Минимальное количество</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-12"><strong><code>-></code></strong></a></p>                                                                                                   |
| <p><img src="../../../.gitbook/assets/iron_chestplate.png" alt="" data-size="line"> <strong>Одет в предмет</strong><br><code>if_player_is_wearing_item</code></p>                      | Проверяет, одет ли игрок в предмет.                                                          | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим проверки</strong> <a data-footnote-ref href="#user-content-fn-13"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-14"><strong><code>-></code></strong></a></p>                  |
| <p><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Предмет не имеет задержку</strong><br><code>if_player_item_is_not_on_cooldown</code></p>             | Проверяет, не имеет ли предмет у игрока задержку, применимую к определённому типу предметов. | [<img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line">](../arguments/item.md) **Предметы для проверки**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <p><img src="../../../.gitbook/assets/cyan_shulker_box.png" alt="" data-size="line"> <strong>Имеет предмет в слоте</strong><br><code>if_player_has_item_in_slot</code></p>             | Проверяет, имеет ли игрок предмет в определённом слоте инвентаря.                            | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Номер слота для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-15"><strong><code>-></code></strong></a></p>                                                                                                |
| <p><img src="../../../.gitbook/assets/chest_minecart.png" alt="" data-size="line"> <strong>Слот в инвентаре содержит</strong><br><code>if_player_inventory_menu_slot_equals</code></p> | Проверяет, содержит ли сейчас игрок с открытым инвентарём определённый предмет в слоте.      | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Номер слота для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-16"><strong><code>-></code></strong></a></p>                                                                                                |
| <p><img src="../../../.gitbook/assets/fishing_rod.png" alt="" data-size="line"> <strong>Предмет на курсоре равен</strong><br><code>if_player_cursor_item_equals</code></p>             | Проверяет, равен ли предмет, находящийся на курсоре игрока, выбранному предмету.             | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-17"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                              |
| <p><img src="../../../.gitbook/assets/flower_pot.png" alt="" data-size="line"> <strong>Имеет место для предметов</strong><br><code>if_player_has_room_for_item</code></p>              | Проверяет, имеет ли игрок в своём инвентаре место для одного или нескольких предметов.       | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим проверки предметов</strong><a data-footnote-ref href="#user-content-fn-18"> <strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим проверки слотов</strong> <a data-footnote-ref href="#user-content-fn-19"><strong><code>-></code></strong></a></p> |
{% endtab %}

{% tab title="Прочие условия" %}
<img src="../../../.gitbook/assets/bedrock.png" alt="" data-size="line"> **Если имя равно, если имеет эффект и т.д.**

***

| Опция                                                                                                                                                                    | Описание                                                                                                                                                                                                                     | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Имя равно</strong><br><code>if_player_name_equals</code></p>                        | Проверяет, равно ли имя игрока имени в сундуке.                                                                                                                                                                              | [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line">](../arguments/text.md) **Имена или UUID для проверки**                                                                                                                                                                                                                                                                                                                                                           |
| <p><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> <strong>Слот в хот-баре равен</strong><br><code>if_player_hotbar_slot_equals</code></p>   | Проверяет, совпадает ли текущий слот хот-бара игрока со слотом от 1 до 9 в сундуке.                                                                                                                                          | [<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line">](../arguments/number.md) **Номер слота для проверки**                                                                                                                                                                                                                                                                                                                                                      |
| <p><img src="../../../.gitbook/assets/brewing_stand.png" alt="" data-size="line"> <strong>Имеет эффект от зелья</strong><br><code>if_player_has_potion_effect</code></p> | Проверяет, имеет ли игрок эффект от зелья.                                                                                                                                                                                   | <p><a href="../arguments/potion.md"><img src="../../../.gitbook/assets/dragon_breath.png" alt="" data-size="line"></a> <strong>Зелья для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим проверки</strong> <a data-footnote-ref href="#user-content-fn-20"><strong><code>-></code></strong></a></p>                                                                             |
| <p><img src="../../../.gitbook/assets/saddle.png" alt="" data-size="line"> <strong>Оседлал существо</strong><br><code>if_player_is_riding_entity</code></p>              | Проверяет, оседлал ли игрок существо (включая транспорт).                                                                                                                                                                    | <p><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя, UUID или тип существа для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-21"><strong><code>-></code></strong></a></p>                                                                  |
| <p><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Открыт инвентарь типа</strong><br><code>if_player_inventory_type_open</code></p>    | Проверяет, открыт ли инвентарь определённого типа у игрока.                                                                                                                                                                  | [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Тип инвентаря** [**`->`**](#user-content-fn-22)[^22]                                                                                                                                                                                                                                                                                                                        |
| <p><img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> <strong>Режим игры равен</strong><br><code>if_player_gamemode_equals</code></p>       | Проверяет, равен ли режим игры игрока выбранному.                                                                                                                                                                            | [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Режим игры** [**`->`**](#user-content-fn-23)[^23]                                                                                                                                                                                                                                                                                                                           |
| <p><img src="../../../.gitbook/assets/writable_book.png" alt="" data-size="line"> <strong>Сообщение равно</strong><br><code>if_player_chat_message_equals</code></p>     | Проверяет, равно ли сообщение игрока выбранному.                                                                                                                                                                             | [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line">](../arguments/text.md) **Сообщение**                                                                                                                                                                                                                                                                                                                                                                             |
| <p><img src="../../../.gitbook/assets/beacon.png" alt="" data-size="line"> <strong>Имеет права</strong><br><code>if_player_has_privilege</code></p>                      | <p>Проверяет, имеет ли игрок определённые права в мире.<br><br>» При включённом маркере "Точность проверки", проверка на права строительства и разработки будет осуществляться, даже если игрок добавлен в белый список.</p> | <p><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Право</strong> <a data-footnote-ref href="#user-content-fn-24"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Точность проверки</strong> <a data-footnote-ref href="#user-content-fn-25"><strong><code>-></code></strong></a></p> |
{% endtab %}
{% endtabs %}

### Селекторы

Нажатием <kbd>Shift</kbd> + <kbd>ПКМ</kbd> по блоку кода открывается меню селекторов, позволяющее выбрать цель, по отношению к которой будет воспроизведена проверка.

| Селектор                                                                                       | Описание                                                                                                                                                 |
| ---------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> **Текущая цель**  | Игроки, мобы и существа выбранные с помощью [<img src="../../../.gitbook/assets/purpur_block.png" alt="" data-size="line"> **Выбрать цель**](select.md). |
| <img src="../../../.gitbook/assets/potato.png" alt="" data-size="line"> **Игрок по умолчанию** | Игрок, который спровоцировал данное событие.                                                                                                             |
| <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Убийца**         | Игрок, который убил жертву в данном событии.                                                                                                             |
| <img src="../../../.gitbook/assets/stone_sword.png" alt="" data-size="line"> **Атакующий**     | Игрок, который атаковал жертву в данном событии.                                                                                                         |
| <img src="../../../.gitbook/assets/bow.png" alt="" data-size="line"> **Стрелок**               | Игрок, который выстрелил в данном событии.                                                                                                               |
| <img src="../../../.gitbook/assets/skeleton_skull.png" alt="" data-size="line"> **Жертва**     | Игрок, который получил урон или убит в данном событии.                                                                                                   |
| <img src="../../../.gitbook/assets/ender_eye.png" alt="" data-size="line"> **Случайный игрок** | Случайный игрок в мире.                                                                                                                                  |
| <img src="../../../.gitbook/assets/beacon.png" alt="" data-size="line"> **Все игроки**         | Все игроки в мире.                                                                                                                                       |

[^1]: * Игнорировать жидкости
    * Только источники жидкостей
    * Все виды жидкостей

[^2]: * Учитывать
    * Не учитывать

[^3]: * Игнорировать
    * Не игнорировать

[^4]: * Игнорировать
    * Не игнорировать

[^5]: * Местоположение
    * Хитбокс

[^6]: * Пересекается
    * Содержит

[^7]: * Пересекается
    * Содержит

[^8]: * Любая рука
    * Главная рука
    * Второстепенная рука

[^9]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^10]: * Любой предмет
    * Все предметы

[^11]: * Полное сравнение
    * Игнорировать количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^12]: * Полное сравнение
    * Только тип предмета

[^13]: * Одет во что-либо
    * Одет во всё

[^14]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^15]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^16]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^17]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^18]: * Любые предметы
    * Все предметы

[^19]: * Весь инвентарь
    * Главный инвентарь
    * Верхний инвентарь
    * Хот-бар
    * Броня

[^20]: * Любой эффект
    * Все эффекты

[^21]: * Тип существа
    * Имя или UUID

[^22]: * Сундук
    * Раздатчик
    * Выбрасыватель
    * Печь
    * Верстак
    * Не открыт
    * Чародейский стол
    * Зельеварка
    * Инвентарь игрока
    * Инвентарь креатива
    * Торговец
    * Эндер-сундук
    * Наковальня
    * Стол кузнеца (старый)
    * Маяк
    * Воронка
    * Шалкеровый ящик
    * Бочка
    * Плавильная печь
    * Кафедра
    * Коптильня
    * Ткацкий станок
    * Стол картографа
    * Точило
    * Камнерез
    * Компостер
    * Резная книжная полка
    * Нотный блок
    * Ваза
    * Сборщик
    * Стол кузнеца

[^23]: * Выживание
    * Творческий
    * Приключение
    * Наблюдатель

[^24]: * Строитель
    * Разработчик
    * Строитель и разработчик
    * В белом списке
    * Владелец мира

[^25]: * Включить
    * Выключить
