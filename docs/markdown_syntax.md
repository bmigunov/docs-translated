## Оглавление

* [[#1. Обзор]]
* [[#2. Заголовки]]
	* [[#2.1. Альтернативный синтаксис]]
* [[#3. Параграфы]]
* [[#4. Перевод строки]]
* [[#5. Подчёркивание]]
	* [[#5.1. Жирный]]
	* [[#5.2. Курсив]]
	* [[#5.3. Жирный курсив]]
* [[#6. Цитаты]]
	* [[#6.1. Цитирование нескольких параграфов]]
	* [[#6.2. Вложенное цитирование]]
	* [[#6.3. Цитаты с другими элементами]]
	* [[#6.4. Дополнительно]]
* [[#7. Списки]]
	* [[#7.1. Упорядоченные списки]]
	* [[#7.2. Неупорядоченные списки]]
	* [[#7.3. Дополнительно]]
	* [[#7.4. Вставка элементов Markdown в списки]]
* [[#8. Код]]
	* [[#8.1. Использование escape-последовательностей]]
	* [[#8.2. Блоки кода]]
* [[#9. Горизонтальные линии]]
* [[#10. Ссылки]]
	* [[#10.1. Привязка "тайтлов"]]
	* [[#10.2. URL и Email-адреса]]
	* [[#10.3. Форматирование ссылок]]
	* [[#10.4. Ссылки-сноски]]
* [[#11. Изображения]]
	* [[#11.1. Изображение-ссылка]]
* [[#12. Игнорирование символов]]
* [[#13. HTML]]
* [[#14. Расширенный синтаксис]]
	* [[#14.1. Доступность]]
		* [[#14.1.1. Легковесные языки разметки]]
		* [[#14.1.2. Обработчики языков разметки]]
	* [[#14.2. Таблицы]]
		* [[#14.2.1. Выравнивание]]
		* [[#14.2.2. Форматирование текста]]
		* [[#14.2.3. Игнорирование символа прямой черты]]
	* [[#14.3. Выделенные блоки кода]]
		* [[#14.3.1. Подсветка синтаксиса]]
	* [[#14.4. Сноски]]
	* [[#14.5. Идентификаторы заголовков]]
		* [[#14.5.1. Ссылки на идентификаторы заголовков]]
	* [[#14.6. Списки определений]]
	* [[#14.7. Зачёркнутый текст]]
	* [[#14.8. Списки задач]]
	* [[#14.9. Emoji]]
		* [[#14.9.1. Копирование и вставка]]
		* [[#14.9.2. Использование коротких кодов emoji]]
	* [[#14.10. Подсветка текста]]
	* [[#14.11. Индексация символов]]
		* [[#14.11.1. Нижняя]]
		* [[#14.11.2. Верхняя]]
	* [[#14.12. Автоматическое связывание URL]]

## 1. Обзор
Практически все приложения, использующие *Markdown*, поддерживают его базовый
синтаксис, определённый в оригинальной спецификации. Существуют небольшие
вариации и расхождения между обработчиками *Markdown*, и они, по возможности,
всегда в них обозначены.

## 2. Заголовки
Для создания заголовка используются знаки "решётки" (`#`), поставленные перед
словом или фразой. Количество знаков "решётки" определяют уровень вложенности.

***

**Markdown**  
`# Heading level 1`  
**HTML**  
`<h1>Heading level 1</h1>`  
**Вывод**  
# Heading level 1

***

**Markdown**  
`## Heading level 2`  
**HTML**  
`<h2>Heading level 2</h2>`  
**Вывод**  
## Heading level 2

***

**Markdown**  
`### Heading level 3`  
**HTML**  
`<h3>Heading level 3</h3>`  
**Вывод**  
### Heading level 3

***

**Markdown**  
`#### Heading level 4`  
**HTML**  
`<h4>Heading level 4</h4>`  
**Вывод**  
#### Heading level 4

***

**Markdown**  
`##### Heading level 5`  
**HTML**  
`<h5>Heading level 5</h5>`  
**Вывод**  
##### Heading level 5

***

**Markdown**  
`###### Heading level 6`  
**HTML**  
`<h6>Heading level 6</h6>`  
**Вывод**  
###### Heading level 6

***

### 2.1. Альтернативный синтаксис
Дополнительно, ниже линии с текстом можно добавить любое количество символов
`==` для заголовков первого уровня вложенности или `--` для заголовков второго
уровня вложенности.

***

**Markdown**  
```
Heading level 1
===============
```  
**HTML**  
`<h1>Heading level 1</h1>`  
**Вывод**  
# Heading level 1

***

**Markdown**  
```
Heading level 2
---------------
```  
**HTML**  
`<h2>Heading level 2</h2>`  
**Вывод**  
## Heading level 2

***

## 3. Параграфы
Для создания параграфа используется пустая строка, разделяющая одну или
несеколько линий текста.

***

**Markdown**  
```
I really like using Markdown.

I think I'll use it to format all of my documents from now on.
```  
**HTML**  
```
<p>I really like using Markdown</p>

<p>I think I'll use it to format all of my documents from now on.
```  
**Вывод**  
I really like using Markdown.

I think I'll use it to format all of my documents from now on.

***

Не стоит выделять параграфы отсупами в виде пробелов и/или табуляций (если
параграф не в списке).

## 4. Перевод строки
Для создания разрыва строки/новой линии (`<br>`), нужно завершить строку двумя
или более пробелами, затем перевести строку.

***

**Markdown**  
```
This is the first line.  
And this is the second line.  
```  
**HTML**  
```
<p>This is the first line.<br>
And this is the second line.</p>
```  
**Вывод**  
This is the first line.  
And this is the second line.

***

## 5. Подчёркивание
Существует возможность выделить текст, сделав его жирным или курсивным.  

### 5.1. Жирный
Для выделения текста жирным шрифтом, нужно добавить два символа "звёздочки" или
нижнего подчёркивания до и после нужного сегмента текста.

| Markdown                     | HTML                                      | Вывод                      |
|------------------------------| ------------------------------------------|----------------------------|
| `I just love **bold text**.` | `I just love <strong>bold text</strong>.` | I just love **bold text**. |
| `I just love __bold text__.` | `I just love <strong>bold text</strong>.` | I just love __bold text__. |
| `Love**is**bold`             | `Love<strong>is</strong>bold`             | Love**is**bold             |

Использование символов нижнего подчёркивания в середине слов нежелательно.

### 5.2. Курсив
Для выделения текста курсивом используется символ "звёздочки" или символ нижнего
подчёркивания до и после выделяемого участка текста.

| Markdown                               | HTML                                          | Вывод                                   |
|----------------------------------------|-----------------------------------------------|-----------------------------------------|
| `Italicized text is the *cat's meow*.` | `Italicized text is the <em>cat's meow</em>.` | Italicized text is the *cat's meow*.    |
| `Italicized text is the _cat's meow_.` | `Italicized text is the <em>cat's meow</em>.` | Italicized text is the _cat's meow_.    |
| `A*cat*meow`                           | `A<em>cat</em>meow`                           | A*cat*meow                              |

Использование символов нижнего подчёркивания в середине слов нежелательно.

### 5.3. Жирный курсив
Для выделения текста жирным курсивом используются по три символа "звёздочки"
и/или нижнего подчёркивания до и после выделяемого фрагмента.

| Markdown                                   | HTML                                                          | Вывод                                   |
|--------------------------------------------|---------------------------------------------------------------|-----------------------------------------|
| `This text is ***really important***.`     | `This text is <em><strong>really important</strong></em>.`    | This text is ***really important***.    |
| `This text is ___really important___.`     | `This text is <em><strong>really important</strong></em>.`    | This text is ___really important___.    |
| `This text is __*really important*__.`     | `This text is <em><strong>really important</strong></em>.`    | This text is __*really important*__.    |
| `This text is **_really important_**.`     | `This text is <em><strong>really important</strong></em>.`    | This text is **_really important_**.    |
| `This is really***very***important text.`  | `This is really<em><strong>very</strong></em>important text.` | This is really***very***important text. |

Использование символов нижнего подчёркивания в середине слов нежелательно.

## 6. Цитаты
Для цитирования используется символ `>` в начале параграфа.

***

**Markdown**  
`> Dorothy followed her through many of the beautiful rooms in her castle.`  
**Вывод**  

> Dorothy followed her through many of the beautiful rooms in her castle.  

***

### 6.1. Цитирование нескольких параграфов
Цитаты могут содержать несколько параграфов. Для этого нужно добавить символ `>`
на пустой строке между параграфами.

***

**Markdown**  
```
> Dorothy followed her through many of the beautiful rooms in her castle
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```  
**Вывод**  

> Dorothy followed her through many of the beautiful rooms in her castle
>
> The Witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  

***

### 6.2. Вложенное цитирование
Цитаты могут быть вложенными. Для этого нужно добавить символы `>>` перед
парагрофом, который нужно "вложить".

***

**Markdown**  
```
> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.
```  
**Вывод**  

> Dorothy followed her through many of the beautiful rooms in her castle.
>
>> The witch bade her clean the pots and kettles and sweep the floor and keep the fire fed with wood.  

***

### 6.3. Цитаты с другими элементами
Цитаты могут содержать другие элементы формата Markdown. Не все элементы могут
быть использованы.

***

**Markdown**  
```
> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everything* is going accorting to **plan**.
```  
**Вывод**  

> #### The quarterly results look great!
>
> - Revenue was off the chart.
> - Profits were higher than ever.
>
> *Everything* is going accorting to **plan**.  

***

### 6.4. Дополнительно
Для совместимости желательно вставлять пустые линии до и после цитат.

## 7. Списки
Списки могут быть упорядоченными и неупорядоченными.

### 7.1. Упорядоченные списки
Для создания упорядоченного списка используются числа и следующие за ними точки.
Числа могут следовать не по порядку, но список должен начинаться с числа 1.

***

**Markdown**  
```
1. First item
2. Second item
3. Third item
4. Fourth item
```  
**HTML**  
```
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>
```  
**Вывод**  
1. First item
2. Second item
3. Third item
4. Fourth item

***

**Markdown**  
```
1. First item
1. Second item
1. Third item
1. Fourth item
```  
**HTML**  
```
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ol>
```  
**Вывод**  
1. First item
1. Second item
1. Third item
1. Fourth item

***

**Markdown**  
```
1. First item
2. Second item
3. Third item
	1. Indented item
	2. Indented item
4. Fourth item
```  
**HTML**  
```
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ol>
      <li>Indented item</li>
      <li>Indented item</li>
    </ol>
  </li>
  <li>Fourth item</li>
</ol>
```  
**Вывод**  
1. First item
2. Second item
3. Third item
	1. Indented item
	2. Indented item
4. Fourth item

***

### 7.2. Неупорядоченные списки
Для создания неупорядоченных списков используются символы черты, "звёздочки" или
знак плюса перед элементами списка. Для вложения в список, перед вкладываемым
элементом делается отступ.

***

**Markdown**  
```
- First item
- Second item
- Third item
- Fourth item
```  
**HTML**  
```
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>
```  
**Вывод**  
- First item
- Second item
- Third item
- Fourth item

***

**Markdown**  
```
* First item
* Second item
* Third item
* Fourth item
```  
**HTML**  
```
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>
```  
**Вывод**  
* First item
* Second item
* Third item
* Fourth item

***

**Markdown**  
```
+ First item
+ Second item
+ Third item
+ Fourth item
```  
**HTML**  
```
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
  <li>Fourth item</li>
</ul>
```  
**Вывод**  
+ First item
+ Second item
+ Third item
+ Fourth item

***

**Markdown**  
```
- First item
- Second item
- Third item
	- Indented item
	- Indented item
- Fourth item
```  
**HTML**  
```
<ul>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item
    <ul>
      <li>Indented item</li>
      <li>Indented item</li>
    </ul>
  </li>
  <li>Fourth item</li>
</ul>
```  
**Вывод**  
- First item
- Second item
- Third item
	- Indented item
	- Indented item
- Fourth item

***

### 7.3. Дополнительно
Для создания элемента, начинающегося с числа, в неупорядоченном списке, можно
воспользоваться escape-символом обратная косая черта (`\`).  
Также не рекомендуется смешивать доступные разделители для составления списков
между собой.

### 7.4. Вставка элементов Markdown в списки
Для того, чтобы добавить в список элемент разметки Markdown, нужно выделить
соответствующий элемент отступом в 4 пробела или 1 табуляцию.

***

**Markdown**  
```
* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third item.
```  
**Вывод**  
* This is the first list item.
* Here's the second list item.

    I need to add another paragraph below the second list item.

* And here's the third item.

***

**Markdown**  
```
* This is the first list item.
* Here's the secold list item.

    > A blockquote would look gread below the secold list item.

* And here's the third list item.
```  
**Вывод**  
* This is the first list item.
* Here's the secold list item.

    > A blockquote would look gread below the secold list item.

* And here's the third list item.

***

Вставка блоков кода обычно выделяется отступами в 4 пробела или 1 табуляцию.
Когда вставка в списке, она выделяется отступами в 8 пробелов или 2 табуляции.  
**Markdown**  
```
1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.
```  
**Вывод**  
1. Open the file.
2. Find the following code block on line 21:

        <html>
          <head>
            <title>Test</title>
          </head>

3. Update the title to match the name of your website.

***

**Markdown**  
```
1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.
```  
**Вывод**  
1. Open the file containing the Linux mascot.
2. Marvel at its beauty.

    ![Tux, the Linux mascot](/assets/images/tux.png)

3. Close the file.

***

**Markdown**  
```
1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item
```  
**Вывод**  
1. First item
2. Second item
3. Third item
    - Indented item
    - Indented item
4. Fourth item

***

## 8. Код
Для обозначения текста, как кода, используются символы обратных кавычек (\`).

| Markdown                                | HTML                                             | Вывод                               |
|-----------------------------------------|--------------------------------------------------|-------------------------------------|
| ``At the command prompt, type `nano`.`` | `At the command prompt, type <code>nano</code>.` | At the command prompt, type `nano`. |

### 8.1. Использование escape-последовательностей
Если слово или фраза, которое необходимо обозначить, как код, содержит одну или
несколько обратных кавычек, их можно проигнорировать, заключив участок текста
между двумя обратными кавычками (\`\`).

***

**Markdown**  
```
``Use `code` in your Markdown file.``
```  
**HTML**  
``<code>Use `code` in your Markdown file.</code>``  
**Вывод**  
``Use `code` in your Markdown file.``

***

### 8.2. Блоки кода
Для создания блоков кода, нужно выделить все строки кода отступом в, как
минимум, 4 пробела или 1 табуляцию.

***

**Markdown**  
```
    int main(int argc, char **argv)
    {
        return 0;
    }
```  
**Вывод**  
    int main(int argc, char **argv)
    {
        return 0;
    }

***

## 9. Горизонтальные линии
Для создания горизонтальных линий используются три и более символов "звёздочка"/
горизонтальных черт/символов подчёркивания на собственной линии.

***

**Markdown**  
```

***

---

___

```

***

Рекомендуется оставлять пустые строки между горизонтальными линиями.

## 10. Ссылки
Для создания ссылок, включите текст ссылки в квадратные скобки и, затем, введите
адрес в круглые скобки, следующие за ними.

| Markdown                                                               | Вывод                                                                |
|------------------------------------------------------------------------|----------------------------------------------------------------------|
| `My favorite search engine is [Duck Duck Go](https://duckduckgo.com).` | My favorite search engine is [Duck Duck Go](https://duckduckgo.com). |

### 10.1. Привязка "тайтлов"
К ссылкам опционально можно привязать "тайтл" ("тайтл" всплывёт, если навести на ссылку курсор). Для привязки "тайтла" используются символы двойных кавычек после адреса.

| Markdown                                                                                       | Вывод                                     |
|------------------------------------------------------------------------------------------------|-------------------------------------------|
| `My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy").` | My favorite search engine is [Duck Duck Go](https://duckduckgo.com "The best search engine for privacy"). |

### 10.2. URL и Email-адреса
Для быстрого превращения URL или Email-адреса в ссылку используются треугольные
скобки.

***

**Markdown**  
```
<https://www.markdownguide.org>
<fake@example.com>
```  
**Вывод**  
<https://www.markdownguide.org>
<fake@example.com>

***

### 10.3. Форматирование ссылок
Соответствующие примеры ниже.

***

**Markdown**  
```
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#8.Код).
```  
**Вывод**  
I love supporting the **[EFF](https://eff.org)**.
This is the *[Markdown Guide](https://www.markdownguide.org)*.
See the section on [`code`](#8.Код).

***

### 10.4.  Ссылки-сноски
Ссылки-сноски состоят из двух частей. В первой части хранятся текст ссылки и
соответствующая метка для сноски (первая часть вставляется непосредственно в
текст). Во второй части находятся метка и адрес ссылки.  
Сделано это для большего удобства чтения.

***

**Markdown**  
```
[hobbit-hole][1]
[hobbit-hole] [1]

Links:
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle "Hobbit lifestyles"
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle 'Hobbit lifestyles'
[1]: https://en.wikipedia.org/wiki/Hobbit#Lifestyle (Hobbit lifestyles)
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> "Hobbit lifestyles"
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> 'Hobbit lifestyles'
[1]: <https://en.wikipedia.org/wiki/Hobbit#Lifestyle> (Hobbit lifestyles)
```  

***

## 11. Изображения
Для того, чтобы добавить изображение, используется восклицательный знак (`!`) с
последующим размещением текста в квадратных скобках и пути/URL изображения в
круглых скобках. Дополнительно можно добавить название в двойных кавычках после
пути/URL.

***

**Markdown**  
`![The San Juan Mountains are beautiful!](/assets/images/san-juan-mountains.jpg "San Juan Mountains")`  
**Вывод**  
![The San Juan Mountains are beautiful!](/assets/images/san-juan-mountains.jpg "San Juan Mountains")

***

### 11.1. Изображение-ссылка
Для того, чтобы добавить изображение-ссылку, необходимо включить элемент
"изображение" в квадратные скобки и, затем, добавить ссылку в круглые скобки.

***

**Markdown**  
`[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)`  
**Вывод**  
[![An old rock in the desert](/assets/images/shiprock.jpg "Shiprock, New Mexico by Beau Rogers")](https://www.flickr.com/photos/beaurogers/31833779864/in/photolist-Qv3rFw-34mt9F-a9Cmfy-5Ha3Zi-9msKdv-o3hgjr-hWpUte-4WMsJ1-KUQ8N-deshUb-vssBD-6CQci6-8AFCiD-zsJWT-nNfsgB-dPDwZJ-bn9JGn-5HtSXY-6CUhAL-a4UTXB-ugPum-KUPSo-fBLNm-6CUmpy-4WMsc9-8a7D3T-83KJev-6CQ2bK-nNusHJ-a78rQH-nw3NvT-7aq2qf-8wwBso-3nNceh-ugSKP-4mh4kh-bbeeqH-a7biME-q3PtTf-brFpgb-cg38zw-bXMZc-nJPELD-f58Lmo-bXMYG-bz8AAi-bxNtNT-bXMYi-bXMY6-bXMYv)

***

## 12. Игнорирование символов
Для игнорирования символов, обрабатываемых Markdown, перед ними необходимо
вставлять символ обратной косой черты (`\`).

| Markdown                                                             | Вывод                                                              |
|----------------------------------------------------------------------|--------------------------------------------------------------------|
|`\* Without backslash, this would be a bullet in an unordered list.*` | \* Without backslash, this would be a bullet in an unordered list. |

**Список символов, разрешённых для игнорирования**

| Символ | Имя                  |
|--------|----------------------|
| `\`    | Обратная косая черта |
| \`     | Обратные кавычки     |
| `*`    | "Звёздочка"          |
| `_`    | Нижнее подчёркивание |
| `{}`   | Фигурные скобки      |
| `[]`   | Квадратные скобки    |
| `<>`   | Треугольные скобки   |
| `()`   | Круглые скобки       |
| `#`    | "Решётка"            |
| `+`    | Знак плюса           |
| `-`    | Знак минуса (дефис)  |
| `.`    | Точка                |
| `!`    | Восклицательный знак |
| `|`    | Вертикальная черта   |

## 13. HTML
Множество приложений для работы с Markdown позволяют использовать HTML-тэги в
тексте формата Markdown. Это может быть полезно, если есть необходимость
изменить какой-либо из атрибутов элемента (например, цвет текста или размер
изображения).

## 14. Расширенный синтаксис
За время развития в Markdown были добавлены такие дополнительные элементы, как
таблицы, блоки кода, подсветка синтаксиса, автоматическое связывание URL и
сноски.

### 14.1. Доступность
Не все приложения, использующие Markdown, поддерживают элементы расширенного
синтаксиса. Следовательно, рекомендуется проверить, имеется ли поддержка
расширенного синтаксиса в приложении и опция поддержки расширенного синтаксиса в
обработчике Markdown.

#### 14.1.1. Легковесные языки разметки
Существует несколько легковесных языков разметки, которые включают в себя
Markdown.  
* [CommonMark](https://commonmark.org/)
* [GitHub Flavored Markdown (GFM)](https://github.github.com/gfm/)
* [Markdown Extra](https://michelf.ca/projects/php-markdown/extra/)
* [MultiMarkdown](https://fletcherpenney.net/multimarkdown/)
* [R Markdown](https://rmarkdown.rstudio.com/)

#### 14.1.2. Обработчики языков разметки
Существует [большое количество обработчиков Markdown](https://github.com/markdown/markdown.github.com/wiki/Implementations).
Многие из них позволяют использовать расширенный синтаксис. Рекомендуется
обратиться к документации конкретного обработчика.

### 14.2. Таблицы
Для того, чтобы добавить таблицу, используются три и более дефиса `---` для
создания заголовка каждого столбца и знаки вертикальной черты для разделения
столбцом между собой.

***

**Markdown**  
```
| Syntax    | Description |
|-----------|-------------|
| Header    | Title       |
| Paragraph | Text        |
```  
**Вывод**  

| Syntax    | Description |
|-----------|-------------|
| Header    | Title       |
| Paragraph | Text        |

***

Ширина ячеек может варьироваться, но вывод будет тем же.
Также для создания таблиц в Markdown рекомендуется использовать такие
инструменты, как [Markdown Tables Generator](https://www.tablesgenerator.com/markdown_tables)
или [AnyWayData Markdown Export](https://anywaydata.com/).

#### 14.2.1. Выравнивание
Текст в столбцах можно выровнять слева, справа или по-центру, используя символ
двоеточия (`:`) слева, справа или на обоих сторонах дефисов, обозначающих
заголовок столбца.

***

**Markdown**  
```
| Syntax    | Description | Test Text   |
| :---------| :---------: | ----------: |
| Header    | Title       | Here's this |
| Paragraph | Text        | And more    |
```  
**Вывод**  

| Syntax    | Description | Test Text   |
| :---------| :---------: | ----------: |
| Header    | Title       | Here's this |
| Paragraph | Text        | And more    |

***


#### 14.2.2. Форматирование текста
Внутри таблиц позволяется форматировать текст. К примеру, можно добавлять
ссылки, вставлять код (не блоками) и выделять текст.  
Нельзя добавлять заголовки, цитаты, списки, горизонтальные линии, изображения и
большую часть тэгов HTML. Но, используя HTML, можно добавлять разрывы линий и
списки внутрь ячеек.

#### 14.2.3. Игнорирование символа прямой черты
Можно проигнорировать символ прямой черты внутри таблицы, используя код символа
в HTML (`&#124;`).

### 14.3. Выделенные блоки кода
В зависимости от используемого обработчика Markdown, для создания выделенных
блоков кода, используются три символа обратных кавычек \`\`\` или три символа
тильды `~~~` на строках до и после блока кода.

#### 14.3.1. Подсветка синтаксиса
Многие обработчики Markdown поддерживают подсветку синтаксиса для выделенных
блоков кода. Для этого нужно обозначить язык, синтаксис которого нужно
подсвечивать, сразу после первых трёх символов, открывающих выделенный блок кода
(напр.: \`\`\`json).

### 14.4. Сноски
Сноски позволяют добавлять примечания и ссылки без загромождения содержимого
документа. При создании сноски, возникает номер в верхнем индексе над тем
местом, где была создана ссылка на сноску. Читатель может нажать на ссылку и
переместиться к содержимому сноски в конце страницы.  
Для создания ссылки на сноску, нужно добавить знак вставки и идентификатор
внутрь квадратных скобок (`[^1]`). Идентификаторами могут служить цифры или
слова, но они не могут содержать пробелов и символов табуляции. Идентификаторы
только сопоставляют сноску со ссылкой на неё же - на выходе, все сноски
перечисляются последовательно.  
Для создания самой сноски используется символ вставки вместе с идентификатором
внутри квадратных скобок вместе с двоеточием и соответствующим текстом
(`[^1]: My footnote.`). Сноски не обязательно вставлять в самый конец документа
(главное - не добавлять их внутрь других элементов).

***

**Markdown**  
```
Here's a simple footnote,[^1] and here's a longer one.[^bignote]

[^1]: This is the firs footnote.

[^bignote]: Here's one with multiple paragraphs and code.
	Indent paragraphs to include them in the footnote.
	`{ my code }`
	Add as many paragraphs as you like.
```  

***

### 14.5. Идентификаторы заголовков
Множество обработчиков Markdown поддерживают пользовательские идентификаторы
заголовков - некоторые обработчики разметки автоматически добавляют их. Для
того, чтобы добавить пользовательский идентификатор заголовка, нужно заключить
идентификатор в фигурные скобки на той же строке, на которой находится
заголовок.

| Markdown                           | HTML                                       |
|------------------------------------|--------------------------------------------|
|`### My Great Heading {#custom-id}` | `<h3 id="custom-id">My Great Heading</h3>` |

#### 14.5.1. Ссылки на идентификаторы заголовков
Существует возможность создать ссылку на заголовок с идентификатором (т.н. якорная ссылка).

| Markdown                      | HTML                                     |
|-------------------------------|------------------------------------------|
| `[Heading IDs](#heading-ids)` | `<a href="#heading-ids">Heading IDs</a>` |

### 14.6. Списки определений
Некоторые обработчики Markdown позволяют создавать списки определений,
содержащие термины и соответствующие им определения. Для создания списка
определений, на следующей строке после термина вставляется двоеточие с
последующим символом пробела и определением.

***

**Markdown**  
```
First Term
: This is the definition of the first term.

Second Term
: This is one definition of the second term.
: This is another definition of the second term.
```  
**HTML**  
```
<dl>
  <dt>First Term</dt>
  <dd>This is the definition of the first term.</dd>
  <dt>Second Term</dt>
  <dd>This is one definition of the second term.</dd>
  <dd>This is another definition of the second term.</dd>
</dl>
```

***

### 14.7. Зачёркнутый текст
Имеется возможность перечёркивать текст горизонтальной линией. Делается это при
помощи двух сиволов тильда `~~` до и после слов(а), которые нужно перечеркнуть.

| Markdown                                                      | Вывод                                                       |
|---------------------------------------------------------------|-------------------------------------------------------------|
| `~~The world is flat.~~ We now know that the world is round.` | ~~The world is flat.~~ We now know that the world is round. |

### 14.8. Списки задач
Списки задач позволяют создавать списки с "чекбоксами".

***

**Markdown**  
```
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media
```  
**Вывод**  
- [x] Write the press release
- [ ] Update the website
- [ ] Contact the media

***

### 14.9. Emoji
Ниже обозначены два случая использования emoji.

#### 14.9.1. Копирование и вставка
В большинстве случаев можно скопировать и вставить emoji из источника навроде
[Emojipedia](https://emojipedia.org/).

#### 14.9.2. Использование коротких кодов emoji
Некоторые приложения, использующие Markdown, позволяют вставлять emoji по их
короткому коду. Короткий код для вставки emoji выделяется двоеточиями с обеих
сторон.

***

**Markdown**  
```
Gone camping! :tent: Be back soon.

That is so funny! :joy:
```  

***

Для этих целий можно использовать данный
[список коротких кодов emoji](https://gist.github.com/rxaviers/7360908), но,
стоит заметить, что некоторые из них могут варьироваться от приложения к
приложению.

### 14.10. Подсветка текста
Некоторые обработчики Markdown позволяют подсвечивать текст. Для этого текст
заключается между двумя символами "равно" в начале и конце.

| Markdown                                     | HTML                                                  | Вывод                                                                |
|----------------------------------------------|-------------------------------------------------------|----------------------------------------------------------------------|
|`I need to highlight these ==very important words==.` | `I need to highlight these <mark>very important words</mark>.` | I need to highlight these ==very important words==. |

### 14.11. Индексация символов
Некоторые обработчики Markdown позволяют индексировать один или несколько
символов.

#### 14.11.1. Нижняя
Для нижней индексации символов используется символ тильды до и после
индексирующих символов.

| Markdown | HTML             | Вывод          |
|----------|------------------|----------------|
| `H~2~O`  | `H<sub>2</sub>O` | H<sub>2</sub>O |

#### 14.11.2. Верхняя
Для верхней индексации символов используется символ вставки до и после
индексирующих символов.

| Markdown | HTML            | Вывод         |
|----------|-----------------|---------------|
| `X^2^`   | `X<sup>2</sup>` | X<sup>2</sup> |

### 14.12. Автоматическое связывание URL
Многие обработчики Markdown умеют автоматически создавать ссылки. К примеру,
если ввести `http://www.example.com`, некоторые обработчики автоматически
превратят адрес в ссылку несмотря на то, что не были использованы скобки.  
Для того, чтобы это предотвратить, рекомендуется заключать адрес в обратные
кавычки.