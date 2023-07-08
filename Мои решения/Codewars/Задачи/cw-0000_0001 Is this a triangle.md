|                 |                    |                  |
| --------------- | ------------------ | ---------------- |
| Название        | Is this a triangle | Это треугольник? |
| Отзыв[^отзыв]   |                    |                  |
| Ссылка[^ссылка] |                    |                  |

# Задача

> ## Оригинал
> 
> Implement a function that accepts 3  integer values a, b, c. The function should return true if a triangle can be built with the sides of given length and false in any other case.
> 
> (In this case, all triangles must have surface greater than 0 to be accepted).

> ## Перевод
> 
> Реализуйте функцию, которая принимает 3 целых значения a, b, c. Функция должна возвращать значение true, если можно построить треугольник со сторонами заданной длины, и значение false в любом другом случае.
> 
> (В этом случае все треугольники должны иметь поверхность больше 0, чтобы быть принятыми).

# Начальный код

## Моё:

```haskell
module Codewars.Triangles where

import Data.List (sort)

isTriangle :: Int -> Int -> Int -> Bool
isTriangle a b c = error "todo: isTriangle"
```

## Лучшее:

```
```

# Решение

```haskell
module Codewars.Triangles where

import Data.List (sort)

isTriangle :: Int -> Int -> Int -> Bool
isTriangle a b c = (a1 + b1) > c1
                   where
                     [a1, b1, c1] = sort [a, b, c]
```

[^отзыв]:**Отзыв**
	> Определение, могут ли данных три числа быть длинами сторон треугольника.
	> 
	> С этой катой тренируются базовые логические конструкции. Полезно, что есть простор и для элегантных решений, и для решений "в лоб".
	> 
	> Есть вероятность, что практикующий потренирует так же совсем базовую работу со списками (хотя тут это необязательно).

[^ссылка]: **Ссылка**
	- [Is this a triangle](https://www.codewars.com/kata/is-this-a-triangle)