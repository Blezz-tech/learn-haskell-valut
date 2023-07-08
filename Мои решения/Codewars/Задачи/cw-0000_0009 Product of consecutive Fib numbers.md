|                 |                                    |                                               |
| --------------- | ---------------------------------- | --------------------------------------------- |
| Название        | Product of consecutive Fib numbers | Произведение последовательных чисел Фибоначчи | 
| Отзыв[^отзыв]   |                                    |                                               |
| Ссылка[^ссылка] |                                    |                                               |

# Задача

> ## Оригинал
> The Fibonacci numbers are the numbers in the following integer sequence (Fn):
> 
> 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, ...
> 
> such as
> 
> F(n) = F(n-1) + F(n-2) with F(0) = 0 and F(1) = 1.
> 
> Given a number, say prod (for product), we search two Fibonacci numbers F(n) and F(n+1) verifying
> 
> F(n) * F(n+1) = prod.
> 
> Your function productFib takes an integer (prod) and returns an array:
> 
> ```haskell
> [F(n), F(n+1), true] or {F(n), F(n+1), 1} or (F(n), F(n+1), True)
> ```
> 
> depending on the language if F(n) * F(n+1) = prod.
> 
> If you don't find two consecutive F(n) verifying `F(n) * F(n+1) = prod`you will return
> 
> ```haskell
> [F(n), F(n+1), false] or {F(n), F(n+1), 0} or (F(n), F(n+1), False)
> ```
> 
> F(n) being the smallest one such as `F(n) * F(n+1) > prod`.
> 
> #### Some Examples of Return:
> 
> (depend on the language)
> 
> ```haskell
> productFib(714) # should return (21, 34, true), 
>                 # since F(8) = 21, F(9) = 34 and 714 = 21 * 34
> 
> productFib(800) # should return (34, 55, false), 
>                 # since F(8) = 21, F(9) = 34, F(10) = 55 and 21 * 34 < 800 < 34 * 55
> -----
> productFib(714) # should return [21, 34, true], 
> productFib(800) # should return [34, 55, false], 
> -----
> productFib(714) # should return {21, 34, 1}, 
> productFib(800) # should return {34, 55, 0},        
> -----
> productFib(714) # should return {21, 34, true}, 
> productFib(800) # should return {34, 55, false}, 
> ```
> 
> #### Note:
> 
> - You can see examples for your language in "Sample Tests".

> ## Перевод
> Числа Фибоначчи — это числа в следующей целочисленной последовательности (Fn):
> 
> 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, 233, ...
> 
> такой как
> 
> F(n) = F(n-1) + F(n-2), где F(0) = 0 и F(1) = 1.
> 
> Имея число, скажем, prod (для произведения), мы ищем два числа Фибоначчи F(n) и F(n+1), проверяя
> 
> F(n) * F(n+1) = произв.
> 
> Ваша функция productFib принимает целое число (prod) и возвращает массив:
> 
> ```haskell
> [F(n), F(n+1), true] or {F(n), F(n+1), 1} or (F(n), F(n+1), True)
> ```
> 
> в зависимости от языка, если F(n) * F(n+1) = prod.
> 
> Если вы не найдете два последовательных подтверждения F (n), `F(n) * F(n+1) = prod`вы вернетесь
> 
> ```haskell
> [F(n), F(n+1), false] or {F(n), F(n+1), 0} or (F(n), F(n+1), False)
> ```
> 
> F(n) является наименьшим из таких, как `F(n) * F(n+1) > prod`.
> 
> #### Некоторые примеры возврата:
> 
> (зависит от языка)
> 
> ```haskell
> productFib(714) # should return (21, 34, true), 
>                 # since F(8) = 21, F(9) = 34 and 714 = 21 * 34
> 
> productFib(800) # should return (34, 55, false), 
>                 # since F(8) = 21, F(9) = 34, F(10) = 55 and 21 * 34 < 800 < 34 * 55
> -----
> productFib(714) # should return [21, 34, true], 
> productFib(800) # should return [34, 55, false], 
> -----
> productFib(714) # should return {21, 34, 1}, 
> productFib(800) # should return {34, 55, 0},        
> -----
> productFib(714) # should return {21, 34, true}, 
> productFib(800) # should return {34, 55, false}, 
> ```
> 
> #### Примечание:
> 
> - Вы можете увидеть примеры для вашего языка в разделе "Образцы тестов".

# Начальный код

```

```

# Решение

## Моё:

```

```

## Лучшее:

```

```


[^отзыв]:**Отзыв**
	> Нужно найти является ли переданное число произведением соседних чисел в последовательности Фибоначчи.
	> 
	> Задача тренирует навыки создания рекурсии, или обращения с функциями из Data.List.

[^ссылка]: **Ссылка**
	- [Product of consecutive Fib numbers](https://www.codewars.com/kata/5541f58a944b85ce6d00006a)