---
description: >-
  Контролирует выполнение кода внутри поршней, может проверять наличие ошибки
  или затрату по времени на выполнение кода.
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

# Контроллер

<figure><img src="../../../.gitbook/assets/dark_prismarine.png" alt="" width="150"><figcaption></figcaption></figure>

**Тип:** Действие\
**Текстовый идентификатор:** `controller_action`

***

## Использование

Поставьте блок в строку и нажмите ПКМ по нему, чтобы открыть меню опций блока. В открывшемся меню выберите нужное действие контроллера.

Внутри поршней выполняется код, который подчиняется контроллеру. Код, расположенный после поршней, не будет подчиняться контроллеру.

### Опции

| Опция                                                                                                                                                            | Описание                                                                                                                                                                        | Аргументы                                                                                                                                                                                                                                                                                                                                                                                                       |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><img src="../../../.gitbook/assets/red_dye.png" alt="" data-size="line"> <strong>Уловить ошибку</strong><br><code>controller_exception</code></p>             | <p>Улавливает ошибку в коде внутри поршней и присваивает её содержание к переменной.<br><br>» Не улавливает глобальные и критические ошибки.</p>                                | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Тип ошибки</strong> <a data-footnote-ref href="#user-content-fn-1"><strong><code>-></code></strong></a></p>     |
| <p><img src="../../../.gitbook/assets/clock.png" alt="" data-size="line"> <strong>Замерить время выполнения</strong><br><code>controller_measure_time</code></p> | <p>Замеряет время выполнения кода внутри поршней и присваивает результат к переменной.<br><br>» Учитывает блоки "<a data-footnote-ref href="#user-content-fn-2">Ждать</a>".</p> | <p><a href="../arguments/variable/"><img src="../../../.gitbook/assets/magma_cream.png" alt="" data-size="line"></a> <strong>Переменная для присвоения</strong><br><a href="../arguments/enum.md"><img src="../../../.gitbook/assets/heart_of_the_sea.png" alt="" data-size="line"></a> <strong>Формат времени</strong> <a data-footnote-ref href="#user-content-fn-3"><strong><code>-></code></strong></a></p> |

[^1]: * Предупреждение
    * Ошибка

[^2]: Опция **Ждать** в блоке [**Контроль действий**](control.md).

[^3]: * Наносекунды
    * Микросекунды
    * Миллисекунды
