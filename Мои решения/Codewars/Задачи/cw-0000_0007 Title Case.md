|                 |            |                   |
| --------------- | ---------- | ----------------- |
| Название        | Title Case | Регистр заголовка |
| Отзыв[^отзыв]   |            |                   | 
| Ссылка[^ссылка] |            |                   |

# Задача

> ## Оригинал
> A string is considered to be in title case if each word in the string is either (a) capitalised (that is, only the first letter of the word is in upper case) or (b) considered to be an exception and put entirely into lower case unless it is the first word, which is always capitalised.
> 
> Write a function that will convert a string into title case, given an optional list of exceptions (minor words). The list of minor words will be given as a string with each word separated by a space. Your function should ignore the case of the minor words string -- it should behave in the same way even if the case of the minor word string is changed.
> 
> ### Arguments (Haskell)
> 
> - **First argument**: space-delimited list of minor words that must always be lowercase except for the first word in the string.
> - **Second argument**: the original string to be converted.
> 
> ### Arguments (Other languages)
> 
> - **First argument (required)**: the original string to be converted.
> - **Second argument (optional)**: space-delimited list of minor words that must always be lowercase except for the first word in the string. The JavaScript/CoffeeScript tests will pass `undefined` when this argument is unused.
> 
> ### Example
> 
> ```haskell
> titleCase "a an the of" "a clash of KINGS" -- should return: "A Clash of Kings"
> titleCase "The In" "THE WIND IN THE WILLOWS" -- should return: "The Wind in the Willows"
> titleCase "" "the quick brown fox" -- should return: "The Quick Brown Fox"
> ```
> 

> ## Перевод
> Строка считается заглавной, если каждое слово в строке либо (а) написано заглавной буквой (то есть только первая буква слова в верхнем регистре), либо (б) считается исключением и полностью помещается в строчными буквами, если только это не первое слово, которое всегда пишется с большой буквы.
> 
> Напишите функцию, которая преобразует строку в заглавный регистр, учитывая необязательный список исключений (второстепенные слова). Список второстепенных слов будет представлен в виде строки, где каждое слово отделено пробелом. Ваша функция должна игнорировать регистр строки второстепенных слов — она должна вести себя так же, даже если регистр строки второстепенных слов изменен.
> 
> ### Аргументы (Хаскель)
> 
> - **Первый аргумент** : список второстепенных слов, разделенных пробелами, которые всегда должны быть в нижнем регистре, за исключением первого слова в строке.
> - **Второй аргумент** : исходная строка для преобразования.
> 
> ### Аргументы (другие языки)
> 
> - **Первый аргумент (обязательный)** : исходная строка для преобразования.
> - **Второй аргумент (необязательный)** : список второстепенных слов, разделенных пробелами, которые всегда должны быть в нижнем регистре, за исключением первого слова в строке. Тесты JavaScript/CoffeeScript будут пройдены, `undefined`если этот аргумент не используется.
> 
> ### Пример
> 
> ```haskell
> titleCase "a an the of" "a clash of KINGS" -- should return: "A Clash of Kings"
> titleCase "The In" "THE WIND IN THE WILLOWS" -- should return: "The Wind in the Willows"
> titleCase "" "the quick brown fox" -- should return: "The Quick Brown Fox"
> ```
> 

# Начальный код

```haskell
module TitleCase (titleCase) where

titleCase :: String -> String -> String
titleCase minor title = undefined
```

# Решение

## Моё:

```haskell
module TitleCase (titleCase) where

import Data.Char (toUpper, toLower)

titleCase :: String -> String -> String
titleCase ""    title = unwords $ map capitalize $ words title
titleCase minor title = unwords $ capitalize title_w : map helper title_ws
  where
    (title_w:title_ws) = words $ toLowerStr title
    minors_w = words $ toLowerStr minor
    helper x = if x `elem` minors_w
                        then x
                        else capitalize x

capitalize :: String -> String
capitalize (x:xs) = toUpper x : toLowerStr xs

toLowerStr :: String -> String
toLowerStr = map toLower
```

## Лучшее:

```haskell
module TitleCase (titleCase) where

import Data.List (find)
import Data.Char (toUpper, toLower)

capitalize :: String -> String
capitalize (c:cs) = toUpper c : map toLower cs
capitalize     [] = []

titleCase :: String -> String -> String
titleCase minor = unwords . process . words
  where 
    process :: [String] -> [String]
    process [] = []
    process (w:ws) = capitalize w : map checkNotMinor ws

    checkNotMinor :: String -> String
    checkNotMinor w = maybe (capitalize w) id $ find (== normalize w) normalizedMinors
    
    normalizedMinors :: [String]
    normalizedMinors = map normalize (words minor)

    normalize :: String -> String
    normalize = map toLower
```


[^отзыв]:**Отзыв**
	> Кульминация базовых тренировок, где необходимо уметь работать и с символами, и со строками, и со списками. Задача, которая действительно может встретиться в боевых условиях, и которая позволит показать навыки написания "читаемого" кода. Здесь есть возможность, как для явной рекурсии, так и для использования стандартных функций высшего порядка, есть интересное требование замены буквы на заглавный аналог и условие, когда вообще ничего делать не надо :)

[^ссылка]: **Ссылка**
	- [Title case](https://www.codewars.com/kata/title-case)