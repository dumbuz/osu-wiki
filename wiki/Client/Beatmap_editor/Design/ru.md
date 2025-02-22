---
outdated_translation: true  # нужно перевести с нуля
---

# Дизайн

**Редактор сториборды** — одна из вкладок [редактора карт](/wiki/Client/Beatmap_editor), позволяющая легко (относительно [ручного скриптинга](/wiki/Storyboard/Scripting)) создать собственный [сториборд](/wiki/Storyboard).

## Возможности

- Показывает текущую позицию курсора и время в миллесекундах.
- Показывает текущую [загрузку сториборды](/wiki/Client/Beatmap_editor/SB_Load).
- Позволяет отображать/скрывать различные слои картинок (задний фон, fail, pass, передний фон и игровые объекты)
- Основные эффекты трансформации картинок (работает по ключевым кадрам):
  - Движение.
  - Изменение размера.
  - Изменение прозрачности.
  - Поворот.
- Дополнительные эффекты:
  - Именение размера только по оси Х или Y.
  - Зеркальное отображение по горизонтали/вертикали.
- Tweening.
- Easing — скорость, с которой происходит переход от одного ключевого кадра к другому.
- Origin — точка, от которой ведётся отсчёт нахождения объекта и вокруг которой объект будет вращаться. Используется редко.
- Возможность сделать анимацию, которая будет отображаться только на текущем уровне сложности.
- Возможность добавить фоновую картинку и задать цвет остального фона.

## Ограничения

- Нет возможности задать звуки через SB, что практически никогда не используется, т. к. посторонние звуки отвлекают игрока от игры, а если они ещё и звучат как хитсаунды, то игрок может просто запутаться.
- Нет поддержки повторов (loops) и триггерных действий.
- Нет поддержки изменения цвета.

Для действий выше встроенный редактор карт не годится, для соответствующих изменений нужно использовать [ручной скриптинг](/wiki/Storyboard/Scripting).
