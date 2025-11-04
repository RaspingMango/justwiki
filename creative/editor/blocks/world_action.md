---
description: Выполняет действия, связанные с миром.
---

# Действие над миром

<figure><img src="../../../.gitbook/assets/netherrack.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `game_action`

***

## Использование

Поставьте блок в строку и нажмите <kbd>ПКМ</kbd> по нему, чтобы открыть меню опций блока. Перейдите в нужную категорию и выберите действие, которое необходимо выполнить.

При выборе действия, над его блоком может появиться хранилище (по умолчанию: сундук), в котором содержатся [аргументы](../arguments/) действия.

### Опции

{% tabs fullWidth="false" %}
{% tab title="Создание сущностей" %}
<img src="../../../.gitbook/assets/sheep_spawn_egg.png" alt="" data-size="line"> **Действия, которые создают сущностей в мире.**

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/polar_bear_spawn_egg.png" alt="" data-size="line"> <strong>Создать моба</strong><br><code>game_spawn_mob</code></td><td>Создаёт моба в указанном местоположении с выбранными параметрами.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Тип моба</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество здоровья</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/potion.md"><img src="../../../.gitbook/assets/dragon_breath.png" alt="" data-size="line"></a> <strong>Эффекты</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет в основной руке</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Головной убор</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Нагрудник</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Поножи</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Ботинки</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет во второстепенной руке</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Стандартное снаряжение</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> <strong>Создать предмет</strong><br><code>game_spawn_item</code></td><td>Создаёт предмет в указанном местоположении с выбранными параметрами.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет для создания</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Задать движение предмета при создании</strong> <a data-footnote-ref href="#user-content-fn-2"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Смогут ли подбирать предмет мобы</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Смогут ли подбирать предмет игроки</strong> <a data-footnote-ref href="#user-content-fn-4"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/oak_boat.png" alt="" data-size="line"> <strong>Создать транспорт</strong><br><code>game_spawn_vehicle</code></td><td>Создаёт транспорт в указанном местоположении с выбранными параметрами.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Тип транспорта</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong></td></tr><tr><td><img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> <strong>Создать сферу опыта</strong><br><code>game_spawn_experience_orb</code></td><td>Создаёт сферу опыта в указанном местоположении с выбранными параметрами.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество опыта</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong></td></tr><tr><td><img src="../../../.gitbook/assets/tnt_minecart.png" alt="" data-size="line"> <strong>Создать взрыв</strong><br><code>game_create_explosion</code></td><td>Создаёт взрыв в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Сила взрыва (от 0 до 4)</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Появление огня</strong> <a data-footnote-ref href="#user-content-fn-5"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Разрушение блоков</strong> <a data-footnote-ref href="#user-content-fn-6"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/tnt.png" alt="" data-size="line"> <strong>Создать подожжённый динамит</strong><br><code>game_spawn_primed_tnt</code></td><td>Создаёт подожжённый динамит в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Мощность динамита (от 0 до 4)</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время задержки взрыва</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок для маскировки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/donkey_spawn_egg.png" alt="" data-size="line"> <strong>Создать челюсти заклинателя</strong><br><code>game_spawn_evoker_fangs</code></td><td>Создаёт челюсти заклинателя в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong></td></tr><tr><td><img src="../../../.gitbook/assets/firework_rocket.png" alt="" data-size="line"> <strong>Создать фейерверк</strong><br><code>game_launch_firework</code></td><td>Запускает фейерверк в указанном местоположении.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Фейерверк для создания</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Движение</strong> <a data-footnote-ref href="#user-content-fn-7"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Мгновенный взрыв</strong> <a data-footnote-ref href="#user-content-fn-8"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> <strong>Запустить снаряд</strong><br><code>game_launch_projectile</code></td><td>Запускает снаряд в указанном местоположении.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Снаряд для запуска</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место запуска</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Скорость снаряда</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Отклонение снаряда (0, чтобы снаряд летел ровно)</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя снаряда</strong><br><a href="../arguments/"><img src="../../../.gitbook/assets/white_dye.png" alt="" data-size="line"></a> <strong>След, который будет оставаться за снарядом</strong></td></tr><tr><td><img src="../../../.gitbook/assets/shulker_shell.png" alt="" data-size="line"> <strong>Создать снаряд Шалкера</strong><br><code>game_spawn_shulker_bullet</code></td><td>Создаёт снаряд Шалкера в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong></td></tr><tr><td><img src="../../../.gitbook/assets/golden_axe.png" alt="" data-size="line"> <strong>Создать молнию</strong><br><code>game_spawn_lightning_bolt</code></td><td>Создаёт молнию в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong></td></tr><tr><td><img src="../../../.gitbook/assets/lingering_water_bottle.png" alt="" data-size="line"> <strong>Создать облако туманного зелья</strong><br><code>game_spawn_effect_cloud</code></td><td>Создаёт облако туманного зелья, которое пропитывает эффектами сущностей в нём.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/potion.md"><img src="../../../.gitbook/assets/dragon_breath.png" alt="" data-size="line"></a> <strong>Эффекты зелья</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Радиус облака</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность</strong><br><a href="../arguments/particle.md"><img src="../../../.gitbook/assets/phantom_membrane.png" alt="" data-size="line"></a> <strong>Частицы облака</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong></td></tr><tr><td><img src="../../../.gitbook/assets/sand.png" alt="" data-size="line"> <strong>Создать падающий блок</strong><br><code>game_spawn_falling_block</code></td><td>Создаёт падающий блок в указанном местоположении.</td><td><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок для создания</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Должен исчезать</strong> <a data-footnote-ref href="#user-content-fn-9"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/armor_stand.png" alt="" data-size="line"> <strong>Создать стойку для брони</strong><br><code>game_spawn_armor_stand</code></td><td>Создаёт стойку для брони в указанном местоположении.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Головной убор</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Нагрудник</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Поножи</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Ботинки</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет в правой руке</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет в левой руке</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Установить гравитацию</strong> <a data-footnote-ref href="#user-content-fn-10"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим маркера</strong> <a data-footnote-ref href="#user-content-fn-11"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сделать маленьким</strong> <a data-footnote-ref href="#user-content-fn-12"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Отображение рук</strong> <a data-footnote-ref href="#user-content-fn-13"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Отображение плиты</strong> <a data-footnote-ref href="#user-content-fn-14"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Невидимость</strong> <a data-footnote-ref href="#user-content-fn-15"><strong><code>-></code></strong></a><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя стойки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/end_crystal.gif" alt="" data-size="line"> <strong>Создать кристалл Энда</strong><br><code>game_spawn_end_crystal</code></td><td>Создаёт кристалл Энда в указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Создание фундамента</strong> <a data-footnote-ref href="#user-content-fn-16"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/ender_eye.png" alt="" data-size="line"> <strong>Создать око Энда</strong><br><code>game_spawn_eye_of_ender</code></td><td>Создаёт в указанном местоположении око Энда, которое будет двигаться в сторону цели.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Цель</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность жизни</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>По окончанию</strong> <a data-footnote-ref href="#user-content-fn-17"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/dark_oak_sign.png" alt="" data-size="line"> <strong>Создать визуализатор текста</strong><br><code>game_spawn_text_display</code></td><td>Создаёт визуализатор текста на указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Объединение текста</strong> <a data-footnote-ref href="#user-content-fn-18"><strong><code>-></code></strong></a><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Отображаемый текст</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glow_item_frame.png" alt="" data-size="line"> <strong>Создать визуализатор предмета</strong><br><code>game_spawn_item_display</code></td><td>Создаёт визуализатор предмета на указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Отображаемый предмет</strong></td></tr><tr><td><img src="../../../.gitbook/assets/bricks.png" alt="" data-size="line"> <strong>Создать визуализатор блока</strong><br><code>game_spawn_block_display</code></td><td>Создаёт визуализатор блока на указанном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Отображаемый блок</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> <strong>Создать сущность взаимодействия</strong><br><code>game_spawn_interaction_entity</code></td><td>Создаёт сущность взаимодействия на указанном местоположении.<br><br>» Определяйте взаимодействие при помощи событий атаки и клика по сущности.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Место создания</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Горизонтальный размер</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Вертикальный размер</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Отзывчивость</strong> <a data-footnote-ref href="#user-content-fn-19"><strong><code>-></code></strong></a></td></tr></tbody></table>
{% endtab %}

