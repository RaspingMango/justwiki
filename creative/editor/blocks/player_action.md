---
description: Выполняет действия над игроком или над группой игроков.
---

# Действие над игроком

<figure><img src="../../../.gitbook/assets/cobblestone.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `player_action`

***

## Использование

Поставьте блок в строку и нажмите <kbd>ПКМ</kbd> по нему, чтобы открыть меню опций блока. Перейдите в нужную категорию и выберите действие, которое необходимо выполнить.

При выборе действия, над его блоком может появиться хранилище (по умолчанию: сундук), в котором содержатся [аргументы](../arguments/) действия.

### Опции

{% tabs fullWidth="true" %}
{% tab title="Управление инвентарём" %}
<p align="center"><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Выдача, удаление, установка и сохранение предметов.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Выдать предмет</strong><br><code>player_give_items</code></td><td>Выдаёт игроку предметы из сундука.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для выдачи</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество предметов для выдачи</strong></td></tr><tr><td><img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> <strong>Установить предметы</strong><br><code>player_set_items</code></td><td>Устанавливает в инвентарь игрока соответственно предметы из сундука.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для выдачи в соответствующие слоты</strong></td></tr><tr><td><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> <strong>Установить предмет в слот</strong><br><code>player_set_slot_item</code></td><td>Устанавливает предмет в слот в инвентаре игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для выдачи</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Слот для выдачи</strong></td></tr><tr><td><img src="../../../.gitbook/assets/shield.png" alt="" data-size="line"> <strong>Установить экипировку</strong><br><code>player_set_equipment</code></td><td>Устанавливает предметы в один из слотов экипировки (броня и предметы в руках) игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для выдачи</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Слот снаряжения</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/iron_leggings.png" alt="" data-size="line"> <strong>Установить броню</strong><br><code>player_set_armor</code></td><td>Устанавливает броню игрока.<br><br>» Любой предмет или блок будет отображаться на голове, если положить его в слот головного убора.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Головной убор</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Нагрудник</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Штаны</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Ботинки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/lever.png" alt="" data-size="line"> <strong>Заменить предметы</strong><br><code>player_replace_items</code></td><td>Заменяет указанные предметы в инвентаре на определённый предмет.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Заменяемые предметы</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Заменяющий предмет</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество предметов для замены</strong></td></tr><tr><td><img src="../../../.gitbook/assets/cobweb.png" alt="" data-size="line"> <strong>Удалить предметы</strong><br><code>player_remove_items</code></td><td>Удаляет указанные предметы из инвентаря игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для удаления</strong></td></tr><tr><td><img src="../../../.gitbook/assets/string.png" alt="" data-size="line"> <strong>Очистить предметы</strong><br><code>player_clear_items</code></td><td>Удаляет все выбранные предметы из инвентаря игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для очистки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"> <strong>Очистить инвентарь</strong><br><code>player_clear_inventory</code></td><td>Очищает инвентарь игрока.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим очистки</strong> <a data-footnote-ref href="#user-content-fn-2"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/dropper.png" alt="" data-size="line"> <strong>Выдать случайный предмет</strong><br><code>player_give_random_item</code></td><td>Выдаёт игроку случайный предмет или стак из предметов в сундуке.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для выбора</strong></td></tr><tr><td><img src="../../../.gitbook/assets/fishing_rod.png" alt="" data-size="line"> <strong>Установить предмет на курсор</strong><br><code>player_set_cursor_item</code></td><td>Устанавливает предмет на курсор игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/cyan_shulker_box.png" alt="" data-size="line"> <strong>Сохранить текущий инвентарь</strong><br><code>player_save_inventory</code></td><td>Сохраняет текущий инвентарь игрока. Его можно будет загрузить позже с помощью <img src="../../../.gitbook/assets/lime_shulker_box.png" alt="" data-size="line"> <strong>Загрузить сохранённый инвентарь</strong>.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/lime_shulker_box.png" alt="" data-size="line"> <strong>Загрузить сохранённый инвентарь</strong><br><code>player_load_inventory</code></td><td>Загружает выбранный сохранённый инвентарь.<br><br>» Если нет сохранённого инвентаря, инвентарь игрока будет очищен.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Установить задержку предмета</strong><br><code>player_set_item_cooldown</code></td><td>Применяет визуальный эффект шкалы задержки для всех предметов выбранного типа.<br><br>» Задержка будет применена ко всем предметам выбранного типа.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Тип предмета для задержки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Задержка в тиках</strong><br><a href="../arguments/sound.md"><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"></a> <strong>Звук сброса задержки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Установить задержку для группы предметов</strong><br><code>player_set_item_group_cooldown</code></td><td>Применяет визуальный эффект шкалы задержки для всех предметов указанной группы.<br><br>» Задержка будет применена ко всем предметам, которые относятся к указанной группе.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Группа предметов</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Задержка</strong><br></td></tr><tr><td><img src="../../../.gitbook/assets/ender_eye.png" alt="" data-size="line"> <strong>Установить содержимое Эндер-сундука</strong><br><code>player_set_ender_chest_contents</code></td><td>Устанавливает предметы в инвентарь Эндер-сундука игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/ender_eye.png" alt="" data-size="line"> <strong>Очистить содержимое Эндер-сундука</strong><br><code>player_clear_ender_chest_contents</code></td><td>Очищает предметы в инвентаре Эндер-сундука игрока.</td><td></td></tr></tbody></table>
{% endtab %}

{% tab title="Коммуникация" %}
<p align="center"><img src="../../../.gitbook/assets/jungle_sign.png" alt="" data-size="line"> <strong>Отображение текста, отправка сообщений и проигрывание эффектов.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> <strong>Отправить сообщение</strong><br><code>player_send_message</code></td><td>Отправляет сообщение в чат указанным игрокам.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст для отправки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Объединение текста</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/bookshelf.png" alt="" data-size="line"> <strong>Диалог</strong><br><code>player_send_dialogue</code></td><td>Отправляет несколько сообщений в чат выбранным игрокам с задержкой после каждого сообщения.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст для отправки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Задержка между сообщениями</strong></td></tr><tr><td><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"> <strong>Очистить чат</strong><br><code>player_clear_chat</code></td><td>Удаляет все сообщения из окна чата выбранных игроков.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/birch_sign.png" alt="" data-size="line"> <strong>Отправить титул</strong><br><code>player_send_title</code></td><td>Высвечивает выбранному игроку две надписи на экран - титул и подтитул.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст титула</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст подтитула</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время появления в тиках</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Задержка в тиках</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время удаления в тиках</strong></td></tr><tr><td><img src="../../../.gitbook/assets/spruce_sign.png" alt="" data-size="line"> <strong>Отправить экшн-бар</strong><br><code>player_send_action_bar</code></td><td>Высвечивает выбранному игроку экшн-бар.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Сообщения в экшн-баре</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Объединение текста</strong> <a data-footnote-ref href="#user-content-fn-4"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/writable_book.png" alt="" data-size="line"> <strong>Открыть книгу</strong><br><code>player_open_book</code></td><td>Открывает книгу определённому игроку.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Книга для открытия</strong></td></tr><tr><td><img src="../../../.gitbook/assets/wither_skeleton_skull.png" alt="" data-size="line"> <strong>Установить босс-бар</strong><br><code>player_set_boss_bar</code></td><td>Устанавливает у определённого игрока пользовательский босс-бар.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID босс-бара</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Заполненность (0-100)</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Цвет</strong> <a data-footnote-ref href="#user-content-fn-5"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Стиль</strong> <a data-footnote-ref href="#user-content-fn-6"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Эффект неба</strong> <a data-footnote-ref href="#user-content-fn-7"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/netherrack.png" alt="" data-size="line"> <strong>Удалить босс-бар</strong><br><code>player_remove_boss_bar</code></td><td>Удаляет имеющийся босс-бар у определённого игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID босс-бара</strong></td></tr><tr><td><img src="../../../.gitbook/assets/totem_of_undying.png" alt="" data-size="line"> <strong>Отправить достижение игроку</strong><br><code>player_send_advancement</code></td><td>Высвечивает игроку пользовательское всплывающее достижение.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип достижения</strong> <a data-footnote-ref href="#user-content-fn-8"><strong><code>-></code></strong></a><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Название достижения</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Иконка достижения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/observer.png" alt="" data-size="line"> <strong>Установить текст в списке игроков</strong><br><code>player_set_player_list_info</code></td><td>Устанавливает текст над или под списком игроков для игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст в списке игроков</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Позиция</strong> <a data-footnote-ref href="#user-content-fn-9"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Объединение текста</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"> <strong>Проиграть звук</strong><br><code>player_play_sound</code></td><td>Проигрывает звук игроку.</td><td><a href="../arguments/sound.md"><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"></a> <strong>Звук для проигрывания</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение звука</strong></td></tr><tr><td><img src="../../../.gitbook/assets/goat_horn.png" alt="" data-size="line"> <strong>Проиграть звук от сущности</strong><br><code>player_play_sound_from_entity</code></td><td>Проигрывает звук игроку от указанной сущности.<br><br>» Стерео звуки не будут проигрываться.</td><td><a href="../arguments/sound.md"><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"></a> <strong>Звук для проигрывания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID сущности</strong></td></tr><tr><td><img src="../../../.gitbook/assets/music_disc_11.png" alt="" data-size="line"> <strong>Остановить звук</strong><br><code>player_stop_sound</code></td><td>Останавливает все или определённые звуки для игрока.</td><td><a href="../arguments/sound.md"><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"></a> <strong>Эффекты для остановки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/music_disc_11.png" alt="" data-size="line"> <strong>Остановить звуки по источнику</strong><br><code>player_stop_sounds_by_source</code></td><td>Останавливает все звуки по определённому источнику.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Источник звука</strong> <a data-footnote-ref href="#user-content-fn-10"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/jukebox.png" alt="" data-size="line"> <strong>Проиграть последовательность звуков</strong><br><code>player_play_sound_sequence</code></td><td>Проигрывает игроку последовательность звуков с задержкой между каждым звуком.</td><td><a href="../arguments/sound.md"><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"></a> <strong>Звуки для проигрывателя</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Задержка в тиках</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение звука</strong></td></tr><tr><td><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Показать диалоговое окно</strong><br><code>player_show_dialog_menu_from_nbt</code></td><td>Показывает игроку диалоговое окно из NBT-тегов.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>NBT-теги диалогового окна</strong></td></tr><tr><td><img src="../../../.gitbook/assets/dark_oak_hanging_sign.png" alt="" data-size="line"> <strong>Закрыть диалоговое окно</strong><br><code>player_close_dialog_menu</code></td><td>Закрывает текущее диалоговое окно игроку.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/knowledge_book.png" alt="" data-size="line"> <strong>Обновление подсказок в чате</strong><br><code>player_set_chat_completions</code></td><td>Обновляет игроку подсказки, показываемые при вводе текста в чате.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Подсказки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип обновления</strong> <a data-footnote-ref href="#user-content-fn-11"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Показать экран титров</strong><br><code>player_show_win_screen</code></td><td>Показывает игроку экран титров.<br><br>» Действие <a href="player_action.md#inventarnye-menyu"><img src="../../../.gitbook/assets/oak_door.png" alt="" data-size="line"> <strong>Закрыть Меню</strong></a> закрывает титры.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Показать экран демо-режима</strong><br><code>player_show_demo_screen</code></td><td>Показывает игроку экран демо-режима.</td><td></td></tr></tbody></table>
{% endtab %}

