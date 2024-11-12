---
description: >-
  Выполняет код внутри поршней, если в мире соблюдается условие, указанное на
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

# Если в мире

<figure><img src="../../../.gitbook/assets/red_nether_bricks.png" alt="" width="150"><figcaption><p>Блок кода</p></figcaption></figure>

**Тип:** Условие\
**Текстовый идентификатор:** `if_game`

***

## Использование

Поставьте блок в строку и нажмите ПКМ по нему, чтобы открыть меню опций блока. Затем выберите условие, которое необходимо поставить.

Внутри поршней выполняется код, который подчиняется поставленному условию. Код, расположенный после поршней, не будет подчиняться условию.

При выборе условия, над его блоком может появиться хранилище (по умолчанию: сундук), в котором содержатся [аргументы](../arguments/) условия.

Условие можно заменить на обратное (инвертировать). Для этого нужно взять предмет <img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> **НЕ стрела** в активный слот и нажать ПКМ по табличке на блоке условия.

### Опции

| Опция                                                                                                                                                                                       | Описание                                                                                           | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/bricks.png" alt="" data-size="line"> <strong>Блок равен</strong><br><code>if_game_block_equals</code></p>                                             | Проверяет, является ли блок в определённом местоположении определённым типом блока.                | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Тип блока для проверки</strong></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <p><img src="../../../.gitbook/assets/redstone_torch.png" alt="" data-size="line"> <strong>Блок запитан редстоуном</strong><br><code>if_game_block_powered</code></p>                       | Проверяет, запитан ли блок в определённом местоположении редстоуном.                               | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Вид запитывания редстоуном</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| <p><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Контейнер имеет предмет</strong><br><code>if_game_container_has</code></p>                                | Проверяет, имеет ли контейнер в определённом местоположении определённые предметы в его инвентаре. | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Вид сравнения</strong> <a data-footnote-ref href="#user-content-fn-2"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                         |
| <p><img src="../../../.gitbook/assets/flower_pot.png" alt="" data-size="line"> <strong>Контейнер имеет место для предметов</strong><br><code>if_game_container_has_room_for_item</code></p> | Проверяет, имеет ли контейнер в определённом местоположении место для предметов в его инвентаре.   | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Вид сравнения</strong> <a data-footnote-ref href="#user-content-fn-4"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| <p><img src="../../../.gitbook/assets/oak_sign.png" alt="" data-size="line"> <strong>Табличка содержит текст</strong><br><code>if_game_sign_contains</code></p>                             | Проверяет, содержит ли табличка в определённом местоположении определённый текст.                  | <p><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение таблички</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сторона таблички</strong> <a data-footnote-ref href="#user-content-fn-5"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Вид сравнения</strong> <a data-footnote-ref href="#user-content-fn-6"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Строки для сравнения</strong> <a data-footnote-ref href="#user-content-fn-7"><strong><code>-></code></strong></a></p> |
| <p><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Игрок в игре</strong><br><code>if_game_has_player</code></p>                                        | Проверяет, находится ли определённый игрок в игре.                                                 | [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line">](../arguments/text.md) **Ник игрока или UUID**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <p><img src="../../../.gitbook/assets/grass_block.png" alt="" data-size="line"> <strong>Блок события равен</strong><br><code>if_game_event_block_equals</code></p>                          | Проверяет, равен ли блок текущего события определённому блоку.                                     | <p><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Типы блоков для проверки</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположения блоков для проверки</strong></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <p><img src="../../../.gitbook/assets/crafting_table.png" alt="" data-size="line"> <strong>Предмет события равен</strong><br><code>if_game_event_item_equals</code></p>                     | Проверяет, равен ли предмет текущего события определённому предмету.                               | <p><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для проверки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-8"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| <p><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Событие отменено</strong><br><code>if_game_event_is_canceled</code></p>                                 | Проверяет, отменено ли событие.                                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <p><img src="../../../.gitbook/assets/diamond_sword.png" alt="" data-size="line"> <strong>Атака была критической</strong><br><code>if_game_event_attack_is_critical</code></p>              | Проверяет, была ли атака в событии критической.                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <p><img src="../../../.gitbook/assets/dead_bush.png" alt="" data-size="line"> <strong>Источник урона события равен</strong><br><code>if_game_damage_cause_equals</code></p>                 | Проверяет, равен ли источник урона события выбранному.                                             | [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Источник урона** [**`->`**](#user-content-fn-9)[^9]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| <p><img src="../../../.gitbook/assets/potion_of_healing.png" alt="" data-size="line"> <strong>Источник исцеления равен</strong><br><code>if_game_heal_cause_equals</code></p>               | Проверяет, равен ли источник исцеления выбранному.                                                 | [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Источник исцеления** [**`->`**](#user-content-fn-10)[^10]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| <p><img src="../../../.gitbook/assets/flint_and_steel.png" alt="" data-size="line"> <strong>Источник огня равен</strong><br><code>if_game_ignite_cause_equals</code></p>                    | Проверяет, равен ли источник огня выбранному.                                                      | [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Источник огня** [**`->`**](#user-content-fn-11)[^11]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| <p><img src="../../../.gitbook/assets/note_block.png" alt="" data-size="line"> <strong>Инструмент равен</strong><br><code>if_game_instrument_equals</code></p>                              | Проверяет, равен ли инструмент в событии выбранному.                                               | [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Инструмент** [**`->`**](#user-content-fn-12)[^12]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <p><img src="../../../.gitbook/assets/structure_block.png" alt="" data-size="line"> <strong>Чанк загружен</strong><br><code>if_game_chunk_is_loaded</code></p>                              | Проверяет, загружен ли чанк на местоположении.                                                     | [<img src="../../../.gitbook/assets/paper.png" alt="" data-size="line">](../arguments/location.md) **Местоположение чанка**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |

[^1]: * Прямое запитывание
    * Непрямое запитывание

[^2]: * Любые предметы
    * Все предметы

[^3]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^4]: * Любые предметы
    * Все предметы

[^5]: * Любая
    * Передняя
    * Задняя

[^6]: * Сравнение по содержанию
    * Полное сравнение

[^7]: * 1 строка
    * 2 строка
    * 3 строка
    * 4 строка
    * Все строки

[^8]: * Полное сравнение
    * Игнорировать только количество
    * Игнорировать количество и прочность
    * Только тип предмета

[^9]: * Команда
    * Граница мира
    * Контакт
    * Атака сущности
    * Обширная атака сущности
    * Снаряд
    * Удушение
    * Падение
    * Прямой огонь
    * Горение
    * Таяние
    * Лава
    * Утопление
    * Взрыв блока
    * Взрыв сущности
    * Бездна
    * Молния
    * Суицид (грех)
    * Голод
    * Отравление
    * Магия
    * Иссушение
    * Падающий блок
    * Шипы
    * Дыхание дракона
    * Кастомный
    * Кинетическая энергия
    * Магма
    * Толпёжка
    * Высыхание
    * Замерзание
    * Взрывная волна

[^10]: * Исцеление в Мирном режиме
    * Исцеление при утолённом голоде
    * От употребления пищи
    * От кристалла Энда
    * От зелья или заклинания
    * Со временем от зелья или заклинания
    * При появлении Иссушителя
    * От эффекта Иссушение
    * Кастомный

[^11]: * Лава
    * Огниво
    * Распространение огня
    * Молния
    * Огненный заряд
    * Кристалл Энда
    * Взрыв
    * Стрела

[^12]: * Пианино
    * Бас-барабан
    * Малый барабан
    * Клаве
    * Бас-гитара
    * Флейта
    * Колокол
    * Гитара
    * Чаймс
    * Ксилофон
    * Железный ксилофон
    * Ковбелл
    * Диджериду
    * Бит
    * Банджо
    * Плинг
    * Зомби
    * Скелет
    * Крипер
    * Эндер-дракон
    * Визер-скелет
    * Пиглин
    * Кастомная голова
