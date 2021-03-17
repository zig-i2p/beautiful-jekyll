---
layout: post
title: Образец блога
subtitle: Каждая должность также имеет подзаголовок
gh-repo: daattali/beautiful-jekyll
gh-badge: [star, fork, follow]
tags: [test]
comments: true
---

Это демо-пост, чтобы показать вам, как писать сообщения в блоге с разметкой.  Я настоятельно призываю вас [выдели 5 минут, чтобы узнать, как написать в Markdown](https://markdowntutorial.com/) - Это научит вас, как превратить обычный текст в
bold/italics/headings/tables/etc.

**Вот некоторые примеры текста**

## Вот второстепенный заголовок

Вот бесполезная таблица:

| Номер | Следующий номер | Предыдущий номер |
| :------ |:--- | :--- |
| Пять | Шесть | Четыре |
| Десять | Одиннадцать | Девять |
| Семь | Восемь | Шесть |
| Два | Три | Один |


Как насчет вкусного крепа?

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg)

Он также может быть по центру!

![Crepe](https://s3-media3.fl.yelpcdn.com/bphoto/cQ1Yoa75m2yUFFbY2xwuqw/348s.jpg){: .mx-auto.d-block :}

Вот фрагмент кода:

~~~
var foo = function(x) {
  return(x + 5);
}
foo(3)
~~~

А вот тот же код с синтаксисом:

```javascript
var foo = function(x) {
  return(x + 5);
}
foo(3)
```

И вот тот же код еще раз, но с номерами строк:

{% highlight javascript linenos %}
var foo = function(x) {
  return(x + 5);
}
foo(3)
{% endhighlight %}

## Коробки
Вы можете добавить уведомления, предупреждения и ошибки коробки, как это:

### Уведомления

{: .box-note}
**Примечание:** Это окно уведомлений.

### Предупреждение

{: .box-warning}
**Предупреждение:** Это предупреждающий ящик.

### Ошибка

{: .box-error}
**Ошибка:** Это окно ошибок.