{% tab title="Инвентарные меню" %}
<p align="center"><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Отображение и изменение предметов в инвентарном меню.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/impulse_command_block.gif" alt="" data-size="line"> <strong>Показать меню</strong><br><code>player_show_inventory_menu</code></td><td>Показывает игроку инвентарное меню с выбранными предметами и названием.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы инвентаря</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Название инвентаря</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип инвентаря</strong> <a data-footnote-ref href="#user-content-fn-12"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/command_block_minecart.png" alt="" data-size="line"> <strong>Расширить меню</strong><br><code>player_expand_inventory_menu</code></td><td>Расширяет открытое инвентарное меню игрока на выбранное количество строк и заполняет его указанными предметами.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для заполнения</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество строк для расширения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> <strong>Установить предмет в слот</strong><br><code>player_set_inventory_menu_item</code></td><td>Устанавливает предмет в указанный слот открытого инвентарного меню игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для установки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Слот для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Установить название меню</strong><br><code>player_set_inventory_menu_name</code></td><td>Устанавливает новое название для открытого инвентарного меню игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Новое название</strong></td></tr><tr><td><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"> <strong>Установить кастомный ID открытого инвентаря</strong><br><code>player_set_inventory_menu_custom_id</code></td><td>Устанавливает кастомный ID для открытого меню игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Кастомный ID</strong></td></tr><tr><td><img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> <strong>Добавить строку меню</strong><br><code>player_add_inventory_menu_row</code></td><td>Добавляет строку с указанными предметами в инвентаре типа "Сундук".</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Позиция строки</strong> <a data-footnote-ref href="#user-content-fn-13"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/tnt.png" alt="" data-size="line"> <strong>Убрать строки меню</strong><br><code>player_remove_inventory_menu_row</code></td><td>Убирает одну или несколько строк в инвентаре типа "Сундук".</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество строк</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Позиция строки</strong> <a data-footnote-ref href="#user-content-fn-14"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/oak_door.png" alt="" data-size="line"> <strong>Закрыть меню</strong><br><code>player_close_inventory</code></td><td>Закрывает открытое инвентарное меню игрока.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Открыть меню блока</strong><br><code>player_open_container_inventory</code></td><td>Открывает для игрока меню блока в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока для открытия</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Параметры" %}
<p align="center"><img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> <strong>Изменение параметров игрока, такие как здоровье, голод, опыт и другое.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> <strong>Нанести урон</strong><br><code>player_damage</code></td><td>Наносит урон игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество урона</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Источник урона (имя или UUID существа)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/potion_of_healing.png" alt="" data-size="line"> <strong>Исцелить игрока</strong><br><code>player_heal</code></td><td>Исцеляет игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество половинок сердец для излечения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> <strong>Установить здоровье игрока</strong><br><code>player_set_health</code></td><td>Устанавливает здоровье игрока на выбранное количество.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество здоровья</strong></td></tr><tr><td><img src="../../../.gitbook/assets/golden_apple.png" alt="" data-size="line"> <strong>Установить максимальное здоровье игрока</strong><br><code>player_set_max_health</code></td><td>Устанавливает максимальное количество здоровья для игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Максимальное количество здоровья</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Исцелить игрока</strong> <a data-footnote-ref href="#user-content-fn-15"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/honey_bottle.png" alt="" data-size="line"> <strong>Установить дополнительное здоровье</strong><br><code>player_set_absorption_health</code></td><td>Устанавливает дополнительное здоровье игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество дополнительного здоровья</strong></td></tr><tr><td><img src="../../../.gitbook/assets/cooked_chicken.png" alt="" data-size="line"> <strong>Установить голод</strong><br><code>player_set_food</code></td><td>Устанавливает уровень голода игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень голода</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим установки</strong> <a data-footnote-ref href="#user-content-fn-16"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/cooked_beef.png" alt="" data-size="line"> <strong>Установить насыщенность</strong><br><code>player_set_saturation</code></td><td>Устанавливает второстепенный уровень голода (насыщенность) игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень насыщенности</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим установки</strong> <a data-footnote-ref href="#user-content-fn-16"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/rotten_flesh.png" alt="" data-size="line"> <strong>Установить уровень истощения</strong><br><code>player_set_exhaustion</code></td><td>Устанавливает уровень истощения игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень истощения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим установки</strong> <a data-footnote-ref href="#user-content-fn-16"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/potion_of_leaping.png" alt="" data-size="line"> <strong>Прибавить уровень</strong><br><code>player_give_experience</code></td><td>Прибавляет уровень игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество для прибавки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип прибавления</strong> <a data-footnote-ref href="#user-content-fn-17"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> <strong>Установить уровень</strong><br><code>player_set_experience</code></td><td>Устанавливает уровень игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество для установки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип установки</strong> <a data-footnote-ref href="#user-content-fn-18"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/dragon_breath.png" alt="" data-size="line"> <strong>Выдать эффект</strong><br><code>player_give_potion_effect</code></td><td>Выдаёт выбранные эффекты игроку.</td><td><a href="../arguments/potion.md"><img src="../../../.gitbook/assets/dragon_breath.png" alt="" data-size="line"></a> <strong>Эффекты для выдачи</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Перезаписывать существующие эффекты</strong> <a data-footnote-ref href="#user-content-fn-19"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Показывать иконку эффекта</strong> <a data-footnote-ref href="#user-content-fn-20"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Показывать частицы</strong> <a data-footnote-ref href="#user-content-fn-21"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/glass_bottle.png" alt="" data-size="line"> <strong>Удалить эффект</strong><br><code>player_remove_potion_effect</code></td><td>Удаляет выбранные эффекты у игрока.</td><td><a href="../arguments/potion.md"><img src="../../../.gitbook/assets/dragon_breath.png" alt="" data-size="line"></a> <strong>Эффекты для удаления</strong></td></tr><tr><td><img src="../../../.gitbook/assets/cauldron.png" alt="" data-size="line"> <strong>Очистить эффекты</strong><br><code>player_clear_potion_effects</code></td><td>Очищает все эффекты у игрока.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Установить слот</strong><br><code>player_set_hotbar_slot</code></td><td>Устанавливает выбранный слот игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Номер слота</strong></td></tr><tr><td><img src="../../../.gitbook/assets/golden_sword.png" alt="" data-size="line"> <strong>Установить скорость атаки</strong><br><code>player_set_attack_speed</code></td><td>Устанавливает скорость атаки игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Скорость атаки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/diamond_helmet.png" alt="" data-size="line"> <strong>Установить длительность неуязвимости</strong><br><code>player_set_invulnerability_ticks</code></td><td>Устанавливает длительность неуязвимости для игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность неуязвимости (в тиках)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/enchanted_diamond_helmet.gif" alt="" data-size="line"> <strong>Установить максимальную длительность неуязвимости</strong><br><code>player_set_max_invulnerability_ticks</code></td><td>Устанавливает максимальную длительность неуязвимости для игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность (в тиках)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/blaze_powder.png" alt="" data-size="line"> <strong>Поджечь игрока</strong><br><code>player_set_fire_ticks</code></td><td>Поджигает игрока на выбранное время.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность (в тиках)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/powder_snow_bucket.png" alt="" data-size="line"> <strong>Установить время заморозки</strong><br><code>player_set_freeze_ticks</code></td><td>Устанавливает игроку время заморозки (количество тиков, которое игрок провёл в рыхлом снегу).</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время заморозки в тиках</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Блокировка состояния (время не будет изменяться)</strong> <a data-footnote-ref href="#user-content-fn-22"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/water_bottle.png" alt="" data-size="line"> <strong>Установить оставшийся воздух</strong><br><code>player_set_air_ticks</code></td><td>Устанавливает оставшийся воздух игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество оставшегося воздуха (в тиках)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/hay_block.png" alt="" data-size="line"> <strong>Установить дистанцию падения</strong><br><code>player_set_fall_distance</code></td><td>Устанавливает дистанцию, с которой падает игрок.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Дистанция падения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/netherite_boots.png" alt="" data-size="line"> <strong>Установить скорость движения</strong><br><code>player_set_movement_speed</code></td><td>Устанавливает скорость движения игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Скорость движения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип движения</strong> <a data-footnote-ref href="#user-content-fn-23"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> <strong>Установить атрибут</strong><br><code>player_set_attribute</code></td><td>Устанавливает игроку указанное значение атрибута.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Значение атрибута</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип атрибута</strong> <a data-footnote-ref href="#user-content-fn-24"><strong><code>-></code></strong></a></td></tr></tbody></table>
{% endtab %}

