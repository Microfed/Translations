Кажется ни один из курсов программирования не обходится без упражнений на Евклидов алгоритм вычисления Наибольшего Общего
Делителя (НОД или GCD).

НОД двух чисел `A` и `B` называют такое третье число `C` что оба первых делятся на него без остатка, при этом
`C` должно быть наибольшим из возможных. Например `gcd(20, 35) = 5` а `gcd(13, 28) = 1`. Алгоритм Евклида заключается в том что
из большего числа вычитают меньшее, повторяя эту операцию пока числа не сравняются - это и будет НОД. Для ускорения можно не
вычитать, а брать остаток от деления.

Если кажется что это очень абстрактные математические "фокусы", то стоит обратить внимание что делимость чисел вообще и НОД
в частности положены в основу современной криптографии (в чем вы убедитесь из дальнейших задач).

Наименьшее общее кратное (НОК или LCM) - это наименьшее из чисел `D` которые делятся и на `A` и на `B`. Его можно найти
так:

    lcm(A, B) = A * B / gcd(A, B)

### Задача

**Входные данные** указывают количество тестов в первой строке.  
Дальше идут тестовые строки, каждая содержит по два числа - `A` и `B`.  
**Ответ** должен содержать НОД и НОК каждой пары, заключенные в скобки и разделенные пробелами.

Пример:

    входные данные:
    2
    2 3
    4 10
    
    ответ:
    (1 6) (2 20)