{% tab title="Действия с блоками" %}
<img src="../../../.gitbook/assets/bricks.png" alt="" data-size="line"> **Действия, которые взаимодействуют с миром и блоками.**

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/oak_log.png" alt="" data-size="line"> <strong>Установить блок</strong><br><code>game_set_block</code></td><td>Устанавливает выбранный тип блока на выбранных местоположениях.</td><td><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположения установки блока</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Обновлять блоки вокруг</strong> <a data-footnote-ref href="#user-content-fn-20"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/oak_wood.png" alt="" data-size="line"> <strong>Установить блоки в регионе</strong><br><code>game_set_region</code></td><td>Устанавливает выбранный тип блока на весь выбранный регион.</td><td><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блок</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Угол региона</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Противоположный угол региона</strong></td></tr><tr><td><img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> <strong>Заменить блоки в регионе</strong><br><code>game_replace_blocks_in_region</code></td><td>Заменяет одни блоки на другие в выбранном регионе.</td><td><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Блоки для замены</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Угол региона</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Противоположный угол региона</strong><br><a href="../arguments/block.md"><img src="../../../.gitbook/assets/chiseled_stone_bricks.png" alt="" data-size="line"></a> <strong>Новый блок</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glass_pane.png" alt="" data-size="line"> <strong>Очистить регион</strong><br><code>game_clear_region</code></td><td>Удаляет все блоки в регионе.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Угол региона</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Противоположный угол региона</strong></td></tr><tr><td><img src="../../../.gitbook/assets/netherite_scrap.png" alt="" data-size="line"> <strong>Клонировать блоки региона</strong><br><code>game_clone_region</code></td><td>Клонирует регион на выбранное местоположение.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Угол региона</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Противоположный угол региона</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение копирования</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение для вставки</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Игнорировать воздух</strong> <a data-footnote-ref href="#user-content-fn-21"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Клонировать существ</strong> <a data-footnote-ref href="#user-content-fn-22"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> <strong>Сломать блок</strong><br><code>game_break_block</code></td><td>Разрушает блоки на указанных местоположениях, как если бы это сделал игрок в режиме выживания нужным инструментом.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположения блоков</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Инструмент</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Выпадение опыта</strong> <a data-footnote-ref href="#user-content-fn-23"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/cocoa_beans.png" alt="" data-size="line"> <strong>Установить возраст</strong><br><code>game_set_age</code></td><td>Устанавливает возраст блока на выбранном местоположении.<br><br>Работает с:<br>» Любыми блоками, которые могут иметь возраст</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Тики</strong></td></tr><tr><td><img src="../../../.gitbook/assets/bone_meal.png" alt="" data-size="line"> <strong>Удобрить блок</strong><br><code>game_bone_meal_block</code></td><td>Удобряет блок на выбранном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество попыток удобрить</strong></td></tr><tr><td><img src="../../../.gitbook/assets/oak_sapling.png" alt="" data-size="line"> <strong>Создать дерево</strong><br><code>game_generate_tree</code></td><td>Создаёт дерево на выбранном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение дерева</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип дерева</strong> <a data-footnote-ref href="#user-content-fn-24"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/wheat_seeds.png" alt="" data-size="line"> <strong>Установить стадию роста блока</strong><br><code>game_block_growth</code></td><td>Устанавливает стадию роста для блока на выбранном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Стадия роста</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип роста</strong> <a data-footnote-ref href="#user-content-fn-25"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/dispenser.png" alt="" data-size="line"> <strong>Заполнить контейнер</strong><br><code>game_fill_container</code></td><td>Заполняет контейнер на выбранном местоположении указанными предметами.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для заполнения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/chest_minecart.png" alt="" data-size="line"> <strong>Установить предметы в контейнере</strong><br><code>game_set_container</code></td><td>Устанавливает указанные предметы в контейнер на выбранном местоположении.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> <strong>Установить предмет в слот контейнера</strong><br><code>game_set_item_in_container_slot</code></td><td>Установить предмет в указанный слот контейнера на выбранном местоположении.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Номер слота</strong></td></tr><tr><td><img src="../../../.gitbook/assets/diamond_chestplate.png" alt="" data-size="line"> <strong>Заменить предметы в контейнере</strong><br><code>game_replace_container_items</code></td><td>Заменяет указанные предметы в контейнере на выбранном местоположении на определённый предмет.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Заменяемые предметы</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/map.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Заменяющий предмет</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество предметов для замены</strong></td></tr><tr><td><img src="../../../.gitbook/assets/hopper_minecart.png" alt="" data-size="line"> <strong>Удалить предметы из контейнера</strong><br><code>game_remove_container_items</code></td><td>Удаляет из контейнера на выбранном местоположении указанные предметы.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы</strong></td></tr><tr><td><img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> <strong>Очистить предметы в контейнере</strong><br><code>game_clear_container_items</code></td><td>Очищает указанные предметы из контейнера.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы</strong></td></tr><tr><td><img src="../../../.gitbook/assets/tnt_minecart.png" alt="" data-size="line"> <strong>Очистить контейнер</strong><br><code>game_clear_container</code></td><td>Удаляет все предметы из контейнера на выбранном местоположении.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong></td></tr><tr><td><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Установить имя контейнеру</strong><br><code>game_set_container_name</code></td><td>Устанавливает имя контейнеру на выбранном местоположении.<br><br>Работает с:<br>» Любыми контейнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя контейнера</strong></td></tr><tr><td><img src="../../../.gitbook/assets/tripwire_hook.png" alt="" data-size="line"> <strong>Установить ключ контейнера</strong><br><code>game_set_container_lock</code></td><td>Устанавливает определённый ключ контейнеру на выбранном местоположении.<br><br>» В качестве ключа контейнера служит любой предмет с определённым именем.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение контейнера</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имя ключа контейнера</strong></td></tr><tr><td><img src="../../../.gitbook/assets/oak_sign.png" alt="" data-size="line"> <strong>Установить текст таблички</strong><br><code>game_set_sign_text</code></td><td>Устанавливает текст таблички на выбранном местоположении.<br><br>Работает с:<br>» Табличками</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение таблички</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст для установки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Строка</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сторона таблички</strong> <a data-footnote-ref href="#user-content-fn-26"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/crimson_sign.png" alt="" data-size="line"> <strong>Установить цвет текста таблички</strong><br><code>game_set_sign_text_color</code></td><td>Устанавливает цвет текста таблички на выбранном местоположении.<br><br>Работает с:<br>» Табличками</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение таблички</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сторона таблички</strong> <a data-footnote-ref href="#user-content-fn-26"><strong><code>-></code></strong></a><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Цвет текста</strong> <a data-footnote-ref href="#user-content-fn-27"><strong><code>-></code></strong></a><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Свечение текста</strong> <a data-footnote-ref href="#user-content-fn-28"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/honeycomb.png" alt="" data-size="line"> <strong>Установить вощённость таблички</strong><br><code>game_set_sign_waxed</code></td><td>Устанавливает вощённость таблички на выбранном местоположении.<br><br>Работает с:<br>» Табличками</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение таблички</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Вощённость</strong> <a data-footnote-ref href="#user-content-fn-29"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> <strong>Установить голову игрока</strong><br><code>game_set_player_head</code></td><td>Устанавливает голову игрока на выбранном местоположении.<br><br>Работает с:<br>» Головами игроков</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение головы</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Значение</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип значения</strong> <a data-footnote-ref href="#user-content-fn-30"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/furnace.png" alt="" data-size="line"> <strong>Установить время готовки печи</strong><br><code>game_set_furnace_cook_time</code></td><td>Устанавливает время готовки печи на выбранном местоположении.<br><br>Работает с:<br>» Печками<br>» Плавильнями<br>» Коптильнями</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение печи</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время готовки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/campfire.png" alt="" data-size="line"> <strong>Установить предмет в костёр</strong><br><code>game_set_campfire_item</code></td><td>Устанавливает предмет в костёр на выбранном местоположении.<br><br>Работает с:<br>» Кострами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение костра</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время готовки</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Слот</strong> <a data-footnote-ref href="#user-content-fn-31"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/lectern.png" alt="" data-size="line"> <strong>Установить книгу в кафедру</strong><br><code>game_set_lectern_book</code></td><td>Устанавливает книгу в кафедру на выбранном местоположении.<br><br>Работает с:<br>» Кафедрами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение кафедры</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Книга для установки</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Страница</strong></td></tr><tr><td><img src="../../../.gitbook/assets/suspicious_sand.png" alt="" data-size="line"> <strong>Установить предмет в подозрительный блок</strong><br><code>game_set_brushable_block_item</code></td><td>Устанавливает предмет в подозрительный блок (песок, гравий) на выбранном местоположении.<br><br>Работает с:<br>» Подозрительным песком<br>» Подозрительным гравием</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предмет</strong></td></tr><tr><td><img src="../../../.gitbook/assets/decorated_pot.png" alt="" data-size="line"> <strong>Установить украшение вазы</strong><br><code>game_set_decorate_pot_sherd</code></td><td>Устанавливает указанный черепок выбранной стороне вазы на указанном местоположении.<br><br>Работает с:<br>» Вазами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение вазы</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Черепок для установки</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сторона вазы</strong> <a data-footnote-ref href="#user-content-fn-32"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/sculk_catalyst.png" alt="" data-size="line"> <strong>Продлить скалк-заражение к местоположению</strong><br><code>game_bloom_skulk_catalyst</code></td><td>Продлевает скалк-заражение к местоположению.<br><br>Работает с:<br>» Скалк-катализаторами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение скалкового катализатора</strong><br><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Конечное местоположение</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Сила заражения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/sculk_shrieker.gif" alt="" data-size="line"> <strong>Установить скалк-крикуну возможность призыва</strong><br><code>game_set_sculk_shrieker_can_summon</code></td><td>Устанавливает указанному скалк-крикуну возможность призыва Вардена.<br><br>Работает с:<br>» Скалк-крикунами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение скалк-крикуна</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Возможность призыва</strong> <a data-footnote-ref href="#user-content-fn-33"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/sculk_shrieker.gif" alt="" data-size="line"> <strong>Установить состояние скалк-крикуну</strong><br><code>game_set_sculk_shrieker_shrieking</code></td><td>Устанавливает указанному скалк-крикуну состояние.<br><br>Работает с:<br>» Скалк-крикунами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение скалк-крикуна</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Состояние</strong> <a data-footnote-ref href="#user-content-fn-34"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/warden_spawn_egg.png" alt="" data-size="line"> <strong>Установить скалк-крикуну уровень опасности</strong><br><code>game_set_sculk_shrieker_warning_level</code></td><td>Устанавливает указанному скалк-крикуну уровень опасности.<br><br>Работает с:<br>» Скалк-крикунами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение скалк-крикуна</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Уровень опасности</strong></td></tr><tr><td><img src="../../../.gitbook/assets/redstone_lamp.png" alt="" data-size="line"> <strong>Активировать блок</strong><br><code>game_set_block_powered</code></td><td>Активирует блок на выбранном местоположении.<br><br>Работает с:<br>» Активируемыми блоками</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Активация</strong> <a data-footnote-ref href="#user-content-fn-35"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/redstone.png" alt="" data-size="line"> <strong>Установить силу редстоун-сигнала</strong><br><code>game_set_block_analogue_power</code></td><td>Устанавливает на выбранном местоположении определённую силу сигнала.<br><br>Работает с:<br>» Активируемыми блоками</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Новая сила сигнала</strong></td></tr><tr><td><img src="../../../.gitbook/assets/spawner.png" alt="" data-size="line"> <strong>Установить сущность в спавнере</strong><br><code>game_set_spawner_entity</code></td><td>Устанавливает спавнеру на выбранном местоположении сущность внутри.<br><br>Работает с:<br>» Спавнерами</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение спавнера</strong><br><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Яйцо призыва сущности</strong></td></tr><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Вызвать случайный тик</strong><br><code>game_random_tick_block</code></td><td>Вызывает случайный тик на выбранном местоположении.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество тиков</strong></td></tr><tr><td><img src="../../../.gitbook/assets/sand.png" alt="" data-size="line"> <strong>Обновить смежные блоки</strong><br><code>game_update_block</code></td><td>Обновляет соседние блоки на указанном местоположении, если блок на местоположении не является воздухом. Сам по себе блок на местоположении не обновляется, но может обновиться от соседних.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение</strong></td></tr><tr><td><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Установить параметр блоку</strong><br><code>game_set_block_single_data</code></td><td>Устанавливает указанный параметр блоку на местоположении на заданное значение.</td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположение блока</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Изменяемый параметр</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Новое значение</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Действия с событиями" %}
<img src="../../../.gitbook/assets/diamond.png" alt="" data-size="line"> **Действия, которые изменяют поведение события.**

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Отмена события</strong><br><code>game_cancel_event</code></td><td>Отменяет начальное событие, которое вызвало этот код.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> <strong>Возврат события</strong><br><code>game_uncancel_event</code></td><td>Возвращает отмену события, которое вызвало этот код.</td><td></td></tr><tr><td><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> <strong>Убрать сообщение события</strong><br><code>game_hide_event_message</code></td><td>Убирает отправку сообщения события, которое вызвало этот код.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-mira"><img src="../../../.gitbook/assets/potato.png" alt="" data-size="line"> <strong>Игрок зашёл в мир</strong></a><br>» Событием <a href="player_event.md#sobytiya-mira"><img src="../../../.gitbook/assets/poisonous_potato.png" alt="" data-size="line"> <strong>Игрок вышел из мира</strong></a><br>» Событием <a href="player_event.md#sobytiya-smerti"><img src="../../../.gitbook/assets/redstone.png" alt="" data-size="line"> <strong>Игрок умирает</strong></a></td><td><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Убрать сообщение</strong> <a data-footnote-ref href="#user-content-fn-36"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> <strong>Установить урон события</strong><br><code>game_set_event_damage</code></td><td>Устанавливает урон, связанный с этим событием.<br><br>Работает с:<br>» Событиями урона</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество урона</strong></td></tr><tr><td><img src="../../../.gitbook/assets/slime_block.png" alt="" data-size="line"> <strong>Установить вектор отталкивания события</strong><br><code>game_set_event_knockback_vector</code></td><td>Устанавливает вектор отталкивания, связанный с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-urona"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Игрок отталкивается</strong></a><br>» Событием <a href="entity_event.md#opcii"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Сущность отталкивается</strong></a></td><td><a href="../arguments/vector.md"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"></a> <strong>Вектор отталкивания</strong></td></tr><tr><td><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"> <strong>Установить вектор скорости события</strong><br><code>game_set_event_velocity</code></td><td>Устанавливает вектор скорости, связанный с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-peredvizheniya"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"> <strong>Игрок изменил вектор скорости</strong></a></td><td><a href="../arguments/vector.md"><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"></a> <strong>Вектор скорости</strong></td></tr><tr><td><img src="../../../.gitbook/assets/water_bottle.png" alt="" data-size="line"> <strong>Установить лечение события</strong><br><code>game_set_event_heal</code></td><td>Устанавливает значение лечения, связанное с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-urona"><img src="../../../.gitbook/assets/splash_potion_of_healing.png" alt="" data-size="line"> <strong>Игрок восстанавливает здоровье</strong></a><br>» Событием <a href="entity_event.md#opcii"><img src="../../../.gitbook/assets/splash_potion_of_healing.png" alt="" data-size="line"> <strong>Сущность исцеляется</strong></a></td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество лечения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/rotten_flesh.png" alt="" data-size="line"> <strong>Установить истощение события</strong><br><code>game_set_event_exhaustion</code></td><td>Устанавливает значение истощения, связанное с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-urona"><img src="../../../.gitbook/assets/rotten_flesh.png" alt="" data-size="line"> <strong>Игрок истощается</strong></a></td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество истощения</strong></td></tr><tr><td><img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> <strong>Установить опыт события</strong><br><code>game_set_event_experience</code></td><td>Устанавливает значение опыта, связанное с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-predmetov"><img src="../../../.gitbook/assets/fishing_rod.png" alt="" data-size="line"> <strong>Игрок рыбачит</strong></a><br>» Событием <a href="player_event.md#sobytiya-vzaimodeistviya-s-sushnostyu"><img src="../../../.gitbook/assets/experience_bottle.gif" alt="" data-size="line"> <strong>Игрок поднял сферу опыта</strong></a><br>» Событиями убийства</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Количество опыта</strong></td></tr><tr><td><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Установить конечный слот события</strong><br><code>game_set_event_target_slot</code></td><td>Устанавливает конечный слот, связанный с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-inventarya"><img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> <strong>Игрок находит предмет в инвентаре</strong></a></td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Слот для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/chest.png" alt="" data-size="line"> <strong>Установить начальный слот события</strong><br><code>game_set_event_source_slot</code></td><td>Устанавливает начальный слот, связанный с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-inventarya"><img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> <strong>Игрок находит предмет в инвентаре</strong></a></td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Слот для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/bow.png" alt="" data-size="line"> <strong>Установить снаряд события</strong><br><code>game_set_event_projectile</code></td><td>Заменяет снаряд, который связан с этим событием.</td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Снаряд</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Отображаемое имя снаряда</strong></td></tr><tr><td><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"> <strong>Установить звук события</strong><br><code>game_set_event_sound</code></td><td>Устанавливает звук для проигрывания, связанный с этим событием, заменяя изначальный.</td><td><a href="../arguments/sound.md"><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" data-size="line"></a> <strong>Проигрываемый звук</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glass.png" alt="" data-size="line"> <strong>Очистить взорванные блоки</strong><br><code>game_clear_exploded_blocks</code></td><td>Возвращает взорванные блоки в исходное положение.<br><br>Работает с:<br>» Событием <a href="world_event.md#sobytiya-blokov"><img src="../../../.gitbook/assets/wither_skeleton_skull.png" alt="" data-size="line"> <strong>Сущность взрывается</strong></a><br>» Событием <a href="world_event.md#sobytiya-blokov"><img src="../../../.gitbook/assets/end_crystal.gif" alt="" data-size="line"> <strong>Блок взрывается</strong></a></td><td><a href="../arguments/location.md"><img src="../../../.gitbook/assets/paper.png" alt="" data-size="line"></a> <strong>Местоположения блоков</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glow_item_frame.png" alt="" data-size="line"> <strong>Установить предмет события</strong><br><code>game_set_event_item</code></td><td>Устанавливает предмет, связанный с этим событием.<br><br>Работает с:<br>» Событием <a href="world_event.md#sobytiya-blokov"><img src="../../../.gitbook/assets/dispenser.png" alt="" data-size="line"> <strong>Раздатчик надевает броню</strong></a><br>» Событием <a href="world_event.md#sobytiya-blokov"><img src="../../../.gitbook/assets/dropper.png" alt="" data-size="line"> <strong>Блок выбрасывает предмет</strong></a><br>» Событием <a href="player_event.md#sobytiya-predmetov"><img src="../../../.gitbook/assets/cooked_chicken.png" alt="" data-size="line"> <strong>Игрок употребляет предмет</strong></a><br>» Событием <a href="player_event.md#sobytiya-inventarya"><img src="../../../.gitbook/assets/crafting_table.png" alt="" data-size="line"> <strong>Игрок крафтит предмет</strong></a><br>» Событием <a href="player_event.md#sobytiya-predmetov"><img src="../../../.gitbook/assets/sugar.png" alt="" data-size="line"> <strong>Игрок выбрасывает предмет</strong></a><br>» Событием <a href="entity_event.md#opcii"><img src="../../../.gitbook/assets/sugar.png" alt="" data-size="line"> <strong>Существо выбрасывает предмет</strong></a><br>» Событием <a href="entity_event.md#opcii"><img src="../../../.gitbook/assets/glowstone_dust.png" alt="" data-size="line"> <strong>Существо поднимает предмет</strong></a><br>» Событием <a href="player_event.md#sobytiya-inventarya"><img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> <strong>Игрок кликает в своём инвентаре</strong></a><br>» Событием <a href="player_event.md#sobytiya-inventarya"><img src="../../../.gitbook/assets/fishing_rod.png" alt="" data-size="line"> <strong>Игрок кликает в инвентаре</strong></a><br>» Событием <a href="player_event.md#sobytiya-predmetov"><img src="../../../.gitbook/assets/writable_book.png" alt="" data-size="line"> <strong>Игрок изменяет книгу</strong></a><br>» Событием <a href="player_event.md#sobytiya-vzaimodeistviya-s-sushnostyu"><img src="../../../.gitbook/assets/arrow.png" alt="" data-size="line"> <strong>Игрок поднял снаряд</strong></a><br>» Событием <a href="entity_event.md#opcii"><img src="../../../.gitbook/assets/uncraftable_splash_potion.png" alt="" data-size="line"> <strong>Ведьма кидает зелье</strong></a></td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Новый предмет события</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glow_item_frame.png" alt="" data-size="line"> <strong>Установить предметы события</strong><br><code>game_set_event_items</code></td><td>Устанавливает предметы связанные с этим событием.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-inventarya"><img src="../../../.gitbook/assets/hopper.png" alt="" data-size="line"> <strong>Игрок находит предмет в инвентаре</strong></a></td><td><a href="../arguments/item.md"><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"></a> <strong>Предметы для установки</strong></td></tr><tr><td><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Установить теги в полученную информацию</strong><br><code>game_set_event_uery_info</code></td><td>Устанавливает дополнительные теги в полученную отладочную информацию, которые скопируются в буфер обмена, если событие не отменено.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-vzaimodeistviya-s-mirom"><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Игрок получает информацию о блоке</strong></a><br>» Событием <a href="player_event.md#sobytiya-vzaimodeistviya-s-sushnostyu"><img src="../../../.gitbook/assets/name_tag.png" alt="" data-size="line"> <strong>Игрок получает информацию о сущности</strong></a><br><br>» Изменения касаются только дополнительной информации.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Дополнительные теги</strong></td></tr><tr><td><img src="../../../.gitbook/assets/leather_boots.png" alt="" data-size="line"> <strong>Разрешить передвижение</strong><br><code>game_set_event_move_allowed</code></td><td>Разрешает передвижение, если оно не удалось.<br><br>Работает с:<br>» Событием <a href="player_event.md#sobytiya-peredvizheniya"><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Игроку не удалось передвинуться</strong></a></td><td><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Разрешить передвижение</strong> <a data-footnote-ref href="#user-content-fn-37"><strong><code>-></code></strong></a></td></tr></tbody></table>
{% endtab %}