{% tab title="Настройки" %}
<p align="center"><img src="../../../.gitbook/assets/anvil.png" alt="" data-size="line"> <strong>Базовые настройки игрока, такие как режим игры, полёт и другое.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> <strong>Установить режим игры</strong><br><code>player_set_gamemode</code></td><td>Устанавливает режим игры для игрока.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим игры</strong> <a data-footnote-ref href="#user-content-fn-25"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим полёта</strong> <a data-footnote-ref href="#user-content-fn-26"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> <strong>Установить разрешение полёта игрока</strong><br><code>player_set_allow_flying</code></td><td>Устанавливает разрешение полёта для игрока.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Может летать</strong> <a data-footnote-ref href="#user-content-fn-27"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/netherite_sword.png" alt="" data-size="line"> <strong>Установить разрешение атаковать игроков</strong><br><code>player_set_pvp</code></td><td>Устанавливает разрешение игроку атаковать других игроков и наносить им урон.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Может атаковать</strong> <a data-footnote-ref href="#user-content-fn-28"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/redstone.png" alt="" data-size="line"> <strong>Установить выпадение предметов</strong><br><code>player_set_death_drops</code></td><td>Устанавливает выпадение предметов из игрока при смерти.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Выпадение предметов</strong> <a data-footnote-ref href="#user-content-fn-29"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> <strong>Установить сохранение инвентаря</strong><br><code>player_set_inventory_kept</code></td><td>Устанавливает игроку сохранение инвентаря при смерти.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сохранение инвентаря</strong> <a data-footnote-ref href="#user-content-fn-30"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> <strong>Установить режим столкновения</strong><br><code>player_set_collidable</code></td><td>Устанавливает игроку режим столкновения с существами.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим столкновения</strong> <a data-footnote-ref href="#user-content-fn-31"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/glass_bottle.png" alt="" data-size="line"> <strong>Установить видимость</strong><br><code>player_set_default_visible</code></td><td>Устанавливает игроку видимость.<br><br>» Видимость игрока может быть изменена через действие <a href="player_action.md#mir"><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Скрыть сущность игроку</strong></a>.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Видимость</strong> <a data-footnote-ref href="#user-content-fn-32"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Отображение ника игрока</strong><br><code>player_set_nametag_visible</code></td><td>Отобразит или скроет ник над головой.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Отображение ника</strong> <a data-footnote-ref href="#user-content-fn-33"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/totem_of_undying.png" alt="" data-size="line"> <strong>Установить мгновенное возрождение</strong><br><code>player_set_instant_respawn</code></td><td>Устанавливает мгновенное возрождение игроку.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Мгновенное возрождение</strong> <a data-footnote-ref href="#user-content-fn-34"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"> <strong>Установить местоположение возрождения</strong><br><code>player_set_spawn_point</code></td><td>Устанавливает игроку новое местоположение возрождения.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение возрождения</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Передвижение" %}
<p align="center"><img src="../../../.gitbook/assets/leather_boots.png" alt="" data-size="line"> <strong>Запуск, телепортация и другие взаимодействия, связанные с перемещением игрока.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> <strong>Телепортация</strong><br><code>player_teleport</code></td><td>Телепортирует игрока в выбранное местоположение.<br><br>» Закрывает открытое инвентарное меню.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Новая позиция</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Оставить текущий поворот</strong> <a data-footnote-ref href="#user-content-fn-35"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сохранение инерции</strong> <a data-footnote-ref href="#user-content-fn-36"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Спешиться после телепортации</strong> <a data-footnote-ref href="#user-content-fn-37"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> <strong>Случайная телепортация</strong><br><code>player_randomized_teleport</code></td><td>Телепортирует игрока в случайное местоположение.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Позиции для телепорта</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Оставить текущий поворот</strong> <a data-footnote-ref href="#user-content-fn-35"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сохранение инерции</strong> <a data-footnote-ref href="#user-content-fn-36"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Спешиться после телепортации</strong> <a data-footnote-ref href="#user-content-fn-37"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/chorus_fruit.png" alt="" data-size="line"> <strong>Последовательность телепортаций</strong><br><code>player_teleport_sequence</code></td><td>Телепортирует игрока между местоположениями с заданной задержкой.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Задержка в тиках</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Позиции для телепортации</strong></td></tr><tr><td><img src="../../../.gitbook/assets/slime_block.png" alt="" data-size="line"> <strong>Подбросить вверх</strong><br><code>player_launch_up</code></td><td>Подбрасывает игрока вверх или вниз в зависимости от силы.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Сила подбрасывания</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Учитывать текущую инерцию</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> <strong>Запустить вперёд</strong><br><code>player_launch_forward</code></td><td>Запускает игрока вперёд или назад по направлению взгляда в зависимости от силы.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Сила подбрасывания</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Учитывать текущую инерцию</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Ось запуска</strong> <a data-footnote-ref href="#user-content-fn-39"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/sticky_piston.png" alt="" data-size="line"> <strong>Запустить к местоположению</strong><br><code>player_launch_to_location</code></td><td>Запускает игрока к выбранному местоположению.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Конечная позиция</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Сила запуска</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Учитывать текущую инерцию</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/saddle.png" alt="" data-size="line"> <strong>Посадить на существо</strong><br><code>player_ride_entity</code></td><td>Сажает игрока на существо или другого игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID цели</strong></td></tr><tr><td><img src="../../../.gitbook/assets/tnt_minecart.png" alt="" data-size="line"> <strong>Высадить из транспорта</strong><br><code>player_leave_vehicle</code></td><td>Высаживает игрока из транспорта или существа.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> <strong>Установить полёт</strong><br><code>player_set_flying</code></td><td>Устанавливает для игрока состояние полёта.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Полёт</strong> <a data-footnote-ref href="#user-content-fn-40"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/elytra.png" alt="" data-size="line"> <strong>Установить полёт на элитрах</strong><br><code>player_set_gliding</code></td><td>Устанавливает для игрока состояние полёта на элитрах.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Полёт на элитрах</strong> <a data-footnote-ref href="#user-content-fn-41"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"> <strong>Установить поворот</strong><br><code>player_set_rotation</code></td><td>Устанавливает поворот игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Горизонтальный поворот (yaw)</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Вертикальный поворот (pitch)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"> <strong>Установить поворот по вектору</strong><br><code>player_set_rotation_by_vector</code></td><td>Устанавливает поворот игрока по вектору.</td><td><a href="../arguments/vector.md"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"></a> <strong>Вектор для поворота</strong></td></tr><tr><td><img src="../../../.gitbook/assets/spider_eye.png" alt="" data-size="line"> <strong>Повернуть к местоположению</strong><br><code>player_face_location</code></td><td>Поворачивает игрока в сторону к местоположению.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение</strong></td></tr><tr><td><img src="../../../.gitbook/assets/arrow_of_oozing.png" alt="" data-size="line"> <strong>Запустить по вектору</strong><br><code>player_set_velocity</code></td><td>Запускает игрока по указанному вектору.</td><td><a href="../arguments/vector.md"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"></a> <strong>Вектор движения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Учитывать текущую инерцию</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/ender_eye.png" alt="" data-size="line"> <strong>Следить за целью</strong><br><code>player_spectate_target</code></td><td>Устанавливает цель слежения игрока в режиме наблюдателя.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID цели</strong></td></tr><tr><td><img src="../../../.gitbook/assets/firework_rocket.png" alt="" data-size="line"> <strong>Ускорить полёт на элитрах</strong><br><code>player_boost_elytra</code></td><td>Ускоряет полёт игрока на элитрах с силой указанного фейерверка.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Фейерверк для ускорения</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Мир" %}
<p align="center"><img src="../../../.gitbook/assets/spectral_arrow.png" alt="" data-size="line"> <strong>Отображение визуальных эффектов в мире, связанные с игроком.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> <strong>Запустить снаряд</strong><br><code>player_launch_projectile</code></td><td>Запустить снаряд из местоположения игрока.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Снаряд для запуска</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Место запуска</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя снаряда</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Скорость снаряда</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Отклонение снаряда (0, чтобы снаряд летел ровно)</strong><br><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>След, который будет оставаться за снарядом</strong></td></tr><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Установить время игрока</strong><br><code>player_set_time</code></td><td>Установить время игроку, не меняя его для остальных игроков.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время в тиках</strong></td></tr><tr><td><img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> <strong>Установить погоду</strong><br><code>player_set_weather</code></td><td>Установить погоду для игрока, не влияя на других игроков.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип погоды</strong> <a data-footnote-ref href="#user-content-fn-42"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/blue_dye.png" alt="" data-size="line"> <strong>Установить уровень дождя</strong><br><code>player_set_rain_level</code></td><td>Устанавливает уровень дождя игроку.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень дождя (от 0 до 100)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/lightning_rod.png" alt="" data-size="line"> <strong>Установить уровень грозы</strong><br><code>player_set_thunder_level</code></td><td>Устанавливает уровень грозы игроку.<br><br>» Для установки необходима дождливая погода.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень грозы (от 0 до 100)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/bucket.png" alt="" data-size="line"> <strong>Сбросить погоду</strong><br><code>player_reset_weather</code></td><td>Сбрасывает погоду игроку.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/compass.png" alt="" data-size="line"> <strong>Установить цель компаса</strong><br><code>player_set_compass_target</code></td><td>Установить цель компаса для игрока, в сторону которой будет крутиться стрелка компаса.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Цель компаса</strong></td></tr><tr><td><img src="../../../.gitbook/assets/fire_coral_block.png" alt="" data-size="line"> <strong>Показать блок</strong><br><code>player_display_block</code></td><td>Показать игроку блок, не влияя на других игроков.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок, который требуется отобразить</strong></td></tr><tr><td><img src="../../../.gitbook/assets/dead_fire_coral_block.png" alt="" data-size="line"> <strong>Скрыть отображаемые блоки</strong><br><code>player_remove_display_blocks</code></td><td>Скрывает от игрока все отображаемые блоки в выбранном пространстве, не влияя на других игроков (максимальный размер пространства - 500 блоков).</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение первого угла</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение второго угла</strong></td></tr><tr><td><img src="../../../.gitbook/assets/cracked_stone_bricks.png" alt="" data-size="line"> <strong>Показать анимацию ломания блока</strong><br><code>player_send_break_animation</code></td><td>Показывает анимацию ломания блока (трещины) для игрока, не влияя на других игроков.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположения блоков</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень разрушения блока (от 0 до 10)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Открыть/Закрыть блок</strong><br><code>player_set_block_opened_state</code></td><td>Отобразить игроку закрытие/открытие блока не меняя состояния блока для других игроков.<br><br>Работает с:<br>» Сундуком<br>» Сундуком-ловушкой<br>» Эндер-сундуком<br>» Шалкеровым ящиком<br>» Бочкой</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Состояние</strong> <a data-footnote-ref href="#user-content-fn-43"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/oak_sign.png" alt="" data-size="line"> <strong>Показать текст таблички</strong><br><code>player_display_sign_text</code></td><td>Показать игроку изменение текста таблички, не изменяя её текст для других игроков.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение таблички</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Первая строка таблички</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Вторая строка таблички</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Третья строка таблички</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Четвёртая строка таблички</strong></td></tr><tr><td><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Показать голограмму</strong><br><code>player_display_hologram</code></td><td>Показывает игроку голограмму. Чтобы удалить голограмму на местоположении, оставьте текст пустым.<br><br>» Чтобы перенести текст на новую строку, используйте символы <code>\n</code>, к примеру: <code>Строка1\nСтрока2</code>.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение голограммы</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст голограммы</strong></td></tr><tr><td><img src="../../../.gitbook/assets/bell.png" alt="" data-size="line"> <strong>Показать удар в колокол</strong><br><code>player_display_bell_ring</code></td><td>Показывает игроку анимацию удара в колокол, не влияя на других игроков.<br><br>Работает с:<br>» Колоколами<br><br>» Направление "Вниз" останавливает анимацию удара.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение колокола</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Направление удара</strong> <a data-footnote-ref href="#user-content-fn-44"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/prismarine_wall.png" alt="" data-size="line"> <strong>Установить границу мира игроку</strong><br><code>player_set_world_border</code></td><td>Установить границу мира для игрока, не меняя её для других игроков.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Центр границы мира</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Размер границы мира</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Расстояние до появления красной обводки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/nether_brick_wall.png" alt="" data-size="line"> <strong>Передвинуть границу мира</strong><br><code>player_shift_world_border</code></td><td>Передвинуть границу мира для игрока, не меняя её для других игроков.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Старый размер границы мира</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Новый размер границы мира</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время изменения размера</strong></td></tr><tr><td><img src="../../../.gitbook/assets/stone_brick_wall.png" alt="" data-size="line"> <strong>Удалить границу мира</strong><br><code>player_remove_world_border</code></td><td>Установить границу мира для игрока на значение по умолчанию.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Установить тик-рейт</strong><br><code>player_set_tick_rate</code></td><td>Устанавливает игроку тик-рейт, не влияя на других игроков.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Тик-рейт</strong></td></tr><tr><td><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Скрыть сущность игроку</strong><br><code>player_hide_entity</code></td><td>Скрывает указанную сущность для игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID сущности</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Скрытие</strong> <a data-footnote-ref href="#user-content-fn-45"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/spyglass.png" alt="" data-size="line"> <strong>Установить дистанцию прорисовки</strong><br><code>player_set_fog_distance</code></td><td>Устанавливает дистанцию прорисовки чанков для игрока. Значение "-1" сбрасывает до стандартной.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Дистанция прорисовки в чанках (2-32)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> <strong>Установить дистанцию симуляции</strong><br><code>player_set_simulation_distance</code></td><td>Устанавливает дистанцию симуляции чанков для игрока.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Дистанция симуляции в чанках (2-32)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/end_portal_frame.png" alt="" data-size="line"> <strong>Показать анимацию луча Врат Энда</strong><br><code>player_display_end_gateway_beam</code></td><td>Показывает анимацию луча Врат Энда на определённом местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение луча</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Цвет луча</strong> <a data-footnote-ref href="#user-content-fn-46"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/hopper_minecart.png" alt="" data-size="line"> <strong>Показать анимацию подбора предмета</strong><br><code>player_display_pick_up_animation</code></td><td>Показывает игроку анимацию подбора предмета.<br><br>» Действие работает с любой сущностью, в том числе игроком.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID поднимаемой сущности</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID сущности, которая поднимает</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество поднимаемых предметов</strong></td></tr><tr><td><img src="../../../.gitbook/assets/lime_stained_glass.png" alt="" data-size="line"> <strong>Показать отладочный маркер</strong><br><code>player_show_debug_marker</code></td><td>Показывает игроку отладочный маркер на местоположении на указанное время. Красный и синий цвет работают для игроков на версии 1.19.4 и выше.<br><br>» Оставьте аргумент "Отображаемое имя" пустым, чтобы полностью скрыть имя.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение появления</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Отображаемое имя</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность в миллисекундах (не обязательно)</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Красный цвет (от 0 до 100)</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Зелёный цвет (от 0 до 100)</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Синий цвет (от 0 до 100)</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Прозрачность (от 0 до 100)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> <strong>Удалить отладочные маркеры</strong><br><code>player_clear_debug_markers</code></td><td>Удаляет все отладочные маркеры для игрока.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/glowstone_dust.png" alt="" data-size="line"> <strong>Установить свечение сущности</strong><br><code>player_set_entity_glowing</code></td><td>Включает или выключает свечение сущности для данного игрока.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID сущности</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Цвет свечения</strong> <a data-footnote-ref href="#user-content-fn-47"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Свечение</strong> <a data-footnote-ref href="#user-content-fn-48"><strong><code>-></code></strong></a></td></tr></tbody></table>
{% endtab %}

