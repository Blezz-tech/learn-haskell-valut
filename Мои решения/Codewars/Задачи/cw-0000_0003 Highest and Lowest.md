|                 |                    |                              |
| --------------- | ------------------ | ---------------------------- |
| Название        | Highest and Lowest | Самый высокий и самый низкий |
| Отзыв[^отзыв]   |                    |                              |
| Ссылка[^ссылка] |                    |                              |

# Задача

> ## Оригинал
> In this little assignment you are given a string of space separated numbers, and have to return the highest and lowest number.
> 
> ### Examples
> 
> ```haskell
> highAndLow "1 2 3 4 5")  # return "5 1"
> highAndLow "1 2 -3 4 5") # return "5 -3"
> highAndLow "1 9 3 4 -5") # return "9 -5"
> ```
> 
> ### Notes
> 
> - All numbers are valid `Int32`, no _need_ to validate them.
> - There will always be at least one number in the input string.
> - Output string must be two numbers separated by a single space, and highest number is first.

> ## Перевод
> В этом небольшом задании вам дается строка чисел, разделенных пробелами, и вы должны вернуть наибольшее и наименьшее число.
> 
> ### Примеры
> 
> ```haskell
> highAndLow "1 2 3 4 5")  # return "5 1"
> highAndLow "1 2 -3 4 5") # return "5 -3"
> highAndLow "1 9 3 4 -5") # return "9 -5"
> ```
> 
> ### Примечания
> 
> - Все номера действительны `Int32`, подтверждать их не _нужно ._
> - Во входной строке всегда будет хотя бы одно число.
> - Выходная строка должна состоять из двух чисел, разделенных одним пробелом, причем наибольшее число должно быть первым.

# Начальный код

```haskell
module Kata (highAndLow) where

highAndLow :: String -> String
highAndLow input = error "Implement me!"
```

# Решение

## Моё:

```haskell
module Kata (highAndLow) where

highAndLow :: String -> String
highAndLow input = list'
  where
    list = map read $ words input :: [Int]
    list' = unwords $ map show [maximum list, minimum list]
```

## Лучшее:

```haskell
module Kata (highAndLow) where

highAndLow :: String -> String
highAndLow xs = show (maximum ns) ++ " " ++ show (minimum ns)
  where ns = (map read $ words xs) :: [Int]
```

или другое в бесточечном стиле

```haskell
module Kata (highAndLow) where

highAndLow :: String -> String
highAndLow = unwords . map show . sequence [maximum,minimum] . map (read ::String->Int) . words
```

[^отзыв]:**Отзыв**
	> Найти самое большое и самое маленькое значение из строки чисел, которую надо предварительно распарсить.
	> 
	> Отличная задача для начального уровня, позволяет натренировать парсинг инстансов Read и самую базовую работу со списками (на поиск наименьшего и наибольшего значений). Естественно, и то, и другое, будет полезно уже при решении реальных задач.

[^ссылка]: **Ссылка**
	- [Highest and lowest](https://www.codewars.com/kata/highest-and-lowest)