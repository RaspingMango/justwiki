---
description: >-
  Выполняет код внутри поршней, если условие, привязанное к этому блоку,
  неверно.
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

# Иначе

<figure><img src="../../../.gitbook/assets/end_stone.png" alt="" width="150"><figcaption><p>Блок кода</p></figcaption></figure>

**Тип:** Условие\
**Текстовый идентификатор:** `else`

***

## Использование

Поставьте блок в строку кода. Данный блок можно поставить только если предшествующий ему блок является блоком условия:

* [<img src="../../../.gitbook/assets/oak_planks.png" alt="" data-size="line"> **Если игрок**](if\_player.md)
* [<img src="../../../.gitbook/assets/mossy_cobblestone.png" alt="" data-size="line"> **Если сущность**](if\_entity.md)
* [<img src="../../../.gitbook/assets/red_nether_bricks.png" alt="" data-size="line"> **Если в мире**](if\_game.md)
* [<img src="../../../.gitbook/assets/obsidian.png" alt="" data-size="line"> **Если переменная**](if\_variable.md)

Внутри поршней выполняется код, который подчиняется поставленному условию. Код, расположенный после поршней, не будет подчиняться условию.