{% tab title="Частицы" %}
<p align="center"><img src="../../../.gitbook/assets/white_dye.png" alt="" data-size="line"> <strong>Отображение различных эффектов частиц для игроков.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/gold_nugget.png" alt="" data-size="line"> <strong>Отобразить эффект частицы</strong><br><code>player_display_particle</code></td><td>Отображает игроку эффект частицы на выбранном местоположении.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение эффекта</strong></td></tr><tr><td><img src="../../../.gitbook/assets/stick.png" alt="" data-size="line"> <strong>Отобразить линию частиц</strong><br><code>player_display_particle_line</code></td><td>Отображает игроку линию эффекта частиц от начального местоположения до конечного с определённым расстоянием.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Начальное местоположение</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Конечное местоположение</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество/расстояние между частицами</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип отображения частиц</strong> <a data-footnote-ref href="#user-content-fn-49"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"> <strong>Отобразить луч частиц</strong><br><code>player_display_particle_ray</code></td><td>Отображает игроку луч эффекта частиц от начального местоположения по указанному вектору с определённым расстоянием.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Начальное местоположение</strong><br><a href="../arguments/vector.md"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"></a> <strong>Направление луча</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество/расстояние между частицами</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип отображения частиц</strong> <a data-footnote-ref href="#user-content-fn-49"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Отобразить окружность частиц</strong><br><code>player_display_particle_circle</code></td><td>Отображает игроку окружность из эффекта частиц с указанными параметрами.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Центр окружности</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Радиус круга</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество точек круга</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Начальный угол</strong><br><a href="../arguments/vector.md"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"></a> <strong>Нормаль плоскости, к которой окружность будет перпендикулярна</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип угла</strong> <a data-footnote-ref href="#user-content-fn-50"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/tinted_glass.png" alt="" data-size="line"> <strong>Отобразить куб частиц</strong><br><code>player_display_particle_cube</code></td><td>Отображает игроку куб из эффекта частиц с указанными параметрами.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Первый угол куба</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Второй угол куба</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Расстояние между частицами</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип куба</strong> <a data-footnote-ref href="#user-content-fn-51"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"> <strong>Отобразить сферу частиц</strong><br><code>player_display_particle_sphere</code></td><td>Отображает игроку сферу из эффекта частиц с указанными параметрами.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Центр сферы</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Радиус сферы</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество точек сферы</strong></td></tr><tr><td><img src="../../../.gitbook/assets/string.png" alt="" data-size="line"> <strong>Отобразить спираль частиц</strong><br><code>player_display_particle_spiral</code></td><td>Отображает игроку спираль из эффекта частиц с указанными параметрами.</td><td><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Эффект частиц для отображения</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Центр спирали</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Дистанция спирали</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Радиус спирали</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество точек спирали</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество оборотов</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Начальный угол</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип угла</strong> <a data-footnote-ref href="#user-content-fn-50"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/sculk_sensor.gif" alt="" data-size="line"> <strong>Отобразить частицу вибрации</strong><br><code>player_display_vibration</code></td><td>Отображает игроку частицу вибрации, движущуюся с одной точки на другую.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Начальное местоположение</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Конечное местоположение</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время полёта до места назначения в тиках</strong></td></tr><tr><td><img src="../../../.gitbook/assets/golden_axe.png" alt="" data-size="line"> <strong>Отобразить эффект молнии</strong><br><code>player_display_lightning</code></td><td>Отобразить молнию игроку, не показывая её для других игроков и не поджигая местность.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Место удара молнии</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Внешний вид" %}
<p align="center"><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Действия, которые изменяют внешний вид игрока.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/player_disguise_as_entity.png" alt="" data-size="line"> <strong>Замаскировать игрока под сущность</strong><br><code>player_disguise_as_entity</code></td><td>Маскирует игрока под выбранную сущность.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Сущность для маскировки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Видимость для игрока</strong> <a data-footnote-ref href="#user-content-fn-52"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/player_disguise_as_block.png" alt="" data-size="line"> <strong>Замаскировать игрока под блок</strong><br><code>player_disguise_as_block</code></td><td>Маскирует игрока под выбранный блок.</td><td><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок для маскировки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Видимость для игрока</strong> <a data-footnote-ref href="#user-content-fn-52"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/chest_head.png" alt="" data-size="line"> <strong>Замаскировать игрока под предмет</strong><br><code>player_disguise_as_item</code></td><td>Маскирует игрока под предмет.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для маскировки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Видимость для игрока</strong> <a data-footnote-ref href="#user-content-fn-52"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Убрать маскировку</strong><br><code>player_remove_disguise</code></td><td>Убирает маскировку игроку.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/player_disguise_as_entity.png" alt="" data-size="line"> <strong>Замаскировать себя под сущность</strong><br><code>player_self_disguise_as_entity</code></td><td>Маскирует игрока под сущность, но эту маскировку видно только этому игроку.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Сущность для маскировки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/player_disguise_as_block.png" alt="" data-size="line"> <strong>Замаскировать себя под блок</strong><br><code>player_self_disguise_as_block</code></td><td>Маскирует игрока под блок, но эту маскировку видно только этому игроку.</td><td><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок для маскировки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/chest_head.png" alt="" data-size="line"> <strong>Замаскировать себя под предмет</strong><br><code>player_self_disguise_as_item</code></td><td>Маскирует игрока под предмет, но эту маскировку видно только этому игроку.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для маскировки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Убрать свою маскировку</strong><br><code>player_remove_self_disguise</code></td><td>Убирает маскировку игрока, которую видно только ему.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/player_set_skin.png" alt="" data-size="line"> <strong>Установить скин</strong><br><code>player_set_skin</code></td><td>Устанавливает скин указанного игрока для цели события.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя или UUID скина</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип сервера скинов</strong> <a data-footnote-ref href="#user-content-fn-53"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Убрать скин</strong><br><code>player_remove_skin</code></td><td>Возвращает обычный скин цели события.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Проиграть анимацию игроку</strong><br><code>player_play_animation_action</code></td><td>Проигрывает для игрока определённую анимацию.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип анимации</strong> <a data-footnote-ref href="#user-content-fn-54"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/cactus.png" alt="" data-size="line"> <strong>Проиграть анимацию получения урона</strong><br><code>player_play_hurt_animation</code></td><td>Проигрывает для игрока анимацию получения урона с определённым наклоном.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Угол получения урона (от 0 до 360 градусов)</strong></td></tr><tr><td><img src="../../../.gitbook/assets/black_bed.png" alt="" data-size="line"> <strong>Установить позу игроку</strong><br><code>player_set_pose</code></td><td>Устанавливает определённую позу игроку.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Отображаемая поза</strong> <a data-footnote-ref href="#user-content-fn-55"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Блокировка позы</strong> <a data-footnote-ref href="#user-content-fn-56"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> <strong>Сбросить позу игроку</strong><br><code>player_remove_pose</code></td><td>Сбрасывает позу игроку.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/golden_sword.png" alt="" data-size="line"> <strong>Проиграть анимацию взмаха руки</strong><br><code>player_swing_hand</code></td><td>Проигрывает для игрока анимацию взмаха руки.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип руки</strong> <a data-footnote-ref href="#user-content-fn-57"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/campfire.png" alt="" data-size="line"> <strong>Установить визуальный огонь</strong><br><code>player_set_visual_fire</code></td><td>Устанавливает игроку эффект горения.</td><td><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Визуальный огонь</strong> <a data-footnote-ref href="#user-content-fn-58"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> <strong>Установить стрелы на игроке</strong><br><code>player_set_arrows_in_body</code></td><td>Отображает определённое количество стрел на игроке.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество отображаемых стрел</strong></td></tr><tr><td><img src="../../../.gitbook/assets/bee_head.png" alt="" data-size="line"> <strong>Установить жало пчелы на игроке</strong><br><code>player_set_bee_stingers_in_body</code></td><td>Отображает определённое количество жал пчёл на игроке.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество отображаемых жал пчёл</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Разное" %}
<p align="center"><img src="../../../.gitbook/assets/bedrock.png" alt="" data-size="line"> <strong>Действия, которые относятся к другим категориям.</strong></p>

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> <strong>Выгнать игрока</strong><br><code>player_kick</code></td><td>Выгоняет игрока из мира.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/golden_boots.png" alt="" data-size="line"> <strong>Переместить игрока в другой мир</strong><br><code>player_redirect_world</code></td><td>Перемещает игрока в мир с указанным ID.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID мира</strong></td></tr><tr><td><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Показать скорборд</strong><br><code>player_show_scoreboard</code></td><td>Отображает определённый скорборд игроку. Для отображения указанный скорборд должен иметь минимум одно значение.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong></td></tr><tr><td><img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> <strong>Скрыть скорборд</strong><br><code>player_hide_scoreboard</code></td><td>Скрывает текущий скорборд игрока.</td><td></td></tr></tbody></table>
{% endtab %}
{% endtabs %}

