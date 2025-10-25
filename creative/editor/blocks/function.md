---
description: Хранит строку кода, которую можно вызвать с помощью блока "Вызвать функцию".
---

# Функция

<figure><img src="../../../.gitbook/assets/lapis_block.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Функция\
**Текстовый идентификатор:** `function`

***

## Использование

Поставьте блок в самое начало строки. Любой код, который вы напишете далее в этой строке, будет входить в функцию.

Присвойте название функции. Для этого возьмите значение [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> **Текст**](../arguments/text.md) в активный слот напишите в чат название. Затем, продолжая держать значение в активном слоте, нажмите <kbd>ПКМ</kbd> по блоку функции.

#### Дополнительные аргументы функции:

* [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/parameter/enum.md) **Отображать функцию в меню вызова** [**`->`**](#user-content-fn-1)[^1]
* [<img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line">](../arguments/item.md) **Значок функции**
* [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line">](../arguments/text.md) **Описание функции**

## Принцип работы

<figure><img src="../../../.gitbook/assets/function_sheme.png" alt="" width="563"><figcaption><p>Схема, изображающая принцип работы функции.</p></figcaption></figure>

Функция вызывается в строке кода блоком [<img src="../../../.gitbook/assets/lapis_ore.png" alt="" data-size="line"> **Вызвать функцию**](call_function.md). Воспроизведение кода в строке не будет продолжаться до тех пор, пока функция не завершит своё выполнение.

Вы можете вынести часто повторяющийся код в функцию и вызывать её, чтобы сэкономить место в коде и ваше время.

[^1]: * <img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"> **Скрыть**
    * <img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"> **Отображать**
