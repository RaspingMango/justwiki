---
description: Используется для указания аргументов типа звук.
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

# Звук

<figure><img src="../../../.gitbook/assets/nautilus_shell.png" alt="" width="150"><figcaption></figcaption></figure>

**Команда получения:** `/sound`\
**Ячейка:** <img src="../../../.gitbook/assets/purple_stained_glass_pane.png" alt="" data-size="line">\
**Текстовый идентификатор:** `sound`

***

## Использование

Возьмите значение в активный слот и нажмите ПКМ. В открывшемся меню перейдите в нужную категорию и выберите звук, либо воспользуйтесь поиском звуков по ID.

* Нажатие ЛКМ воспроизводит звук.
* Нажатие Shift + ЛКМ прекращает воспроизведение звука.

#### У звука есть параметры, которые можно изменять:

| Параметр  | Команда                                                                                  |
| --------- | ---------------------------------------------------------------------------------------- |
| Громкость | `/sound volume <число>`                                                                  |
| Высота    | `/sound pitch <число>`                                                                   |
| Вариация  | `/sound seed <вариация>`                                                                 |
| Источник  | `/sound source <AMBIENT/BLOCK/HOSTILE/MASTER/MUSIC/NEUTRAL/PLAYER/RECORD/VOICE/WEATHER>` |