### Селекторы

Нажатием <kbd>Shift</kbd> + <kbd>ПКМ</kbd> по блоку кода открывается меню селекторов, позволяющее выбрать цель, по отношению к которой будет воспроизведено действие.

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

[^1]: **Слот снаряжения** `slot`:

    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Основная рука**\
      `hand`
    * <img src="../../../.gitbook/assets/shield.png" alt="" data-size="line"> **Второстепенная рука**\
      `off_hand`
    * <img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> **Ботинки**\
      `feet`
    * <img src="../../../.gitbook/assets/iron_leggings.png" alt="" data-size="line"> **Поножи**\
      `legs`
    * <img src="../../../.gitbook/assets/iron_chestplate.png" alt="" data-size="line"> **Нагрудник**\
      `chest`
    * <img src="../../../.gitbook/assets/iron_helmet.png" alt="" data-size="line"> **Шлем**\
      `head`
    * <img src="../../../.gitbook/assets/iron_chestplate.png" alt="" data-size="line"> **Тело**\
      `body`

[^2]: **Режим очистки** `clear_mode`:

    * <img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> **Весь инвентарь**\
      `entire`
    * <img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> **Главный инвентарь**\
      `main`
    * <img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> **Верхний инвентарь**\
      `upper`
    * <img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> **Хот-бар**\
      `hotbar`
    * <img src="../../../.gitbook/assets/iron_chestplate.png" alt="" data-size="line"> **Броня**\
      `armor`

