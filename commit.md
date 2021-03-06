[ К содержанию](./readme.md)



## git commit

---

**Коммит** — базовое понятие во всех системах контроля версий, поэтому совершаться он должен легко и по возможности быстро. В простейшем случае достаточно после индексации набрать:

```bash=
git commit
```

Если индекс не пустой, то на его основе будет совершен коммит, после чего пользователя попросят прокомментировать вносимые изменения вызовом команды **edit.** Сохраняемся, и вуаля! Коммит готов. Есть несколько ключей, упрощающих работу с ***git commit.***

Совершает коммит, автоматически индексируя изменения в файлах проекта. Новые файлы при этом индексироваться не будут! Удаление же файлов будет учтено:

```bash=
git commit -a
```

Комментирует коммит прямо из командной строки вместо текстового редактора:


```bash=
git commit -m «commit comment»
```

Вносит в индекс и создаёт коммит на основе изменений единственного файла:

```bash=
git commit FILENAME
```