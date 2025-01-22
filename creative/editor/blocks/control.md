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

<figure><img src="../../../.gitbook/assets/coal_block.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `control_action`

***

## Использование

Поставьте блок в строку и нажмите <kbd>ПКМ</kbd> по нему, чтобы открыть меню опций блока. В открывшемся меню выберите нужную манипуляцию над выполнением кода.

### Опции

| Опция                                                                                                                                                                   | Описание                                                                                                                                                                                                                      | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Ждать</strong><br><code>control_wait</code></p>                                       | <p>Приостанавливает текущую последовательность блоков кода на определённое время.<br><br>» Минимальная задержка - 1 тик; в режиме Тики можно установить только целые числа.</p>                                               | <p><a href="../arguments/number.md"><img src="../../../.gitbook/assets/slime_ball.png" alt="" data-size="line"></a> <strong>Длительность ожидания</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Единица времени</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p>                                                                                                                      |
| <p><img src="../../../.gitbook/assets/barrier.png" alt="" data-size="line"> <strong>Остановить последовательность</strong><br><code>control_end_thread</code></p>       | <p>Останавливает текущую последовательность блоков кода. Любой код после этого блока не будет выполнен.<br><br>» Если действие было использовано в функциях, то остановит родительскую строку, в которой вызвали функцию.</p> |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <p><img src="../../../.gitbook/assets/arrow_of_splashing.png" alt="" data-size="line"> <strong>Вернуться до вызова</strong><br><code>control_return_function</code></p> | <p>Останавливает текущую последовательность блоков кода в функции и возвращает к блоку вызова этой самой функции.<br><br>» Возвращает до блока вызова текущей функции в родительской строке.</p>                              |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <p><img src="../../../.gitbook/assets/prismarine_shard.png" alt="" data-size="line"> <strong>Остановить повторение</strong><br><code>control_stop_repeat</code></p>     | <p>Полностью останавливает текущее повторение.<br><br>Работает с:<br>» Повторениями</p>                                                                                                                                       |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <p><img src="../../../.gitbook/assets/ender_pearl.png" alt="" data-size="line"> <strong>Пропустить повторение</strong><br><code>control_skip_iteration</code></p>       | <p>Пропускает одну итерацию в текущем повторении.<br><br>Работает с:<br>» Повторениями</p>                                                                                                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| <p><img src="../../../.gitbook/assets/red_dye.png" alt="" data-size="line"> <strong>Вызвать ошибку</strong><br><code>control_call_exception</code></p>                  | <p>Вызывает определённую ошибку с указанным ID и сообщением.<br><br>» Рекомендуется использовать это в действии "<a data-footnote-ref href="#user-content-fn-2">Уловить ошибку</a>".</p>                                      | <p><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>ID ошибки</strong><br><a href="../arguments/text.md"><img src="../../../.gitbook/assets/book.png" alt="" data-size="line"></a> <strong>Сообщение ошибки</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип ошибки</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></p> |

[^1]: * Тики
    * Секунды
    * Минуты

[^2]: Опция **Уловить ошибку** в блоке [**Контроллер**](controller.md).

[^3]: * Предупреждение
    * Ошибка
    * Критическая
