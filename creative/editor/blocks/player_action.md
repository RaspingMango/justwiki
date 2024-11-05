---
description: Выполняет действия над игроком или над группой игроков.
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

# Действие над игроком

<figure><img src="../../../.gitbook/assets/cobblestone.png" alt="" width="150"><figcaption><p>Блок кода</p></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `player_action`

***

## Использование

Поставьте блок в строку и нажмите ПКМ по нему, чтобы открыть меню опций блока. Перейдите в нужную категорию и выберите действие, которое необходимо выполнить.

При выборе действия, над его блоком может появиться хранилище, в котором содержатся аргументы действия (маркеры и значения).

### Опции

{% tabs %}
{% tab title="Управление инвентарём" %}
<img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> **Выдача, удаление, установка и сохранение предметов.**

***

| Опция                                                                                                                                                              | Описание                                                                              | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             | Доп. сведения                                                                                    |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------ |
| <p><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Выдать предмет</strong><br><code>player_give_items</code></p>                    | Выдаёт игроку предметы из сундука.                                                    | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для выдачи</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество предметов для выдачи</strong></p>                                                                                                                                                                                                                                                       |                                                                                                  |
| <p><img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> <strong>Установить предметы</strong><br><code>player_set_items</code></p>          | Устанавливает в инвентарь игрока соответственно предметы из сундука.                  | [<img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line">](../arguments/item.md) **Предметы для выдачи в соответствующие слоты**                                                                                                                                                                                                                                                                                                                                                                                                                                   |                                                                                                  |
| <p><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> <strong>Установить предмет в слот</strong><br><code>player_set_slot_item</code></p> | Устанавливает предмет в слот в инвентаре игрока.                                      | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для выдачи</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Слот для выдачи</strong></p>                                                                                                                                                                                                                                                                        |                                                                                                  |
| <p><img src="../../../.gitbook/assets/shield.png" alt="" data-size="line"> <strong>Установить экипировку</strong><br><code>player_set_equipment</code></p>         | Устанавливает предметы в один из слотов экипировки (броня и предметы в руках) игрока. | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для выдачи</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Слот снаряжения</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p>                                                                                                                                                                               |                                                                                                  |
| <p><img src="../../../.gitbook/assets/iron_leggings.png" alt="" data-size="line"> <strong>Установить броню</strong><br><code>player_set_armor</code></p>           | Устанавливает броню игрока.                                                           | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Головной убор</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Нагрудник</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Штаны</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Ботинки</strong></p> | » Любой предмет или блок будет отображаться на голове, если положить его в слот головного убора. |
{% endtab %}
{% endtabs %}

### Селекторы

Нажатием Shift + ПКМ по блоку кода открывается меню селекторов, позволяющее выбрать цель, по отношению к которой будет воспроизведено действие.

| Селектор                                                                                          | Описание                                                                                                                                                 |
| ------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> **Текущая цель**     | Игроки, мобы и существа выбранные с помощью [<img src="../../../.gitbook/assets/purpur_block.png" alt="" data-size="line"> **Выбрать цель**](select.md). |
| <img src="../../../.gitbook/assets/potato.png" alt="" data-size="line"> **Игрок по умолчанию**    | Игрок, который спровоцировал данное событие.                                                                                                             |
| <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Убийца**            | Игрок, который убил жертву в данном событии.                                                                                                             |
| <img src="../../../.gitbook/assets/stone_sword.png" alt="" data-size="line"> **Атакующий**        | Игрок, который атаковал жертву в данном событии.                                                                                                         |
| <img src="../../../.gitbook/assets/bow.png" alt="" data-size="line"> **Стрелок**                  | Игрок, который выстрелил в данном событии.                                                                                                               |
| <img src="../../../.gitbook/assets/skeleton_skull.png" alt="" data-size="line"> **Жертва**        | Игрок, который получил урон или убит в данном событии.                                                                                                   |
| <img src="../../../.gitbook/assets/eye_of_ender.png" alt="" data-size="line"> **Случайный игрок** | Случайный игрок в мире.                                                                                                                                  |
| <img src="../../../.gitbook/assets/beacon.png" alt="" data-size="line"> **Все игроки**            | Все игроки в мире.                                                                                                                                       |

[^1]: * Основная рука
    * Второстепенная рука
    * Ботинки
    * Поножи
    * Нагрудник
    * Шлем
