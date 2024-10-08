
$\binom{n}{k}$ - комбинации на n елемента k-ти клас
- колко подмножества с k елемента може да има множество с n елемента (подредбата няма значение)
 $$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$
Пермутация - брой подредби на n елемента - $n!$

Вариации - всички редици с k елементи, от множество с n елемента (подредбата има значение)
$$\frac{n!}{(n-k)!}$$
[Теорема: Биномна формула на Нютон](https://en.wikipedia.org/wiki/Binomial_theorem)  

 $$
 \forall x \in R, \forall n \in N
$$
$$
(1+x)^n = \sum \binom{n}{k}x^k
$$

Доказателство
1) Проверяваме за n=1

$$
(1+x)^1 \stackrel{?}{=} \sum_{0}^1\binom{1}{k}x^k
\Leftrightarrow
1+x \stackrel{?}{=}\binom{1}{0}x^0+\binom{1}{1}x^1
$$

 - дясната част се опростява 
 
 $$
 \frac{1!}{0!1!}x^0+\frac{1!}{1!1!}x^1 = 1 + x
$$

 2) Предполагаме, че е вярно за  някое n
 3) Доказваме, че ако е вярно за n, то тогава е вярно за n+1

 $$
 (1+x)^{n+1} = (1+x)(1+x)^n = (1+x)\sum_{k=0}^n\binom{n}{k}x^k =
 $$
 
$$
 =\sum_{k=0}^n\binom{n}{k}x^k + x\sum_{k=0}^n\binom{n}{k}x^k=
$$

$$
 =\sum_{k=0}^n\binom{n}{k}x^k + \sum_{k=0}^n\binom{n}{k}x^{k+1}=
$$

$$
 =\sum_{k=0}^n\binom{n}{k}x^k + \sum_{k=0}^n\binom{n}{k}x^{k+1}=
$$

- втората сума може да се трансформира

$$
=\sum_{k=0}^n \binom{n}{k}x^k + \sum_{k=1}^{n+1} \binom{n}{k-1}x^k=
$$

- изваждаме първия елемент от първата сума и втория елемент от последната сума, като трансформираме сумите

$$
 =\binom{n}{0}x^0 + \sum_{k=1}^{n} \binom{n}{k} x^k\ \ +\ \ \sum_{k=1}^{n} \binom{n}{k-1} x^k + \binom{n}{n} x^{n+1}
$$

- опростяваме и групираме сумите

$$
 = 1 + \sum_{k=1}^n \left(  \binom{n}{k} + \binom{n}{k-1}\right)x^k + x^{n+1}
$$

- чрез доказателство 1* (по-надолу във файла)

$$
 = 1 + \sum_{k=1}^n \binom{n+1}{k}x^k + x^{n+1}=
$$

$$
 = \binom{n+1}{0}+ \sum_{k=1}^n \binom{n+1}{k}x^k + x^{n+1}=
$$

$$
 = \binom{n+1}{0} + \sum_{k=1}^n \binom{n+1}{k}x^k + \binom{n+1}{n+1}x^{n+1}=
$$

$$
 = \sum_{k=0}^n \binom{n+1}{k}x^k + \binom{n+1}{n+1}x^{n+1}=
$$

$$
 = \sum_{k=0}^{n+1} \binom{n+1}{k}x^k
$$

- с това доказахме, че при увеличаване на n с 1 формулата се запазва, което означава, че ако твърдението е вярно за n, то то е вярно и за n+1
- от 1) доказахме, че е вярно за n=1, следователно от 3) трябва да е вярно за n=2, n=3 и тн.
## Доказателство 1*
- отделно смятаме $\binom{n}{k} + \binom{n}{k-1}$

$$
\binom{n}{k} + \binom{n}{k-1} = \frac{n!}{k!(n-k)!} + \frac{n!}{(k-1)!(n-k+1)!}=
$$


- умножаваме първата дроб по $(n-k+1) върху (n-k+1)$ и втората по k върху k, което ни позволява и да променим факториелите долу

$$
=\frac{n!(n-k+1)}{k!(n-k+1)!} + \frac{n!k}{k!(n-k+1)!}=
$$

- изваждаме пред скоби

$$
=\frac{n!}{k!(n-k+1)!}((n-k+1) + k)=\frac{n!(n+1)}{k!(n+1-k)!}=
$$

$$
=\binom{n+1}{k}
$$