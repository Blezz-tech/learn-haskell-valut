|                 |                     |                               |
| --------------- | ------------------- | ----------------------------- |
| Название        | Tribonacci Sequence | Последовательность Трибоначчи | 
| Отзыв[^отзыв]   |                     |                               |
| Ссылка[^ссылка] |                     |                               |

# Задача

> ## Оригинал
> Well met with Fibonacci bigger brother, AKA Tribonacci.
> 
> As the name may already reveal, it works basically like a Fibonacci, but summing the last 3 (instead of 2) numbers of the sequence to generate the next. And, worse part of it, regrettably I won't get to hear non-native Italian speakers trying to pronounce it :(
> 
> So, if we are to start our Tribonacci sequence with `[1, 1, 1]` as a starting input (AKA _signature_), we have this sequence:
> 
> ```
> [1, 1 ,1, 3, 5, 9, 17, 31, ...]
> ```
> 
> But what if we started with `[0, 0, 1]` as a signature? As starting with `[0, 1]` instead of `[1, 1]` basically _shifts_ the common Fibonacci sequence by once place, you may be tempted to think that we would get the same sequence shifted by 2 places, but that is not the case and we would get:
> 
> ```
> [0, 0, 1, 1, 2, 4, 7, 13, 24, ...]
> ```
> 
> Well, you may have guessed it by now, but to be clear: you need to create a fibonacci function that given a **signature** array/list, returns **the first n elements - signature included** of the so seeded sequence.
> 
> Signature will always contain 3 numbers; n will always be a non-negative number; if `n == 0`, then return an empty array (except in C return NULL) and be ready for anything else which is not clearly specified ;)
> 
> If you enjoyed this kata more advanced and generalized version of it can be found in the [Xbonacci kata](http://www.codewars.com/kata/fibonacci-tribonacci-and-friends "Xbonacci sequence")
> 
> _[Personal thanks to Professor [Jim Fowler](https://www.coursera.org/instructor/jimfowler "Jim Fowler") on Coursera for his awesome classes that I really recommend to any math enthusiast and for showing me this mathematical curiosity too with his usual contagious passion :)]_
> 

> ## Перевод
> Хорошо познакомился со старшим братом Фибоначчи, также известным как Трибоначчи.
> 
> Как уже видно из названия, он работает в основном как Фибоначчи, но суммирует последние 3 (вместо 2) чисел последовательности для генерации следующего. И, что еще хуже, к сожалению, я не услышу, как его произносят не носители итальянского языка :(
> 
> Итак, если мы хотим начать нашу последовательность Трибоначчи в `[1, 1, 1]`качестве начального ввода ( _подпись_ AKA ), у нас есть эта последовательность:
> 
> ```
> [1, 1 ,1, 3, 5, 9, 17, 31, ...]
> ```
> 
> Но что, если мы начали с `[0, 0, 1]`подписи? Поскольку, начиная с `[0, 1]`вместо `[1, 1]`основного _сдвига_ обычной последовательности Фибоначчи на одну позицию, у вас может возникнуть соблазн подумать, что мы получим ту же самую последовательность, сдвинутую на 2 позиции, но это не так, и мы получим:
> 
> ```
> [0, 0, 1, 1, 2, 4, 7, 13, 24, ...]
> ```
> 
> Что ж, вы, возможно, уже догадались об этом, но для ясности: вам нужно создать функцию Фибоначчи, которая по заданному массиву **/** списку сигнатур возвращает **первые n элементов — сигнатуру, включенную** в последовательность, заполненную таким образом.
> 
> Подпись всегда будет содержать 3 цифры; n всегда будет неотрицательным числом; если `n == 0`, то верните пустой массив (за исключением C, возвращающего NULL) и будьте готовы ко всему, что не указано явно;)
> 
> Если вам понравилось это ката, более продвинутую и обобщенную версию можно найти в [ката Xbonacci.](http://www.codewars.com/kata/fibonacci-tribonacci-and-friends "Последовательность Xbonacci")
> 
> _[Личное спасибо профессору [Джиму Фаулеру](https://www.coursera.org/instructor/jimfowler "Джим Фаулер") на Coursera за его замечательные уроки, которые я действительно рекомендую всем любителям математики, и за то, что он также проявил ко мне эту математическую любознательность со своей обычной заразительной страстью :)]_
> 

# Начальный код

```haskell
module Tribonacci where

tribonacci :: Num a => (a, a, a) -> Int -> [a]
tribonacci (a, b, c) n = undefined
```

# Решение

## Моё:

```haskell

```

## Лучшее:

```haskell

```


[^отзыв]:**Отзыв**
	> Интересная вариация набившей оскомину задачи про ряд Фибоначчи. Очень простое с виду изменение правил игры заставляет призадуматься. Ката отлично тренирует конструирование списков и рекурсию, либо умение обходиться без рекурсии стандартными функциями высшего порядка :)

[^ссылка]: **Ссылка**
	- [Tribonacci sequence](https://www.codewars.com/kata/tribonacci-sequence)