{% tab title="Действия со скорбордами" %}
<img src="../../../.gitbook/assets/knowledge_book.png" alt="" data-size="line"> **Действия, которые создают или изменяют скорборды.**

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/knowledge_book.png" alt="" data-size="line"> <strong>Создать скорборд</strong><br><code>game_create_scoreboard</code></td><td>Создаёт скорборд с определённым ID. Чтобы отобразить скорборд игроку, используйте действие <a href="player_action.md#raznoe"><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Показать скорборд</strong></a>.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Заголовок</strong></td></tr><tr><td><img src="../../../.gitbook/assets/structure_void.png" alt="" data-size="line"> <strong>Удалить скорборд</strong><br><code>game_remove_scoreboard</code></td><td>Удаляет указанный скорборд.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong></td></tr><tr><td><img src="../../../.gitbook/assets/painting.png" alt="" data-size="line"> <strong>Изменить заголовок скорборда</strong><br><code>game_set_scoreboard_title</code></td><td>Изменяет заголовок указанного скорборда.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Новый заголовок</strong></td></tr><tr><td><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> <strong>Установить значение скорборда</strong><br><code>game_set_scoreboard_score</code></td><td>Устанавливает значение указанной строке в скорборде.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID линии</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Счёт</strong></td></tr><tr><td><img src="../../../.gitbook/assets/writable_book.png" alt="" data-size="line"> <strong>Установить линию в скорборде</strong><br><code>game_set_scoreboard_line</code></td><td>Устанавливает линию в скорборде.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID линии</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Отображаемый текст</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Значение</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Формат текста</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип формата</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line"> <strong>Установить отображаемый текст линии скорборда</strong><br><code>game_set_scoreboard_line_display</code></td><td>Устанавливает указанной линии скорборда отображаемый текст.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID линии</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Отображаемый текст</strong></td></tr><tr><td><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> <strong>Установить формат текста линии скорборда</strong><br><code>game_set_scoreboard_line_format</code></td><td>Устанавливает форматирование текста указанной линии скорборда.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID линии</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Формат текста</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип формата</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"> <strong>Установить форматирование значений скорборда</strong><br><code>game_set_scoreboard_number_format</code></td><td>Устанавливает форматирование значений для скорборда.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Формат текста</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип формата</strong> <a data-footnote-ref href="#user-content-fn-38"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/ink_sac.png" alt="" data-size="line"> <strong>Удалить значение скорборда по тексту</strong><br><code>game_remove_scoreboard_score_by_name</code></td><td>Удаляет значение указанной строки в скорборде.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID линии</strong></td></tr><tr><td><img src="../../../.gitbook/assets/glow_ink_sac.png" alt="" data-size="line"> <strong>Удалить значение скорборда по счёту</strong><br><code>game_remove_scoreboard_score_by_score</code></td><td>Удаляет значение указанного скорборда по счёту.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Счёт значения для удаления</strong></td></tr><tr><td><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Очистить значения скорборда</strong><br><code>game_clear_scoreboard_scores</code></td><td>Очищает все значения указанного скорборда.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID скорборда</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Настройки мира" %}
<img src="../../../.gitbook/assets/anvil.png" alt="" data-size="line"> **Действия, которые взаимодействуют на мир.**

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Установить время мира</strong><br><code>game_set_world_time</code></td><td>Устанавливает время мира в тиках.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Время в тиках</strong></td></tr><tr><td><img src="../../../.gitbook/assets/iron_pickaxe.png" alt="" data-size="line"> <strong>Установить выпадение блоков</strong><br><code>game_set_block_drops_enabled</code></td><td>Устанавливает правило в мире на выпадение блоков при их разрушении.</td><td><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Выпадение блоков</strong> <a data-footnote-ref href="#user-content-fn-39"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/skeleton_skull.png" alt="" data-size="line"> <strong>Установить сложность мира</strong><br><code>game_set_world_difficulty</code></td><td>Устанавливает определённую сложность в мире.</td><td><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Сложность</strong> <a data-footnote-ref href="#user-content-fn-40"><strong><code>-></code></strong></a></td></tr><tr><td><img src="../../../.gitbook/assets/writable_book.png" alt="" data-size="line"> <strong>Установить игровое правило мира</strong><br><code>game_set_world_gamerule</code></td><td>Устанавливает определённое игровое правило (gamerule) мира.<br><br>» Оставьте аргумент "Значение" пустым, чтобы сбросить его на состояние по умолчанию.</td><td><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Игровое правило</strong> <a data-footnote-ref href="#user-content-fn-41"><strong><code>-></code></strong></a><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Значение</strong></td></tr><tr><td><img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> <strong>Установить погоду мира</strong><br><code>game_set_world_weather</code></td><td>Устанавливает погоду мира на определённое время.<br><br>» По умолчания, если не указать длительность, погода не будет изменяться.</td><td><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип погоды</strong> <a data-footnote-ref href="#user-content-fn-42"><strong><code>-></code></strong></a><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность</strong></td></tr><tr><td><img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> <strong>Установить дистанцию симуляции мира</strong><br><code>game_set_world_simulation_distance</code></td><td>Устанавливает дистанцию симуляции чанков для мира.</td><td><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Дистанция симуляции в чанках (2-32)</strong></td></tr></tbody></table>
{% endtab %}

