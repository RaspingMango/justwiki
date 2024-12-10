---
description: Используется для взаимодействия с переменными.
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

# Действие с переменной

<figure><img src="../../../.gitbook/assets/iron_block.png" alt="" width="150"><figcaption><p>Блок кода</p></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `set_variable`

***

## Использование

Поставьте блок в строку и нажмите ПКМ по нему, чтобы открыть меню опций блока. Перейдите в нужную категорию и выберите действие, которое необходимо выполнить.

При выборе действия, над его блоком может появиться хранилище (по умолчанию: сундук), в котором содержатся [аргументы](../arguments/) действия.

### Опции

{% tabs %}
{% tab title="Присвоение значений" %}
<img src="../../../.gitbook/assets/iron_block.png" alt="" data-size="line"> **Различный операции присвоения.**

***

| Опция                                                                                                                                                                          | Описание                                                                   | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/iron_ingot.png" alt="" data-size="line"> <strong>Установить значение (=)</strong><br><code>set_variable_value</code></p>                 | Присваивает значение к переменной.                                         | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/"><img src="../../../.gitbook/assets/white_dye.png" alt="" data-size="line"></a> <strong>Значение для присвоения</strong></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| <p><img src="../../../.gitbook/assets/eye_of_ender.png" alt="" data-size="line"> <strong>Установить случайное значение</strong><br><code>set_variable_random</code></p>        | Присваивает случайное значение к переменной.                               | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/"><img src="../../../.gitbook/assets/white_dye.png" alt="" data-size="line"></a> <strong>Значения для выбора</strong></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| <p><img src="../../../.gitbook/assets/fire_coral.png" alt="" data-size="line"> <strong>Очистить переменные</strong><br><code>set_variable_purge</code></p>                     | Очищает все переменные, подходящие под выбранные имена.                    | <p><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Имена для сравнения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип переменной</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим сравнения</strong> <a data-footnote-ref href="#user-content-fn-2"><strong><code>-></code></strong></a><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Игнорирование регистра</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></p> |
| <p><img src="../../../.gitbook/assets/ender_chest.png" alt="" data-size="line"> <strong>Получить имена переменных</strong><br><code>set_variable_get_list_variables</code></p> | Получает список имён всех переменных и присваивает результат к переменной. | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип переменных</strong> <a data-footnote-ref href="#user-content-fn-4"><strong><code>-></code></strong></a></p>                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
{% endtab %}

{% tab title="Числовые операции" %}
<img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> **Различные числовые операции.**

***

| Опция                                                                                                                                                                         | Описание                                                                                                                                                               | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> <strong>Преобразовать текст в число</strong><br><code>set_variable_convert_text_to_number</code></p> | Присваивает к переменной результат преобразования числа в виде текста другой системы счисления в число десятичной системы счисления. Работает только с целыми числами. | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Текст для преобразования</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Основание системы счисления</strong></p>                                                                                                                                                                                                               |
| <p><img src="../../../.gitbook/assets/brick.png" alt="" data-size="line"> <strong>Сложение чисел (+)</strong><br><code>set_variable_add</code></p>                            | Присваивает к переменной сумму чисел.                                                                                                                                  | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Числа для суммирования</strong></p>                                                                                                                                                                                                                                                                                                                                                                          |
| <p><img src="../../../.gitbook/assets/nether_brick.png" alt="" data-size="line"> <strong>Вычитание чисел (-)</strong><br><code>set_variable_subtract</code></p>               | Присваивает к переменной разницу чисел.                                                                                                                                | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Числа для вычитания</strong></p>                                                                                                                                                                                                                                                                                                                                                                             |
| <p><img src="../../../.gitbook/assets/bricks.png" alt="" data-size="line"> <strong>Умножение чисел (×)</strong><br><code>set_variable_multiply</code></p>                     | Присваивает к переменной произведение чисел.                                                                                                                           | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Числа для умножения</strong></p>                                                                                                                                                                                                                                                                                                                                                                             |
| <p><img src="../../../.gitbook/assets/nether_bricks.png" alt="" data-size="line"> <strong>Деление чисел (÷)</strong><br><code>set_variable_divide</code></p>                  | Присваивает к переменной частное чисел.                                                                                                                                | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Числа для деления</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим деления</strong> <a data-footnote-ref href="#user-content-fn-5"><strong><code>-></code></strong></a></p>                                                                                                                                    |
| <p><img src="../../../.gitbook/assets/nether_wart.png" alt="" data-size="line"> <strong>Остаток от деления (%)</strong><br><code>set_variable_remainder</code></p>            | Присваивает к переменной остаток от деления двух чисел.                                                                                                                | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Делимое</strong><br><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Делитель</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Режим работы</strong> <a data-footnote-ref href="#user-content-fn-6"><strong><code>-></code></strong></a></p> |
{% endtab %}
{% endtabs %}

[^1]: * Игровая
    * Сохранённая
    * Локальная

[^2]: * Полное соответствие
    * Имя содержит текст
    * Текст содержит имя

[^3]: * Включено
    * Выключено

[^4]: * Игровые
    * Сохранённые
    * Локальные

[^5]: * По умолчанию
    * Обычное округление
    * Округлить до меньшего
    * Округлить до большего

[^6]: * Остаток от деления (оставляет знак делимого)
    * Остаток по модулю (оставляет знак делителя)