[^3]: **Объединение текста** `merging`:

    * <img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> **Разделение пробелом**\
      `spaces`
    * <img src="../../../.gitbook/assets/sticky_piston.png" alt="" data-size="line"> **Объединение**\
      `concatenation`
    * <img src="../../../.gitbook/assets/shears.png" alt="" data-size="line"> **Разделение на строки**\
      `separate_lines`

[^4]: **Объединение текста** `merging`:

    * <img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> **Разделение пробелом**\
      `spaces`
    * <img src="../../../.gitbook/assets/sticky_piston.png" alt="" data-size="line"> **Объединение**\
      `concatenation`

[^5]: **Цвет** `color`:

    * <img src="../../../.gitbook/assets/magenta_concrete.png" alt="" data-size="line"> **Розовый**\
      `pink`
    * <img src="../../../.gitbook/assets/light_blue_concrete.png" alt="" data-size="line"> **Синий**\
      `blue`
    * <img src="../../../.gitbook/assets/red_concrete.png" alt="" data-size="line"> **Красный**\
      `red`
    * <img src="../../../.gitbook/assets/lime_concrete.png" alt="" data-size="line"> **Зелёный**\
      `green`
    * <img src="../../../.gitbook/assets/yellow_concrete.png" alt="" data-size="line"> **Жёлтый**\
      `yellow`
    * <img src="../../../.gitbook/assets/purple_concrete.png" alt="" data-size="line"> **Фиолетовый**\
      `purple`
    * <img src="../../../.gitbook/assets/white_concrete.png" alt="" data-size="line"> **Белый**\
      `white`

[^6]: **Стиль** `style`:

    * <img src="../../../.gitbook/assets/iron_block.png" alt="" data-size="line"> **Сплошной**\
      `progress`
    * <img src="../../../.gitbook/assets/stone_sword.png" alt="" data-size="line"> **6 сегментов**\
      `notched_6`
    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **10 сегментов**\
      `notched_10`
    * <img src="../../../.gitbook/assets/golden_sword.png" alt="" data-size="line"> **12 сегментов**\
      `notched_12`
    * <img src="../../../.gitbook/assets/diamond_sword.png" alt="" data-size="line"> **20 сегментов**\
      `notched_20`

[^7]: **Эффект неба** `sky_effect`:

    * <img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> **Отсутствует**\
      `none`
    * <img src="../../../.gitbook/assets/light_gray_stained_glass.png" alt="" data-size="line"> **Туман**\
      `fog`
    * <img src="../../../.gitbook/assets/ink_sac.png" alt="" data-size="line"> **Тёмное небо**\
      `dark_sky`
    * <img src="../../../.gitbook/assets/gray_wool.png" alt="" data-size="line"> **Туман и тёмное небо**\
      `fog_and_dark_sky`

[^8]: **Тип достижения** `frame`:

    * <img src="../../../.gitbook/assets/gold_ingot.png" alt="" data-size="line"> **Обычное достижение**\
      `task`
    * <img src="../../../.gitbook/assets/diamond_sword.png" alt="" data-size="line"> **Испытание**\
      `goal`
    * <img src="../../../.gitbook/assets/golden_helmet.png" alt="" data-size="line"> **Цель**\
      `challenge`

[^9]: **Позиция** `position`:

    * <img src="../../../.gitbook/assets/iron_helmet.png" alt="" data-size="line"> **Сверху**\
      `header`
    * <img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> **Снизу**\
      `footer`

[^10]: **Источник звука** `source`:

    * <img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> **Общий**\
      `master`
    * <img src="../../../.gitbook/assets/music_disc_chirp.png" alt="" data-size="line"> **Музыка**\
      `music`
    * <img src="../../../.gitbook/assets/note_block.png" alt="" data-size="line"> **Музыкальные блоки**\
      `record`
    * <img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> **Погода**\
      `weather`
    * <img src="../../../.gitbook/assets/stone_bricks.png" alt="" data-size="line"> **Блоки**\
      `block`
    * <img src="../../../.gitbook/assets/totem_of_undying.png" alt="" data-size="line"> **Враждебные существа**\
      `hostile`
    * <img src="../../../.gitbook/assets/poppy.png" alt="" data-size="line"> **Дружелюбные существа**\
      `neutral`
    * <img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> **Игроки**\
      `player`
    * <img src="../../../.gitbook/assets/end_crystal.gif" alt="" data-size="line"> **Окружение**\
      `ambient`
    * <img src="../../../.gitbook/assets/observer.png" alt="" data-size="line"> **Голос/Речь**\
      `voice`

[^11]: **Тип обновления** `setting_mode`:

    * <img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> **Добавить**\
      `add`
    * <img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> **Установить**\
      `set`
    * <img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> **Удалить**\
      `remove`

[^12]: **Тип инвентаря** `inventory_type`:

    * <img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> **Сундук**\
      `chest`
    * <img src="../../../.gitbook/assets/dispenser.png" alt="" data-size="line"> **Раздатчик**\
      `dispenser`
    * <img src="../../../.gitbook/assets/dropper.png" alt="" data-size="line"> **Выбрасыватель**\
      `dropper`
    * <img src="../../../.gitbook/assets/furnace.png" alt="" data-size="line"> **Печь**\
      `furnace`
    * <img src="../../../.gitbook/assets/crafting_table.png" alt="" data-size="line"> **Верстак**\
      `workbench`
    * <img src="../../../.gitbook/assets/enchanting_table.png" alt="" data-size="line"> **Чародейский стол**\
      `enchanting`
    * <img src="../../../.gitbook/assets/brewing_stand.png" alt="" data-size="line"> **Зельеварка**\
      `brewing`
    * <img src="../../../.gitbook/assets/anvil.png" alt="" data-size="line"> **Наковальня**\
      `anvil`
    * <img src="../../../.gitbook/assets/smithing_table.png" alt="" data-size="line"> **Стол кузнеца**\
      `smithing`
    * <img src="../../../.gitbook/assets/beacon.png" alt="" data-size="line"> **Маяк**\
      `beacon`
    * <img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> **Воронка**\
      `hopper`
    * <img src="../../../.gitbook/assets/blast_furnace.png" alt="" data-size="line"> **Плавильная печь**\
      `blast_furnace`
    * <img src="../../../.gitbook/assets/smoker.png" alt="" data-size="line"> **Коптильня**\
      `smoker`
    * <img src="../../../.gitbook/assets/cartography_table.png" alt="" data-size="line"> **Стол картографа**\
      `cartography`
    * <img src="../../../.gitbook/assets/grindstone.png" alt="" data-size="line"> **Точило**\
      `grindstone`
    * <img src="../../../.gitbook/assets/stonecutter.gif" alt="" data-size="line"> **Камнерез**\
      `stonecutter`
    * <img src="../../../.gitbook/assets/crafter.png" alt="" data-size="line"> **Сборщик**\
      `crafter`