{% tab title="Веб-действия" %}
<img src="../../../.gitbook/assets/earth_head.png" alt="" data-size="line"> **Действия, которые взаимодействуют с интернет-ресурсами.**

***

<table data-full-width="true"><thead><tr><th>Опция</th><th>Описание</th><th>Аргументы</th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/earth_head.png" alt="" data-size="line"> <strong>Отправить веб-запрос</strong><br><code>game_send_web_request</code></td><td>Отправляет веб-запрос с выбранным методом и телом на выбранный URL.</td><td><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>URL</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Тело запроса</strong><br><a href="../arguments/variable/dictionary.md"><img src="../../../.gitbook/assets/chest_minecart.png" alt="" data-size="line"></a> <strong>Заголовки запроса</strong><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип запроса</strong> <a data-footnote-ref href="#user-content-fn-43"><strong><code>-></code></strong></a><br><a href="../arguments/parameter/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Медиа тип запроса</strong> <a data-footnote-ref href="#user-content-fn-44"><strong><code>-></code></strong></a></td></tr></tbody></table>
{% endtab %}
{% endtabs %}

[^1]: **Стандартное снаряжение** `natural_equipment`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^2]: **Задать движение предмета при создании** `apply_motion`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^3]: **Смогут ли подбирать предмет мобы** `can_mob_pickup`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^4]: **Смогут ли подбирать предмет игроки** `can_player_pickup`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^5]: **Появление огня** `fire`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^6]: **Разрушение блоков** `break_blocks`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^7]: **Движение** `movement`:

    * <img src="../../../.gitbook/assets/firework_rocket.png" alt="" data-size="line"> **Вверх**\
      `upwards`
    * <img src="../../../.gitbook/assets/crossbow.png" alt="" data-size="line"> **Направленное**\
      `directional`

