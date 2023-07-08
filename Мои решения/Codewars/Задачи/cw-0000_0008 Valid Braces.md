|                 |              |                            |
| --------------- | ------------ | -------------------------- |
| Название        | Valid Braces | Допустимые фигурные скобки | 
| Отзыв[^отзыв]   |              |                            |
| Ссылка[^ссылка] |              |                            |

# Задача

> ## Оригинал
> Write a function that takes a string of braces, and determines if the order of the braces is valid. It should return `true` if the string is valid, and `false` if it's invalid.
> 
> This Kata is similar to the [Valid Parentheses](https://www.codewars.com/kata/valid-parentheses-1) Kata, but introduces new characters: brackets `[]`, and curly braces `{}`. Thanks to `@arnedag` for the idea!
> 
> All input strings will be nonempty, and will only consist of parentheses, brackets and curly braces: `()[]{}`.
> 
> ### What is considered Valid?
> 
> A string of braces is considered valid if all braces are matched with the correct brace.
> 
> ### Examples
> 
> ```
> "(){}[]"   =>  True
> "([{}])"   =>  True
> "(}"       =>  False
> "[(])"     =>  False
> "[({})](]" =>  False
> ```
> 

> ## Перевод
> Напишите функцию, которая принимает строку фигурных скобок и определяет, допустим ли порядок фигурных скобок. Он должен возвращаться `true`, если строка действительна и `false`недействительна.
> 
> Этот Kata похож на Kata [Valid Parentheses](https://www.codewars.com/kata/valid-parentheses-1) , но вводит новые символы: скобки `[]`и фигурные скобки `{}`. Спасибо `@arnedag`за идею!
> 
> Все входные строки будут непустыми и будут состоять только из круглых, квадратных и фигурных скобок: `()[]{}`.
> 
> ### Что считается действительным?
> 
> Строка фигурных скобок считается допустимой, если все фигурные скобки соответствуют правильной фигурной скобке.
> 
> ### Примеры
> 
> ```
> "(){}[]"   =>  True
> "([{}])"   =>  True
> "(}"       =>  False
> "[(])"     =>  False
> "[({})](]" =>  False
> ```

# Начальный код

```haskell
module Codewars.Kata.Braces where

validBraces :: String -> Bool
validBraces xs = error "todo: validBraces"
```

# Решение

## Моё:

```haskell

```

## Лучшее:

```haskell

```


[^отзыв]:**Отзыв**
	> Нужно проверить все ли скобки в выражении закрываются. Можно решать разными способами.
	> 
	> Она заставляет задуматься, что является аналогом стека в хаскеле, и тренирует навыки обращения со свертками.

[^ссылка]: **Ссылка**
	- [Valid braces](https://www.codewars.com/kata/5277c8a221e209d3f6000b56)