[^13]: **Позиция строки** `position`:

    * <img src="../../../.gitbook/assets/iron_door.png" alt="" data-size="line"> **Добавить строку сверху**\
      `top`
    * <img src="../../../.gitbook/assets/iron_trapdoor.png" alt="" data-size="line"> **Добавить строку снизу**\
      `button`

[^14]: **Позиция строки** `position`:

    * <img src="../../../.gitbook/assets/iron_door.png" alt="" data-size="line"> **Убрать строку сверху**\
      `top`
    * <img src="../../../.gitbook/assets/iron_trapdoor.png" alt="" data-size="line"> **Убрать строку снизу**\
      `button`

[^15]: **Исцелить игрока** `heal`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^16]: **Режим установки** `mode`:

    * <img src="../../../.gitbook/assets/stone.png" alt="" data-size="line"> **Установка**\
      `set`
    * <img src="../../../.gitbook/assets/stone.png" alt="" data-size="line"> **Прибавление**\
      `add`

[^17]: **Тип прибавления** `mode`:

    * <img src="../../../.gitbook/assets/potion_of_leaping.png" alt="" data-size="line"> **Как очки опыта**\
      `points`
    * <img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> **Как уровень**\
      `level`
    * <img src="../../../.gitbook/assets/turtle_scute.png" alt="" data-size="line"> **Как процент от уровня**\
      `level_percentage`

[^18]: **Тип установки** `mode`:

    * <img src="../../../.gitbook/assets/potion_of_leaping.png" alt="" data-size="line"> **Как очки опыта**\
      `points`
    * <img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> **Как уровень**\
      `level`
    * <img src="../../../.gitbook/assets/turtle_scute.png" alt="" data-size="line"> **Как процент от уровня**\
      `level_percentage`

[^19]: **Перезаписывать существующие эффекты** `overwrite`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^20]: **Показывать иконку эффекта** `show_icon`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^21]: **Показывать частицы** `particle_mode`:

    * <img src="../../../.gitbook/assets/custom_potion_610061.png" alt="" data-size="line"> **Да**\
      `regular`
    * <img src="../../../.gitbook/assets/custom_potion_616161.png" alt="" data-size="line"> **Прозрачными**\
      `ambient`
    * <img src="../../../.gitbook/assets/glass_bottle.png" alt="" data-size="line"> **Нет**\
      `none`

[^22]: **Блокировка состояния (время не будет изменяться)** `ticking_locked`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^23]: **Тип движения** `movement_type`:

    * <img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> **Ходьба**\
      `walk`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **Полёт**\
      `fly`

[^24]: **Тип атрибута** `attribute_type`:

    * <img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> **Максимальное здоровье**\
      `generic_max_health`
    * <img src="../../../.gitbook/assets/golden_apple.png" alt="" data-size="line"> **Максимальное поглощение**\
      `generic_max_absorption`
    * <img src="../../../.gitbook/assets/bone.png" alt="" data-size="line"> **Расстояние следования**\
      `generic_follow_range`
    * <img src="../../../.gitbook/assets/shield.png" alt="" data-size="line"> **Сопротивление отталкиванию**\
      `generic_knockback_resistance`
    * <img src="../../../.gitbook/assets/leather_boots.png" alt="" data-size="line"> **Скорость передвижения**\
      `generic_movement_speed`
    * <img src="../../../.gitbook/assets/elytra.png" alt="" data-size="line"> **Скорость полёта**\
      `generic_flying_speed`
    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Урон атаки**\
      `generic_attack_damage`
    * <img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> **Отталкивание атаки**\
      `generic_attack_knockback`
    * <img src="../../../.gitbook/assets/golden_sword.png" alt="" data-size="line"> **Скорость атаки**\
      `generic_attack_speed`
    * <img src="../../../.gitbook/assets/iron_chestplate.png" alt="" data-size="line"> **Очки защиты**\
      `generic_armor`
    * <img src="../../../.gitbook/assets/diamond_chestplate.png" alt="" data-size="line"> **Очки плотности защиты**\
      `generic_armor_toughness`
    * <img src="../../../.gitbook/assets/emerald.png" alt="" data-size="line"> **Удача рыбалки**\
      `generic_luck`
    * <img src="../../../.gitbook/assets/rabbit_foot.png" alt="" data-size="line"> **Сила прыжка**\
      `generic_jump_strength`
    * <img src="../../../.gitbook/assets/zombie_head.png" alt="" data-size="line"> **Шанс подкрепления зомби**\
      `zombie_spawn_reinforcements`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **Множитель урона от падения**\
      `generic_fall_damage_multiplier`
    * <img src="../../../.gitbook/assets/leather_boots.png" alt="" data-size="line"> **Безопасная высота падения**\
      `generic_safe_fall_distance`
    * <img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> **Масштаб**\
      `generic_scale`
    * <img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> **Высота шага**\
      `generic_step_height`
    * <img src="../../../.gitbook/assets/amethyst_shard.png" alt="" data-size="line"> **Гравитация**\
      `generic_gravity`
    * <img src="../../../.gitbook/assets/iron_pickaxe.png" alt="" data-size="line"> **Расстояние взаимодействия с блоками**\
      `player_block_interaction_range`
    * <img src="../../../.gitbook/assets/golden_axe.png" alt="" data-size="line"> **Расстояние взаимодействия с сущностями**\
      `player_entity_interaction_range`
    * <img src="../../../.gitbook/assets/diamond_pickaxe.png" alt="" data-size="line"> **Скорость ломания блока**\
      `player_block_break_speed`
    * <img src="../../../.gitbook/assets/campfire.png" alt="" data-size="line"> **Время горения**\
      `generic_burning_time`
    * <img src="../../../.gitbook/assets/tnt.png" alt="" data-size="line"> **Сопротивление отбрасыванию от взрыва**\
      `generic_explosion_knockback_resistance`
    * <img src="../../../.gitbook/assets/cobweb.png" alt="" data-size="line"> **Скорость передвижения по замедляющим блокам**\
      `generic_movement_efficiency`
    * <img src="../../../.gitbook/assets/glass_bottle.png" alt="" data-size="line"> **Воздух под водой**\
      `generic_oxygen_bonus`
    * <img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> **Скорость передвижения под водой**\
      `generic_water_movement_efficiency`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Скорость копания**\
      `player_mining_efficiency`
    * <img src="../../../.gitbook/assets/chainmail_leggings.png" alt="" data-size="line"> **Скорость передвижения крадясь**\
      `player_sneaking_speed`
    * <img src="../../../.gitbook/assets/water_bottle.png" alt="" data-size="line"> **Скорость копания под водой**\
      `player_submerged_mining_speed`
    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Коэффициент разящего удара**\
      `player_sweeping_damage_ratio`

[^25]: **Режим игры** `gamemode`:

    * <img src="../../../.gitbook/assets/oak_planks.png" alt="" data-size="line"> **Выживание**\
      `survival`
    * <img src="../../../.gitbook/assets/diamond_block.png" alt="" data-size="line"> **Творческий**\
      `creative`
    * <img src="../../../.gitbook/assets/gold_block.png" alt="" data-size="line"> **Приключение**\
      `adventure`
    * <img src="../../../.gitbook/assets/white_stained_glass.png" alt="" data-size="line"> **Наблюдатель**\
      `spectator`

[^26]: **Режим полёта** `flight_mode`:

    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **Учитывать режим игры**\
      `respect_gamemode`
    * <img src="../../../.gitbook/assets/elytra.png" alt="" data-size="line"> **Оставить изначальный**\
      `keep_original`

[^27]: **Может летать** `allow_flying`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^28]: **Может атаковать** `pvp`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^29]: **Выпадение предметов** `death_drops`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Выпадают**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не выпадают**\
      `false`