[^8]: **Мгновенный взрыв** `instant`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^9]: **Должен исчезать** `should_expire`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^10]: **Установить гравитацию** `gravity`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^11]: **Режим маркера** `marker`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включён**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключен**\
      `false`

[^12]: **Сделать маленьким** `small`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^13]: **Отображение рук** `show_arms`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^14]: **Отображение плиты** `base_plate`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^15]: **Невидимость** `invisible`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^16]: **Создание фундамента** `show_bottom`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^17]: **По окончанию** `end_of_lifespan`:

    * <img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> **Выпасть предметом**\
      `drop`
    * <img src="../../../.gitbook/assets/ender_eye.png" alt="" data-size="line"> **Расколоться**\
      `shatter`
    * <img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"> **Случайно**\
      `random`

[^18]: **Объединение текста** `merging_mode`:

    * <img src="../../../.gitbook/assets/piston.png" alt="" data-size="line"> **Разделение пробелом**\
      `spaces`
    * <img src="../../../.gitbook/assets/sticky_piston.png" alt="" data-size="line"> **Объединение**\
      `concatenation`
    * <img src="../../../.gitbook/assets/shears.png" alt="" data-size="line"> **Разделение на строки**\
      `separate_lines`

[^19]: **Отзывчивость** `responsive`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^20]: **Обновлять блоки вокруг** `update_blocks`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Обновлять**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не обновлять**\
      `false`

