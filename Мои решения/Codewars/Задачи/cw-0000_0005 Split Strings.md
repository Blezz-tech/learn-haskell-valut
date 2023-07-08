|                 |               |                  |
| --------------- | ------------- | ---------------- |
| Название        | Split Strings | Разделить строки | 
| Отзыв[^отзыв]   |               |                  |
| Ссылка[^ссылка] |               |                  |

# Задача

> ## Оригинал
> Complete the solution so that it splits the string into pairs of two characters. If the string contains an odd number of characters then it should replace the missing second character of the final pair with an underscore ('_').
> 
> Examples:
> 
> ```
> * 'abc' =>  ['ab', 'c_']
> * 'abcdef' => ['ab', 'cd', 'ef']
> ```

> ## Перевод
> Завершите решение так, чтобы оно разбило строку на пары из двух символов. Если строка содержит нечетное количество символов, то отсутствующий второй символ последней пары должен быть заменен символом подчеркивания ('_').
> 
> Примеры:
> 
> ```
> * 'abc' =>  ['ab', 'c_']
> * 'abcdef' => ['ab', 'cd', 'ef']
> ```

# Начальный код

```haskell
module Codewars.Kata.SplitStrings where

solution :: String -> [String]
solution = undefined
```

# Решение

## Моё:

```haskell
module Codewars.Kata.SplitStrings where

solution :: String -> [String]
solution [] = []
solution [x] = [x : "_"]
solution (x:y:xs) = [x,y] : solution xs
```

## Лучшее:

```haskell

```


[^отзыв]:**Отзыв**
	> Задача с предельно простым описанием, очень ясным примером, но которая не такая очевидная в решении. Хорошо иллюстрирует работы с паттерн-матчингом и конструированием списков, которые тут приходится то разбирать, то собирать. Ну и, естественно, отличная тренировка самой базовой рекурсии.

[^ссылка]: **Ссылка**
	- [Split strings](https://www.codewars.com/kata/split-strings)