|                 |                   |                     |
| --------------- | ----------------- | ------------------- |
| Название        | Disemvowel Trolls | Потрошители троллей |
| Отзыв[^отзыв]   |                   |                     |
| Ссылка[^ссылка] |                   |                     |

# Задача

> ## Оригинал
> 
> Trolls are attacking your comment section!
> 
> A common way to deal with this situation is to remove all of the vowels from the trolls' comments, neutralizing the threat.
> 
> Your task is to write a function that takes a string and return a new string with all vowels removed.
> 
> For example, the string "This website is for losers LOL!" would become "Ths wbst s fr lsrs LL!".
> 
> Note: for this kata `y` isn't considered a vowel.

> ## Перевод
> 
> Тролли атакуют ваш раздел комментариев!
> 
> Обычный способ справиться с этой ситуацией — удалить все гласные из комментариев троллей, нейтрализуя угрозу.
> 
> Ваша задача — написать функцию, которая принимает строку и возвращает новую строку, в которой удалены все гласные.
> 
> Например, строка «Этот сайт для неудачников, LOL!» станет «Ths wbst s fr lsrs LL!».
> 
> Примечание: для этой ката `y`не считается гласной.

# Начальный код

```haskell
module Disemvowel where

disemvowel :: String -> String
disemvowel str = undefined
```

# Решение

## Моё:

```haskell
module Disemvowel where

disemvowel :: String -> String
disemvowel str = filter isNotVowel str
  where
    isVowel c = elem c "aeiouAEIOU"
    isNotVowel = not . isVowel
```

## Лучшее:

```haskell
module Disemvowel where

disemvowel :: String -> String
disemvowel = filter (`notElem` "AEIOUaeiou")
```

[^отзыв]:**Отзыв**
	> Задача на удаление всех гласных (почти) из строки.
	> 
	> Позволяет закрепить отношение к строкам, как к списку символов, тренирует работу со списками, особенно базовые навыки фильтрации. Ката была выбрана в том числе из-за интересного оформления самой задачи и конкретного use case, где нужно защищаться от кричащих троллей :)

[^ссылка]: **Ссылка**
	- [Disemvowel trolls](https://www.codewars.com/kata/disemvowel-trolls)