[^21]: **Игнорировать воздух** `ignore_air`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Игнорировать**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не игнорировать**\
      `false`

[^22]: **Клонировать существ** `copy_entity`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Клонировать**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не клонировать**\
      `false`

[^23]: **Выпадение опыта** `drop_exp`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^24]: **Тип дерева** `tree_type`:

    * <img src="../../../.gitbook/assets/oak_sapling.png" alt="" data-size="line"> **Обычное дерево**\
      `tree`
    * <img src="../../../.gitbook/assets/oak_sapling.png" alt="" data-size="line"> **Большое дерево**\
      `big_tree`
    * <img src="../../../.gitbook/assets/acacia_sapling.png" alt="" data-size="line"> **Обычная ель**\
      `redwood`
    * <img src="../../../.gitbook/assets/acacia_sapling.png" alt="" data-size="line"> **Высокая ель**\
      `tall_redwood`
    * <img src="../../../.gitbook/assets/birch_sapling.png" alt="" data-size="line"> **Обычная берёза**\
      `birch`
    * <img src="../../../.gitbook/assets/jungle_sapling.png" alt="" data-size="line"> **Дерево джунглей**\
      `jungle`
    * <img src="../../../.gitbook/assets/jungle_sapling.png" alt="" data-size="line"> **Маленькое дерево джунглей**\
      `small_jungle`
    * <img src="../../../.gitbook/assets/jungle_sapling.png" alt="" data-size="line"> **Дерево джунглей с какао-бобами**\
      `cocoa_tree`
    * <img src="../../../.gitbook/assets/jungle_sapling.png" alt="" data-size="line"> **Куст джунглей**\
      `jungle_bush`
    * <img src="../../../.gitbook/assets/red_mushroom.png" alt="" data-size="line"> **Красный гриб**\
      `red_mushroom`
    * <img src="../../../.gitbook/assets/brown_mushroom.png" alt="" data-size="line"> **Коричневый гриб**\
      `brown_mushroom`
    * <img src="../../../.gitbook/assets/oak_sapling.png" alt="" data-size="line"> **Болотное дерево**\
      `swamp`
    * <img src="../../../.gitbook/assets/acacia_sapling.png" alt="" data-size="line"> **Акация**\
      `acacia`
    * <img src="../../../.gitbook/assets/dark_oak_sapling.png" alt="" data-size="line"> **Тёмный дуб**\
      `dark_oak`
    * <img src="../../../.gitbook/assets/acacia_sapling.png" alt="" data-size="line"> **Огромная секвойя**\
      `mega_redwood`
    * <img src="../../../.gitbook/assets/spruce_wood.png" alt="" data-size="line"> **Огромная сосна**\
      `mega_pine`
    * <img src="../../../.gitbook/assets/birch_sapling.png" alt="" data-size="line"> **Высокая берёза**\
      `tall_birch`
    * <img src="../../../.gitbook/assets/chorus_plant.png" alt="" data-size="line"> **Дерево хоруса**\
      `chorus_plant`
    * <img src="../../../.gitbook/assets/crimson_fungus.png" alt="" data-size="line"> **Багровый гриб**\
      `crimson_fungus`
    * <img src="../../../.gitbook/assets/warped_fungus.png" alt="" data-size="line"> **Искажённый гриб**\
      `warped_fungus`
    * <img src="../../../.gitbook/assets/oak_sapling.png" alt="" data-size="line"> **Азалия**\
      `azalea`
    * <img src="../../../.gitbook/assets/mangrove_fence.png" alt="" data-size="line"> **Мангровое дерево**\
      `mangrove`
    * <img src="../../../.gitbook/assets/tall_grass.png" alt="" data-size="line"> **Высокое мангровое дерево**\
      `tall_mangrove`
    * <img src="../../../.gitbook/assets/cherry_sapling.png" alt="" data-size="line"> **Вишня**\
      `cherry`