[^30]: **Сохранение инвентаря** `kept`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^31]: **Режим столкновения** `collidable`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Сталкивается с другими игроками**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не сталкивается с другими игроками**\
      `false`

[^32]: **Видимость** `default_visible`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Видимый**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Невидимый**\
      `false`

[^33]: **Отображение ника** `visible`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Отображать**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не отображать**\
      `false`

[^34]: **Мгновенное возрождение** `instant_respawn`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^35]: **Оставить текущий поворот** `keep_rotation`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^36]: **Сохранение инерции** `keep_velocity`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^37]: **Спешиться после телепортации** `dismount`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^38]: **Учитывать текущую инерцию** `increment`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^39]: **Ось запуска** `launch_axis`:

    * <img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"> **Все оси**\
      `yaw_and_pitch`
    * <img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> **Только по горизонтали**\
      `yaw`

[^40]: **Полёт** `is_flying`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^41]: **Полёт на элитрах** `is_gliding`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^42]: **Тип погоды** `weather_type`:

    * <img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> **Дождливая**\
      `downfall`
    * <img src="../../../.gitbook/assets/bucket.png" alt="" data-size="line"> **Солнечная**\
      `clear`

[^43]: **Состояние** `is_opened`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Открытый**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Закрытый**\
      `false`

[^44]: **Направление удара** `direction`:

    * <img src="../../../.gitbook/assets/bell.png" alt="" data-size="line"> **Вниз**\
      `down`
    *   <img src="../../../.gitbook/assets/bell.png" alt="" data-size="line"> **Север**

        `north`
    *   <img src="../../../.gitbook/assets/bell.png" alt="" data-size="line"> **Юг**

        `south`
    *   <img src="../../../.gitbook/assets/bell.png" alt="" data-size="line"> **Запад**

        `west`
    *   <img src="../../../.gitbook/assets/bell.png" alt="" data-size="line"> **Восток**

        `east`

[^45]: **Скрытие** `hide`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^46]: **Цвет луча** `color`:

    * <img src="../../../.gitbook/assets/magenta_concrete_powder_head.png" alt="" data-size="line"> **Светло-фиолетовый**\
      `light_purple`
    * <img src="../../../.gitbook/assets/purple_concrete_powder_head.png" alt="" data-size="line"> **Тёмно-фиолетовый**\
      `dark_purple`

[^47]: **Цвет свечения** `color`:

    * <img src="../../../.gitbook/assets/white_wool.png" alt="" data-size="line"> **Белый**\
      `white`
    * <img src="../../../.gitbook/assets/light_gray_wool.png" alt="" data-size="line"> **Светло-серый**\
      `gray`
    * <img src="../../../.gitbook/assets/gray_wool.png" alt="" data-size="line"> **Серый**\
      `dark_gray`
    * <img src="../../../.gitbook/assets/black_wool.png" alt="" data-size="line"> **Чёрный**\
      `black`
    * <img src="../../../.gitbook/assets/netherrack.png" alt="" data-size="line"> **Тёмно-красный**\
      `dark_red`
    * <img src="../../../.gitbook/assets/red_wool.png" alt="" data-size="line"> **Красный**\
      `red`
    * <img src="../../../.gitbook/assets/orange_wool.png" alt="" data-size="line"> **Золотой**\
      `gold`
    * <img src="../../../.gitbook/assets/yellow_wool.png" alt="" data-size="line"> **Жёлтый**\
      `yellow`
    * <img src="../../../.gitbook/assets/lime_wool.png" alt="" data-size="line"> **Зелёный**\
      `green`
    * <img src="../../../.gitbook/assets/green_wool.png" alt="" data-size="line"> **Тёмно-зелёный**\
      `dark_green`
    * <img src="../../../.gitbook/assets/dark_prismarine.png" alt="" data-size="line"> **Бирюзовый**\
      `dark_aqua`
    * <img src="../../../.gitbook/assets/prismarine.gif" alt="" data-size="line"> **Светло-синий**\
      `aqua`
    * <img src="../../../.gitbook/assets/light_blue_wool.png" alt="" data-size="line"> **Синий**\
      `blue`
    * <img src="../../../.gitbook/assets/blue_wool.png" alt="" data-size="line"> **Тёмно-синий**\
      `dark_blue`
    * <img src="../../../.gitbook/assets/purple_wool.png" alt="" data-size="line"> **Тёмно-фиолетовый**\
      `dark_purple`
    * <img src="../../../.gitbook/assets/magenta_wool.png" alt="" data-size="line"> **Фиолетовый**\
      `purple`

[^48]: **Свечение** `glow`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^49]: **Тип отображения частиц** `unit_of_measurement`:

    * <img src="../../../.gitbook/assets/stone_button.png" alt="" data-size="line"> **По количеству**\
      `points`
    * <img src="../../../.gitbook/assets/stick.png" alt="" data-size="line"> **По расстоянию**\
      `distance`

[^50]: **Тип угла** `angle_unit`:

    * <img src="../../../.gitbook/assets/sugar.png" alt="" data-size="line"> **Градусы**\
      `degrees`
    * <img src="../../../.gitbook/assets/glowstone_dust.png" alt="" data-size="line"> **Радианы**\
      `radians`

[^51]: **Тип куба** `type`:

    * <img src="../../../.gitbook/assets/tinted_glass.png" alt="" data-size="line"> **Заполненный**\
      `solid`
    * <img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> **Полный**\
      `hollow`
    * <img src="../../../.gitbook/assets/glass_pane.png" alt="" data-size="line"> **Каркас**\
      `wireframe`

[^52]: **Видимость для игрока** `visible_to_self`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Видно**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не видно**\
      `false`

[^53]: **Тип сервера скинов** `server_type`:

    * <img src="../../../.gitbook/assets/apple.png" alt="" data-size="line"> **Скин Mojang**\
      `mojang`
    * <img src="../../../.gitbook/assets/golden_apple.png" alt="" data-size="line"> **Скин JustMC**\
      `server`

[^54]: **Тип анимации** `animation`:

    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Получение урона**\
      `damage`
    * <img src="../../../.gitbook/assets/red_bed.png" alt="" data-size="line"> **Подъём с кровати**\
      `wake_up`
    * <img src="../../../.gitbook/assets/totem_of_undying.png" alt="" data-size="line"> **Тотем**\
      `totem`
    * <img src="../../../.gitbook/assets/guardian_head.png" alt="" data-size="line"> **Древний страж**\
      `jumpscare`

[^55]: **Отображаемая поза** `pose`:

    * <img src="../../../.gitbook/assets/armor_stand.png" alt="" data-size="line"> **Обычное состояние**\
      `standing`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Полёт на Элитрах**\
      `fall_flying`
    * <img src="../../../.gitbook/assets/red_bed.png" alt="" data-size="line"> **Лежание**\
      `sleeping`
    * <img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> **Плаванье**\
      `swimming`
    * <img src="../../../.gitbook/assets/trident.png" alt="" data-size="line"> **Использование Тягуна**\
      `spin_attack`
    * <img src="../../../.gitbook/assets/chainmail_leggings.png" alt="" data-size="line"> **Приседание**\
      `crouching`
    * <img src="../../../.gitbook/assets/iron_boots.png" alt="" data-size="line"> **Длинный прыжок**\
      `long_jumping`
    * <img src="../../../.gitbook/assets/skeleton_skull.png" alt="" data-size="line"> **Смерть**\
      `dying`
    * <img src="../../../.gitbook/assets/frogspawn.png" alt="" data-size="line"> **Кваканье (для Жаб)**\
      `croaking`
    * <img src="../../../.gitbook/assets/ochre_froglight.png" alt="" data-size="line"> **Использование языка (для Жаб)**\
      `using_tongue`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Сидение**\
      `sitting`
    * <img src="../../../.gitbook/assets/goat_horn.png" alt="" data-size="line"> **Рёв (для Хранителя)**\
      `roaring`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Нюханье (для Хранителя)**\
      `sniffing`
    * <img src="../../../.gitbook/assets/sculk_sensor.gif" alt="" data-size="line"> **Появление из земли (для Хранителя)**\
      `emerging`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Зарывание в землю (для Хранителя)**\
      `digging`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Скольжение (для Вихря)**\
      `sliding`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Выстреливание (для Вихря)**\
      `shooting`
    * <img src="../../../.gitbook/assets/golden_pickaxe.png" alt="" data-size="line"> **Вдыхание (для Вихря)**\
      `inhaling`

[^56]: **Блокировка позы** `locked`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^57]: **Тип руки** `hand_type`:

    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Главная**\
      `main`
    * <img src="../../../.gitbook/assets/shield.png" alt="" data-size="line"> **Второстепенная**\
      `off`

[^58]: **Установить визуальный огонь** `visual_fire`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`
