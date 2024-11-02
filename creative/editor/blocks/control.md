---
description: Используется для дальнейшего контроля кода, стоящего после этого блока.
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

# Контроль действий

<figure><img src="../../../.gitbook/assets/coal_block.png" alt="" width="150"><figcaption><p>Блок кода</p></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `control_action`

***

## Использование

Поставьте блок в строку и нажмите ПКМ по нему, чтобы открыть меню опций блока. В открывшемся меню выберите нужную манипуляцию над выполнением кода.

### Опции

| Опция                                                                                                                                                                   | Описание                                                                                                       | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        | Доп. сведения                                                                                              |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Ждать</strong><br><code>control_wait</code></p>                                       | Приостанавливает текущую последовательность блоков кода на определённое время.                                 | <p><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность ожидания</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Единица времени</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p>                                                                                                                      | » Минимальная задержка - 1 тик; в режиме Тики можно установить только целые числа.                         |
| <p><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Остановить последовательность</strong><br><code>control_end_thread</code></p>       | Останавливает текущую последовательность блоков кода. Любой код после этого блока не будет выполнен.           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | » Если действие было использовано в функциях, то остановит родительскую строку, в которой вызвали функцию. |
| <p><img src="../../../.gitbook/assets/arrow_of_splashing.png" alt="" data-size="line"> <strong>Вернуться до вызова</strong><br><code>control_return_function</code></p> | Останавливает текущую последовательность блоков кода в функции и возвращает к блоку вызова этой самой функции. |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | » Возвращает до блока вызова текущей функции в родительской строке.                                        |
| <p><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"> <strong>Остановить повторение</strong><br><code>control_stop_repeat</code></p>     | Полностью останавливает текущее повторение.                                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | <p>Работает с:<br>» Повторениями</p>                                                                       |
| <p><img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> <strong>Пропустить повторение</strong><br><code>control_skip_iteration</code></p>       | Пропускает одну итерацию в текущем повторении.                                                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | <p>Работает с:<br>» Повторениями</p>                                                                       |
| <p><img src="../../../.gitbook/assets/red_dye.png" alt="" data-size="line"> <strong>Вызвать ошибку</strong><br><code>control_call_exception</code></p>                  | Вызывает определённую ошибку с указанным ID и сообщением.                                                      | <p><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID ошибки</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Сообщение ошибки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип ошибки</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></p> | » Рекомендуется использовать это в действии "[Уловить ошибку](#user-content-fn-2)[^2]".                    |

[^1]: * Тики
    * Секунды
    * Минуты

[^2]: Опция **Уловить ошибку** в блоке [**Контроллер**](controller.md).

[^3]: * Предупреждение
    * Ошибка
    * Критическая
