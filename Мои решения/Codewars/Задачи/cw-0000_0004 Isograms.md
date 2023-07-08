|                 |          |           |
| --------------- | -------- | --------- |
| Название        | Isograms | Изограммы | 
| Отзыв[^отзыв]   |          |           |
| Ссылка[^ссылка] |          |           |

# Задача

> ## Оригинал
> An isogram is a word that has no repeating letters, consecutive or non-consecutive. Implement a function that determines whether a string that contains only letters is an isogram. Assume the empty string is an isogram. Ignore letter case.
> 
> **Example: (Input --> Output)**
> 
> "Dermatoglyphics" --> true "aba" --> false "moOse" --> false (ignore letter case)
> 
> ```fsharp
> isIsogram "Dermatoglyphics" = true
> isIsogram "moose" = false
> isIsogram "aba" = false
> ```

> ## Перевод
> Изограмма — это слово, в котором нет повторяющихся букв, последовательных или непоследовательных. Реализуйте функцию, определяющую, является ли строка, содержащая только буквы, изограммой. Предположим, что пустая строка является изограммой. Игнорируёте регистр букв.
> 
> **Пример: (Ввод --> Вывод)**
> 
> "Dermatoglyphics" --> true "aba" --> false "moOse" --> false (игнорируется регистр букв)
> 
> ```fsharp
> isIsogram "Dermatoglyphics" = true
> isIsogram "moose" = false
> isIsogram "aba" = false
> ```

# Начальный код

```haskell
module Isogram where

isIsogram :: String -> Bool
```

# Решение

## Моё:

```haskell
module Isogram where

import Data.Char (toLower)

isIsogram :: String -> Bool
isIsogram str = test lowerStr
  where
    lowerStr = map toLower str
    test [] = True
    test (x:xs) = (lengthChar x lowerStr == 1) && test xs
      where
        lengthChar x = length . filter (== x)
```

## Лучшее:

```haskell
module Isogram where
import Data.Char (toLower)

isIsogram :: String -> Bool
isIsogram = unique . map toLower
  where unique []     = True
        unique (x:xs) = x `notElem` xs && unique xs
```


[^отзыв]:**Отзыв**
	> Задача на вычисление дубликатов в массиве. Это наглядный экземпляр стандартного алгоритмического задания, которое в разных вариациях часто встречается в упражнениях почти на всех языках. Здесь же можно опробовать её на Хаскеле и сравнить (на деле или интуитивно) с тем, как бы это решалось на остальных языках.
	> 
	> Как и почти во всех классических задачах, тут есть простор для фантазии, несмотря на простоту описания. Можно решать как банальными конструкциями, а можно попытаться найти что-то изящное :)

[^ссылка]: **Ссылка**
	- [Isograms](https://www.codewars.com/kata/isograms/)