[^25]: **Тип роста** `growth_type`:

    * <img src="../../../.gitbook/assets/wooden_hoe.png" alt="" data-size="line"> **Номер стадии роста**\
      `stage_number`
    * <img src="../../../.gitbook/assets/short_grass.png" alt="" data-size="line"> **Процент роста**\
      `percentage`

[^26]: **Сторона таблички** `side`:

    * <img src="../../../.gitbook/assets/birch_sign.png" alt="" data-size="line"> **Передняя**\
      `front`
    * <img src="../../../.gitbook/assets/dark_oak_sign.png" alt="" data-size="line"> **Задняя**\
      `back`
    * <img src="../../../.gitbook/assets/cherry_sign.png" alt="" data-size="line"> **Все**\
      `all`

[^27]: **Цвет текста** `sign_text_color`:

    * <img src="../../../.gitbook/assets/white_concrete.png" alt="" data-size="line"> **Белый**\
      `white`
    * <img src="../../../.gitbook/assets/orange_concrete.png" alt="" data-size="line"> **Оранжевый**\
      `orange`
    * <img src="../../../.gitbook/assets/magenta_concrete.png" alt="" data-size="line"> **Пурпурный**\
      `magenta`
    * <img src="../../../.gitbook/assets/light_blue_concrete.png" alt="" data-size="line"> **Голубой**\
      `light_blue`
    * <img src="../../../.gitbook/assets/yellow_concrete.png" alt="" data-size="line"> **Жёлтый**\
      `yellow`
    * <img src="../../../.gitbook/assets/lime_concrete.png" alt="" data-size="line"> **Лаймовый**\
      `lime`
    * <img src="../../../.gitbook/assets/pink_concrete.png" alt="" data-size="line"> **Розовый**\
      `pink`
    * <img src="../../../.gitbook/assets/gray_concrete.png" alt="" data-size="line"> **Серый**\
      `gray`
    * <img src="../../../.gitbook/assets/light_gray_concrete.png" alt="" data-size="line"> **Светло-серый**\
      `light_gray`
    * <img src="../../../.gitbook/assets/cyan_concrete.png" alt="" data-size="line"> **Бирюзовый**\
      `cyan`
    * <img src="../../../.gitbook/assets/purple_concrete.png" alt="" data-size="line"> **Фиолетовый**\
      `purple`
    * <img src="../../../.gitbook/assets/blue_concrete.png" alt="" data-size="line"> **Синий**\
      `blue`
    * <img src="../../../.gitbook/assets/brown_concrete.png" alt="" data-size="line"> **Коричневый**\
      `brown`
    * <img src="../../../.gitbook/assets/green_concrete.png" alt="" data-size="line"> **Зелёный**\
      `green`
    * <img src="../../../.gitbook/assets/red_concrete.png" alt="" data-size="line"> **Красный**\
      `red`
    * <img src="../../../.gitbook/assets/black_concrete.png" alt="" data-size="line"> **Чёрный**\
      `black`

