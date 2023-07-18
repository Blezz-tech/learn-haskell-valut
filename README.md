[Ссылка на сайт откуда был взят курс](https://coda.io/@metalamp/education/back-end-3)

Основная цель - сделать бота из [Задания 3](https://coda.io/@metalamp/education/3-14)

- [[Полезные ресурсы]]
- [[Отчеты]]

# Итого пройдено:

- [x] ghcup
	- [x] ghc
	- [x] cabal
	- [x] haskell language sever
	- [x] stack
- [x] О Haskell по-человечески
- [x] Выполнение обязательных ката на codewars (Задание 1)
- [x] 
- [x] 
- [x] 

- codewars х[Профиль codewars](https://www.codewars.com/users/Blezz-tech)

---
# Задание 1.1 Первичная теория

- [ ] [Learn You a Haskell for Great Good!](http://learnyouahaskell.com/chapters)
	- [x] [Introduction](http://learnyouahaskell.com/introduction
	- [x] [Starting Out](http://learnyouahaskell.com/starting-out)
	- [x] [Types and Typeclasses](http://learnyouahaskell.com/types-and-typeclasses)
	- [x] [Syntax in Functions](http://learnyouahaskell.com/syntax-in-functions)
	- [x] [Recursion](http://learnyouahaskell.com/recursion)
	- [x] [Higher Order Functions](http://learnyouahaskell.com/higher-order-functions)
	- [x] [Modules](http://learnyouahaskell.com/modules)
	- [x] [Making Our Own Types and Typeclasses](http://learnyouahaskell.com/making-our-own-types-and-typeclasses)
	- [x] [Input and Output](http://learnyouahaskell.com/input-and-output)
	- [ ] [Functionally Solving Problems](http://learnyouahaskell.com/functionally-solving-problems)
	- [ ] [Functors, Applicative Functors and Monoids](http://learnyouahaskell.com/functors-applicative-functors-and-monoids)
	- [ ] [A Fistful of Monads](http://learnyouahaskell.com/a-fistful-of-monads)
	- [ ] [For a Few Monads More](http://learnyouahaskell.com/for-a-few-monads-more)
	- [ ] [Zippers](http://learnyouahaskell.com/zippers)


---
# Задание 1.2 Первичная практика

- [ ] Выполнение не обязательных ката на codewars
	- [ ] [[cw-0000_0008 Valid Braces]]
	- [ ] [[cw-0000_0009 Product of consecutive Fib numbers]]
	- [ ] [[cw-0000_0010 Reverse words]]
	- [ ] [Snail](https://www.codewars.com/kata/snail/haskell) **неизвестно** мин^[Интересная с задача с простым условием, для которой сразу понятен императивный алгоритм с вложенными циклами, но не сразу — функциональный.
		Помечена как 4-ый кью, но на самом деле достаточно первых глав LYAH и умения работать со списками.]
	- [ ] [Equal sides of array](https://www.codewars.com/kata/equal-sides-of-an-array/train/haskell) **неизвестно** мин^[В задаче нужно найти индекс элемента в списке, где сумма элементов списка слева будет равна сумме элементов списка справа от найденного элемента. Если же такого элемента нет, то вывести -1.
		В этой кате можно отработать работу со списками, поискать вспомогательные функции в модуле Data.List или же просто посмотреть интересные решение других людей.]
	- [ ] [Go so far around to the right that you end up left](https://www.codewars.com/kata/5424e78460d77749f2000279) **неизвестно** мин^[Необходимо реализовать левую свертку через правую. Для решения нужно ознакомиться с реализацией обеих сверток и хорошо понимать, как работает каждая из них.
		Для решения нужно хорошо разобраться в принципе работы обеих сверток, так как использовать reverse = читерить.]
	- [ ] [Take a Ten Minute Walk](https://www.codewars.com/kata/54da539698b8a2ad76000228) **неизвестно** мин^[Нужно проверить предложенный маршрут (движение по сторонам света) на два условия: длительность (10 минут при минуте на одно перемещение) и совпадение начальной и конечной точки (вернуться туда, откуда пришёл).
		Тренирует работу со списками или использование Data.List.]
	- [ ] [Highest Rank Number in an Array](https://www.codewars.com/kata/5420fc9bb5b2c7fd57000004/haskell) **неизвестно** мин^[Небольшая ката для практики бесточечного стиля и работы со стандартными модулями типа Data.List, Data.Ord и т.д. на ваш выбор.]
	- [ ] [Duplicate Encoder](https://www.codewars.com/kata/54b42f9314d9229fd6000d9c) **неизвестно** мин^[Простая ката, нацеленная на поиск дубликатов в массиве, что часто встречается в реальных задачах.]
	- [ ] [Next bigger number with the same digits](https://www.codewars.com/kata/55983863da40caa2c900004e) **неизвестно** мин^[Ката с очевидным брутфорс-решением. Попытайтесь найти наиболее оптимальный алгоритм, потому как если написать слишком просто, то все тесты пройти не успеет.]
	- [ ] [Find The Parity Outlier](https://www.codewars.com/kata/5526fc09a1bbd946250002dc/haskell) **неизвестно** мин^[У FindOutlier множестово разных решений функциями из Data.List, или можно в лоб, сверткой, тренирует паттерн матчинг и функции как объекты первого класса.]
	- [ ] [Most frequently used words in a text](https://www.codewars.com/kata/51e056fe544cf36c410000fb/haskell) **неизвестно** мин^[Достаточно простая ката для 4 кью. Тренирует обработку строки с использованием Data.Char и Data.List.]
	- [ ] [Fibonacci, Tribonacci and friends](https://www.codewars.com/kata/556e0fccc392c527f20000c5/haskell) **неизвестно** мин^[Логическое продолжение каты Tribonacci, достаточно интересное и неординарное решение, тренирует мозги.]
	- [ ] [Sortable Shapes](https://www.codewars.com/kata/586669a8442e3fc307000048) **неизвестно** мин^[Это простая ката 6 кью (30 минут на решение достаточно) позволит Вам потренироваться в создании пользовательского типа данных. Основной результат - это понимание реализации каких классов нужно предусмотреть для созданного типа, чтобы данные могли отправляться в функцию sort.]
	- [ ] [Recurrence relations](https://www.codewars.com/kata/recurrence-relations/haskell) **неизвестно** мин
	- [ ] [Simple Fun #74: Growing Plant](https://www.codewars.com/kata/58941fec8afa3618c9000184) **неизвестно** мин
	- [ ] [Coloured Triangles](https://www.codewars.com/kata/coloured-triangles) **неизвестно** мин
	- [ ] [Digital Root](https://www.codewars.com/kata/541c8630095125aba6000c00) **неизвестно** мин
	- [ ] [Twice linear](https://www.codewars.com/kata/5672682212c8ecf83e000050/train/haskell) **неизвестно** мин
	- [ ] [Playing with laziness](https://www.codewars.com/kata/5516b80d891547c9b50007fd/haskell) **неизвестно** мин
	- [ ] [Break camelCase](https://www.codewars.com/kata/5208f99aee097e6552000148) **неизвестно** мин
	- [ ] [CamelCase Method](https://www.codewars.com/kata/587731fda577b3d1b0001196) **неизвестно** мин
	- [ ] [Speed Control](https://www.codewars.com/kata/speed-control/haskell) **неизвестно** мин

---
# Более глубокая теория
## Обязательно

- [ ] [учебник чуть более глубоко описывающий Haskell](https://anton-k.github.io/ru-haskell-book/book/home.html).^[Позволяет понять многие теоретические моменты. Обязательны к прочтению главы 1-9, остальные по желанию.]
- [ ] видео-курс на степик от Дениса Москвина. (Ниже разбит на части)
	- Шпаргалка по Решениям (Если прям долго не получается и чтобы не тянуть время)
		- [1](https://github.com/rgordeev/functional_programming_in_haskell)
		- [2](https://github.com/vvscode/hs--stepic-fp-with-haskell/tree/master)
- [ ] [Функциональное программирование на языке Haskell](https://stepik.org/course/75/).^[первая часть курса, очень системный и развернутый материал по Haskell. Она обязательна к изучению.]
	- [x] Введение
	- [x] Основы программирования
	- [ ] Списки
		- [x] [3.1 Функции для работы со списками](https://stepik.org/lesson/8326/step/1?unit=1474)
		- [x] [3.2 Функции высших порядков над списками](https://stepik.org/lesson/12321/step/1?unit=2785)
		- [ ] [3.3 Генераторы списков](https://stepik.org/lesson/8328/step/1?unit=1476)
		- [ ] [3.4 Правая свертка](https://stepik.org/lesson/4745/step/1?unit=1081)
		- [ ] [3.5 Левая свертка и ее сравнение с правой](https://stepik.org/lesson/5790/step/1?unit=1136)
		- [ ] [3.6 Родственные сверткам функции](https://stepik.org/lesson/6196/step/1?unit=1229)
	- [ ] Типы данных
		- [ ] [4.1 Типы перечислений](https://stepik.org/lesson/4916/step/1?unit=1082)
		- [ ] [4.2 Типы произведений и сумм произведений](https://stepik.org/lesson/4985/step/1?unit=1083)
		- [ ] [4.3 Синтаксис записей](https://stepik.org/lesson/5431/step/1?unit=1132)
		- [ ] [4.4 Типы с параметрами](https://stepik.org/lesson/5746/step/1?unit=1256)
		- [ ] [4.5 Рекурсивные типы данных](https://stepik.org/lesson/7009/step/1?unit=1472)
		- [ ] [4.6 Синонимы и обертки для типов](https://stepik.org/lesson/7602/step/1?unit=1473)
	- [ ] Монады
		- [ ] [5.1 Класс типов Functor и законы для него](https://stepik.org/lesson/8432/step/1?unit=2743)
		- [ ] [5.2 Определение монады](https://stepik.org/lesson/8437/step/1?unit=1572)
		- [ ] [5.3 Монада Identity](https://stepik.org/lesson/8438/step/1?unit=1573)
		- [ ] [5.4 Список и Maybe как монады](https://stepik.org/lesson/8439/step/1?unit=1574)
		- [ ] [5.5 Монада IO](https://stepik.org/lesson/8443/step/1?unit=1578)
		- [ ] [5.6 Монада Reader](https://stepik.org/lesson/8441/step/1?unit=1576)
		- [ ] [5.7 Монада Writer](https://stepik.org/lesson/8442/step/1?unit=1577)
		- [ ] [5.8 Монада State](https://stepik.org/lesson/8444/step/1?unit=1579)
- [ ] [Функциональное программирование на языке Haskell (часть 2)](https://stepik.org/course/693/).^[2-я часть курса, она уже необязательна. Материал тут достаточно сложный, его рекомендуем изучать после того, как сделаны первые версии бота и сервера, чтобы закрепить полученные на практике знания и расширить/углубить их.]
	- [ ] Аппликативные функторы
		- [ ] [1.1 Определение аппликативного функтора](https://stepik.org/lesson/28880/step/1?unit=9912) ≈ 2 ч 3 мин
		- [ ] [1.2 Представители класса типов Applicative](https://stepik.org/lesson/30424/step/1?unit=11041) ≈ 1 ч 34 мин
		- [ ] [1.3 Аппликативный парсер Parsec](https://stepik.org/lesson/42245/step/1?unit=20509) ≈ 43 мин
		- [ ] [1.4 Аппликативный парсер своими руками](https://stepik.org/lesson/30425/step/1?unit=11042) ≈ 1 ч 51 мин
		- [ ] [1.5 Композиция на уровне типов](https://stepik.org/lesson/30426/step/1?unit=11043) ≈ 1 ч 15 мин
	- [ ] Управление эффектами
		- [ ] [2.1 Класс типов Foldable](https://stepik.org/lesson/30427/step/1?unit=11044) ≈ 1 ч 41 мин
		- [ ] [2.2 Класс типов Traversable](https://stepik.org/lesson/30428/step/1?unit=11045) ≈ 1 ч 47 мин
		- [ ] [2.3 Законы и свойства класса Traversable](https://stepik.org/lesson/31555/step/1?unit=11808) ≈ 1 ч 44 мин
		- [ ] [2.4 Связь классов Monad и Applicative](https://stepik.org/lesson/28881/step/1?unit=9913) ≈ 1 ч 32 мин
		- [ ] [2.5 Классы типов Alternative и MonadPlus](https://stepik.org/lesson/30721/step/1?unit=11244) ≈ 57 мин
	- [ ] Монады и эффекты
		- [ ] [3.1 Монада Except](https://stepik.org/lesson/30722/step/1?unit=11809) ≈ 1 ч 18 мин
		- [ ] [3.2 Монада Cont](https://stepik.org/lesson/30723/step/1?unit=11811) ≈ 57 мин
		- [ ] [3.3 Трансформеры монад](https://stepik.org/lesson/31556/step/1?unit=11810) ≈ 46 мин
		- [ ] [3.4 Трансформер ReaderT](https://stepik.org/lesson/38577/step/1?unit=17396) ≈ 1 ч 46 мин
	- [ ] Трансформеры монад
		- [ ] [4.1 Трансформер WriterT](https://stepik.org/lesson/38578/step/1?unit=20503) ≈ 1 ч 23 мин
		- [ ] [4.2 Трансформер StateT](https://stepik.org/lesson/38579/step/1?unit=20504) ≈ 1 ч 4 мин
		- [ ] [4.3 Трансформер ExceptT](https://stepik.org/lesson/38580/step/1?unit=20505) ≈ 1 ч 0 мин
		- [ ] [4.4 Неявный лифтинг](https://stepik.org/lesson/38581/step/1?unit=20506) ≈ 57 мин
		- [ ] [4.5 Задачи на трансформеры](https://stepik.org/lesson/45331/step/1?unit=23645) ≈ 5 мин
- [ ] [Typeclassopedia](https://wiki.haskell.org/Typeclassopedia). **неизвестно** мин^[системное описание почти всех самых популярных тайпклассов]

## Необязательно

- [ ] Очень рекомендуется: книга для начинающих с хорошим практическим уклоном Get Programming with Haskell (W. Kurt).^[Т.к. эта книга не доступна бесплатно, мы не включили её в обязательную часть, но очень рекомендуем. Здесь есть очень приближенные к реальным задачи, с помощью которых вы можете быстро и эффективно начать писать свои приложения, вроде бота. Книга максимально свежая и актуальная, хорошо написана. Практика показала, что изучающие её в рамках нашей программы потом её активно хвалили :)]
- [ ] сделать упражнения из глав [Real World Haskell](http://book.realworldhaskell.org/), которые помогут освоиться с приближенными к реальным задачам.
- [ ] По желанию: часто рекомендуемая многими новичками книга [http://haskellbook.com/](http://haskellbook.com/).
- [ ] По желанию: [видео-курс от Николая Кудасова](https://www.youtube.com/watch?v=jNQVa5INdDk&list=PLov3NSwpY86cfkfXyVroSZkHemxoAdnrd&index=1).
- [ ] По желанию: Write Yourself a Scheme in 48 Hours.-     
	Упражнение по написанию простого интерпретатора для языка Scheme (язык, с которого был слизан JavaScript). [https://en.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours](https://en.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours)
	
	Есть так же перевод на русский (там могут быть не все части или неактуальные данные): [https://ru.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours](https://ru.wikibooks.org/wiki/Write_Yourself_a_Scheme_in_48_Hours)
	
	Очень рекомендую пройти, на самом деле туториал довольно небольшой, но дает хороший пример написания средних по размеру програм, в то время как почти все остальные туториалы нацелены на примеры совсем тривиальных вещей в один-два файла.
- [ ] [Выводы и ссылки на рецензии о современных книгах по Haskell](https://medium.com/@_bravit/%D0%BA%D0%BD%D0%B8%D0%B3%D0%B8-%D0%BF%D0%BE-%D0%BF%D1%80%D0%BE%D0%B3%D1%80%D0%B0%D0%BC%D0%BC%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8E-%D0%BD%D0%B0-haskell-%D0%B2%D1%8B%D0%B2%D0%BE%D0%B4%D1%8B-712c1f5b7749).
- [ ] Статьи по различным темам, которые могут оказаться полезными для понимания того или иного материала
	- [ ] [Pitfalls in Haskell](http://web.archive.org/web/20150505013645/http://users.jyu.fi:80/~sapekiis/haskell-pitfalls/)
	- [ ] [Thinking Functionally with Haskell](https://pragprog.com/magazines/2012-09/thinking-functionally-with-haskell)
	- [ ] [Функторы, монады и аппликативы в картинках](https://habr.com/post/183150/)
	- [ ] [Три полезные монады (в картинках)](https://habr.com/post/184722/)
	- [ ] [«Страшные» абстракции Haskell без математики и без кода (почти). Часть I](https://habr.com/post/272115/)
	- [ ] [Моноиды, полугруппы и все-все-все](https://habr.com/company/jugru/blog/340178/). Оригинал [тут](http://blog.ploeh.dk/2017/10/04/from-design-patterns-to-category-theory/)

---
# Задание 2: задачки по языку

- [ ] Рекомендуемые каты
	- [ ] [Бесконечные структуры](https://www.codewars.com/kata/functional-streams)
	- [ ] [Создание своих инстансов для 5 базовых монад](https://www.codewars.com/kata/five-fundamental-monads)
	- [ ] [Монадный стек Maybe + List + State](https://www.codewars.com/kata/escape-the-mines-or-die)
	- [ ] [Представление структур данных из функций](https://www.codewars.com/kata/scott-encoding/train/haskell).^[Практически любой тип данных можно представить даже в языке без специальных синтаксических конструкций, если этот язык поддерживает функции высшего порядка и замыкания. Haskell как раз имеет специальные синтаксические конструкции для создания алгебраических типов данных, однако на замену им могут прийти простые функции. Как с их помощью сэмулировать пары, Maybe и даже списки как раз продемонстрирует эта ката.
		  .
		  Также для закрепления концепции алгебраических типов данных рекомендую подглаву 2.1 книги SICP, там этот подход отлично описан. Саму книгу в целом тоже рекомендую в дальнейшем прочесть, хотя многие темы там уже по продвинутым темам.]
	- [ ] [Изоморфизм (на самом деле довольно простая и интересная ката)](https://www.codewars.com/kata/isomorphism)
- [ ] Необязательные каты
	- [ ] [Алгебраические изоморфизмы (после каты Изоморфизм)](https://www.codewars.com/kata/algebraic-isomorphism/haskell)
	- [ ] [Синглтоны](https://www.codewars.com/kata/54750ed320c64c64e20002e2).^[Несложная ката, решив которую можно познакомиться с зависимыми типами. Несмотря на то, что в Хаскеле на данный момент зависимых типов нет, последние можно сымитировать при помощи некоторых расширений ghci и типов-синглтонов - типов, имеющих только одно значение.]
	- [ ] [Корутины](https://www.codewars.com/kata/547a77a6b84a1fb8bf000211)
	- [ ] [Lens](https://www.codewars.com/kata/54258ffb430ca2e4b5000239)
	- [ ] [Простой компилятор](https://www.codewars.com/kata/5265b0885fda8eac5900093b)
	- [ ] Обязательно попробуйте найти и пройти еще от 3-х кат (1, 2 или 3 kyu) самостоятельно.

---
# Задание 3: бот

Нужно написать эхо-бота, который умеет просто отправлять сообщение от пользователя ему же в ответ.

Бот должен уметь работать с сообщениями через несколько механизмов доставки:

- консоль: сообщение пользователя вводится со стандартного ввода, ответ бота выводится в стандартный вывод (например, с помощью [getLine](https://hackage.haskell.org/package/base-4.16.0.0/docs/Prelude.html#v:getLine) и [putStrLn](https://hackage.haskell.org/package/base-4.16.0.0/docs/Prelude.html#v:putStrLn)).
- Telegram: [https://core.telegram.org/bots/api#poll](https://core.telegram.org/bots/api#poll)
- Вместо Telegram можно выбрать VK (см. [документацию](https://vk.com/dev/bots_longpoll)) или Slack.

## Функциональные требования

1. Пользователь может отправить команду /help и увидеть текст, описывающий бота.
2. Пользователь может отправить команду /repeat, и в ответ бот отправит, какое сейчас выбрано значение повторов и вопрос, сколько раз повторять сообщение в дальнейшем. К вопросу будут прилагаться кнопки для выбора ответа (кнопки с цифрами от 1 до 5). После выбора пользователем все ответы бота должны дублировать сообщение пользователя указанное кол-во раз. Кол-во повторов должно быть индивидуальным для каждого пользователя, т. е. если один пользователь выбрал 3 повторения, то второму мы по-прежнему показываем начальное кол-во сообщений.
3. Все должно быть максимально кастомизируемо через конфиги:
	1.  Сообщение, отправляемое в ответ на /help.
	2.  Вопрос по команде /repeat.
	3.  Начальное кол-во повторов на каждый ответ.
4. Бот должен уметь повторять только текстовые сообщения и какой-нибудь один вид мультимедийных сообщений (например, стикеры или картинки). Остальные виды сообщений можно игнорировать. Конечно, этот пункт не распространяется на сообщения из консоли.

## Технические требования

1. Можно взять за основу [шаблон проекта](https://github.com/fullstack-development/haskell-internship/tree/master/echo-bot-template). Он содержит "скелет" логики бота и некоторые тесты. Запустите stack test и попробуйте исправить логику, чтобы тесты начали проходить. Шаблон можно как угодно править по своему усмотрению, а можно не использовать совсем.
2. Для основного кода проекта (кроме тестов) использовать только библиотеки из стандартной поставки [Haskell Platform](https://coda.io/d/_dXh0LxbfZxo/_suHtD) и три сторонние:
	1. Для отправки http-запросов
	2.  Для парсинга json
	3.  Для работы с конфигом.
3. Все остальное должно быть сделано по максимуму без библиотек. Для тестов можете использовать любой удобный вам инструмент (hspec, HUnit, etc).
4. Обновления от Телеграма получать не посредством веб-хуков, а посредством поллинга. Отправлять запрос за апдейтами телеграму, тот сам будет ставить ответ на паузу, если обновок нет, и отвечать сразу, как только что-то появилось. Ну или отвечать пустым массивом по таймауту. Это требование вкупе с тем, что в следующем задании надо будет свой сервер на Warp реализовать, поможет лучше понять, что такое модель поллинга и модель пуша (через веб-хуки), в чем преимущества и недостатки каждой из моделей.
5. Результатом должно быть одно приложение, а не два. В каком режиме его запускать (Telegram или консоль), определяется параметром в конфиге или опцией командной строки.

## Следующие технические требования также распространяются и на следующее задание "Веб-сервер"

1. Проект должен быть в отдельном репозитории на github, во время выполнения задания коммиты делать как можно чаще, как минимум раз в день, когда написана хоть строчка кода.
2. Использовать [stack](https://www.haskellstack.org/), все используемые библиотеки должны быть зафиксированы в файле package.yaml, сам проект должен быть инициирован командой stack new, которая создает базовую структуру Haskell-проекта.
3. Для разворачивания должно быть достаточно клонирования репозитория и запуска stack build. Обязательно проверить это правило клонированием репозитория в отдельную папку у себя и запуска stack build — результатом должны быть собранные и рабочие бинарники.
4. У каждого проекта должно быть README с описанием того, как разворачивать проект локально и как его запускать, а так же с описанием базовой структуры, чтобы новичок мог легко разобраться (представьте, что после вас проект будет поддерживать совсем нулевой джуниор). Все должно быть на английском.
5. Проект должен иметь файл .gitignore, куда внесены все автогенерируемые файлы проекта, локальные конфиги и т.д. Обязательно добавьте туда следующие папки (даже если вы не пользуетесь редактором VSCode, им пользуемся мы и это правило для нашего удобства при проверке):
	- .vscode
	- .history
6. Проект должен быть покрыт unit-тестами, которые бы покрывали главные use-case каждого модуля в приложении.
7. Конфиги должны быть вынесены в отдельный файл с возможностью переписать локально какие-нибудь значения, но не изменять файлы из git-репозитория, чтобы случайно не запушить пароль или токен.
8. Проект должен поддерживать логи разных уровней, все ключевые моменты должны грамотно логироваться, логи должны легко конфигурироваться хотя бы так, чтобы можно было включать/выключать логи до определенного уровня (например, показывать все от DEBUG и выше, или показывать все от WARN и выше).
9. Для понятной архитектуры рекомендуем использовать [Handle Pattern](https://jaspervdj.be/posts/2018-03-08-handle-pattern.html), так как мы применяем его в большинстве своих проектов.
10. Чтобы добиться понятной архитектуры проекта, и получить тестируемый код, также можно применять различные техники (паттерны) описанные сообществом:
	- [The Service Pattern](https://www.schoolofhaskell.com/user/meiersi/the-service-pattern)
	- [The ReaderT Design Pattern (Discussion)](https://www.fpcomplete.com/blog/2017/06/readert-design-pattern)
	- [Three Layer Haskell Cake](https://www.parsonsmatt.org/2018/03/22/three_layer_haskell_cake.html)
12. Полезно почитать требования к проекту из задания 5 (код-ревью). На старте проекта необязательно забивать себе ими голову — потом успеете, но, все-таки, если знать их заранее, придется меньше исправлять.

## Источники

- Для начала можно посмотреть [простую статью](https://www.bekk.christmas/post/2019/23/making-a-small-haskell-application) про то, как начать собирать первое приложение по отправке HTTP-запроса и получению одного нужного поля из JSON
- [Designing Testable Components](http://felixmulder.com/writing/2019/10/05/Designing-testable-components.html)
- Полезные статьи для данного задания:
- [Telegram-бот на Python: от первой строчки до запуска на Heroku](https://web.archive.org/web/20210120102233/https://tproger.ru/translations/telegram-bot-create-and-deploy/amp/)
	- [https://artyom.me/aeson](https://artyom.me/aeson)
	- [https://ruhaskell.org/posts/packages/2015/02/03/aeson-hello-world.html](https://ruhaskell.org/posts/packages/2015/02/03/aeson-hello-world.html)
	- [https://ruhaskell.org/posts/packages/2015/03/05/aeson-next.html](https://ruhaskell.org/posts/packages/2015/03/05/aeson-next.html)

---

# Задание 4 Сайт (Пока не перенесено)

# Задание 5 Ревью

не будет пока не сделаю задания 3 и 4

# Задание 6 От себя

Что нужно будет сделать когда будет время

- [ ] Пройти ВСЕ Haskell ката на codewars 
- [ ] [Прочесть Error vs. Exception - HaskellWiki](https://wiki.haskell.org/Error_vs._Exception)
- [ ] [Блог Нила Митчелла (Haskell и т. д.): В погоне за утечкой пространства при встряхивании](http://neilmitchell.blogspot.com/2013/02/chasing-space-leak-in-shake.html)
- [ ] GHC.Base
	- [ ] Понять исходный код этих функций
		- [base: Basic libraries](https://hackage.haskell.org/package/base)
- [ ] Прочитать и понять monomorphism restriction
	- [ ] https://wiki.haskell.org/Monomorphism_restriction
	- [ ] https://stackoverflow.com/questions/32496864/what-is-the-monomorphism-restriction
- [ ] Прочитать про бесточечный стиль
	- [ ] https://wiki.haskell.org/Pointfree
- [ ] Разобраться как работает [[Очень интересный парсер]]
