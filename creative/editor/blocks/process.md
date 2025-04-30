---
description: Хранит строку кода, которую можно вызвать с помощью блока "Запустить процесс".
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

# Процесс

<figure><img src="../../../.gitbook/assets/emerald_block.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Процесс\
**Текстовый идентификатор:** `process`

***

## Использование

Поставьте блок в самое начало строки. Любой код, который вы напишете далее в этой строке, будет входить в процесс.

Присвойте название процессу. Для этого возьмите значение [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line"> **Текст**](../arguments/text.md) в активный слот напишите в чат название. Затем, продолжая держать значение в активном слоте, нажмите <kbd>ПКМ</kbd> по блоку процесса.

#### Дополнительные аргументы процесса:

* [<img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line">](../arguments/enum.md) **Отображать процесс в меню вызова** [**`->`**](#user-content-fn-1)[^1]
* [<img src="../../../.gitbook/assets/item_frame.png" alt="" data-size="line">](../arguments/item.md) **Значок процесса**
* [<img src="../../../.gitbook/assets/book.png" alt="" data-size="line">](../arguments/text.md) **Описание процесса**

## Принцип работы

<figure><img src="../../../.gitbook/assets/Process_Scheme.png" alt="" width="563"><figcaption><p>Схема, изображающая принцип работы процесса.</p></figcaption></figure>

Процесс запускается в строке кода блоком [<img src="../../../.gitbook/assets/emerald_ore.png" alt="" data-size="line"> **Запустить процесс**](start_process.md). Строка кода, где он вызывается, будет продолжать свою работу, даже если сам процесс не завершился.

Процесс, в отличие от [<img src="../../../.gitbook/assets/lapis_block.png" alt="" data-size="line"> **функции**](function.md), запускает собственную строку кода независимо от строки, в которой он был вызван. То есть блок [<img src="../../../.gitbook/assets/coal_block.png" alt="" data-size="line"> **Контроль действий**](control.md) не будет влиять на выполнение основной ветви кода.

Процесс можно запускать с различным [режимом передачи переменных](start_process.md#rezhim-peremennykh) и [целями](start_process.md#cel-processa).

Злоупотребление вызовом процессов может оказать значительную нагрузку на мир. Поэтому рекомендуется использовать процесс только в тех случаях, когда это действительно необходимо.

[^1]: * Скрыть
    * Отображать