[^28]: **Свечение текста** `glowing`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^29]: **Вощённость** `waxed`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^30]: **Тип значения** `receive_type`:

    * <img src="../../../.gitbook/assets/player_head.png" alt="" data-size="line"> **Имя или UUID игрока**\
      `name_or_uuid`
    * <img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> **Параметр "value" скина**\
      `value`

[^31]: **Слот** `slot`:

    * <img src="../../../.gitbook/assets/gold_nugget.png" alt="" data-size="line"> **Первый**\
      `first`
    * <img src="../../../.gitbook/assets/gold_nugget.png" alt="" data-size="line"> **Второй**\
      `second`
    * <img src="../../../.gitbook/assets/gold_nugget.png" alt="" data-size="line"> **Третий**\
      `third`
    * <img src="../../../.gitbook/assets/gold_nugget.png" alt="" data-size="line"> **Четвёртый**\
      `fourth`

[^32]: **Сторона вазы** `side`:

    * <img src="../../../.gitbook/assets/prize_pottery_sherd.png" alt="" data-size="line"> **Задняя сторона**\
      `back`
    * <img src="../../../.gitbook/assets/prize_pottery_sherd.png" alt="" data-size="line"> **Левая сторона**\
      `left`
    * <img src="../../../.gitbook/assets/sheaf_pottery_sherd.png" alt="" data-size="line"> **Правая сторона**\
      `right`
    * <img src="../../../.gitbook/assets/sheaf_pottery_sherd.png" alt="" data-size="line"> **Передняя сторона**\
      `front`

[^33]: **Возможность призыва** `can_summon`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Может призывать**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не может призывать**\
      `false`

[^34]: **Состояние** `shrieking`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Кричащий**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Не кричащий**\
      `false`

[^35]: **Активация** `powered`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включить**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключить**\
      `false`

[^36]: **Убрать сообщение** `hide`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^37]: **Разрешить передвижение** `allowed`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Да**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Нет**\
      `false`

[^38]: **Тип формата** `format`:

    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Пустой**\
      `blank`
    * <img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> **Текстовый**\
      `fixed`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **Стиль**\
      `styled`
    * <img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> **Обычный**\
      `reset`

[^39]: **Выпадение блоков** `enable`:

    * <img src="../../../.gitbook/assets/lime_dye.png" alt="" data-size="line"> **Включено**\
      `true`
    * <img src="../../../.gitbook/assets/gray_dye.png" alt="" data-size="line"> **Выключено**\
      `false`

[^40]: **Сложность** `difficulty`:

    * <img src="../../../.gitbook/assets/emerald.png" alt="" data-size="line"> **Мирная**\
      `peaceful`
    * <img src="../../../.gitbook/assets/wooden_sword.png" alt="" data-size="line"> **Лёгкая**\
      `easy`
    * <img src="../../../.gitbook/assets/iron_sword.png" alt="" data-size="line"> **Нормальная**\
      `normal`
    * <img src="../../../.gitbook/assets/diamond_sword.png" alt="" data-size="line"> **Сложная**\
      `hard`

[^41]: **Игровое правило** `gamerule`:

    * Отключение рейдов (disableRaids)
    * Смена дня и ночи (doDaylightCycle)
    * Выпадение экипировки сущностей (doEntityDrops)
    * Распространение огня (doFireTick)
    * Мгновенное возрождение (doImmediateRespawn)
    * Появление фантомов (doInsomnia)
    * Выпадение добычи с мобов (doMobLoot)
    * Появление мобов (doMobSpawning)
    * Патрули Разбойников (doPatrolSpawning)
    * Выпадение блоков (doTileDrops)
    * Странствующие торговцы (doTraderSpawning)
    * Изменения погоды (doWeatherCycle)
    * Урон от утопления (drowningDamage)
    * Урон от падения (fallDamage)
    * Урон от огня (fireDamage)
    * Прощение умерших игроков (forgiveDeadPlayers)
    * Сохранение инвентаря при смерти (keepInventory)
    * Разрушительные действия мобов (mobGriefing)
    * Снаряды могут разрушать блоки (projectilesCanBreakBlocks)
    * Сообщения о смерти (showDeathMessages)
    * Регенерация здоровья (naturalRegeneration)
    * Слепая ярость (universalAnger)
    * Процент спящих (playersSleepingPercentage)
    * Малый экран отладки (reducedDebugInfo)
    * Урон от замерзания (freezeDamage)
    * Частота случайных тиков (randomTickSpeed)
    * Предел сущностей в одном блоке (maxEntityCramming)
    * Радиус области возрождения (spawnRadius)
    * Возобновление источников лавы (lavaSourceConversion)
    * Возобновление источников воды (waterSourceConversion)
    * Потеря части добычи при взрыве динамита (tntExplosionDropDecay)
    * Потеря части добычи при взрыве от взаимодействия с блоком (blockExplosionDropDecay)
    * Потеря части добычи при взрыве моба (mobExplosionDropDecay)
    * Создание только по рецепту (doLimitedCrafting)
    * Время прохождения портала Незера вне творческого режима (playersNetherPortalDefaultDelay)
    * Время прохождения портала Незера в творческом режиме (playersNetherPortalCreativeDelay)
    * Высота снежного покрова (showAccumulationHeight)
    * Радиус чанков возрождения (shawnChunkRadius)
    * Появление Хранителей (doWardenSpawning)
    * Исчезновение брошенного эндер-жемчуга при смерти (enderPearlsVanishOnDeath)
    * Распространение лозы (doVinesSpread)

[^42]: **Тип погоды** `weather_type`:

    * <img src="../../../.gitbook/assets/bucket.png" alt="" data-size="line"> **Ясная**\
      `clear`
    * <img src="../../../.gitbook/assets/water_bucket.png" alt="" data-size="line"> **Дождливая**\
      `raining`
    * <img src="../../../.gitbook/assets/nether_star.gif" alt="" data-size="line"> **Гроза**\
      `thunder`

[^43]: **Тип запроса** `request_type`:

    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **GET**\
      `get`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **HEAD**\
      `head`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **POST**\
      `post`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **PUT**\
      `put`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **PATCH**\
      `patch`
    * <img src="../../../.gitbook/assets/feather.png" alt="" data-size="line"> **DELETE**\
      `delete`

[^44]: **Медиа тип запроса** `content_type`:

    * <img src="../../../.gitbook/assets/writable_book.png" alt="" data-size="line"> **Обычный текст (text/plain)**\
      `text_plain`
    * <img src="../../../.gitbook/assets/bookshelf.png" alt="" data-size="line"> **JSON (application/json)**\
      `application_json`
