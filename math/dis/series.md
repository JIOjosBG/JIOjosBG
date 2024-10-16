Безкрайни редици 
- дефиниция ....
- означават се с 
	- $a_1, a_2, a_3....a_n$
	- $\{a_n\}_{n=1}^\infty$
	- $\{a_n\}$
Казваме, че една редица е сходяща, ако 
$\forall \epsilon >0, \epsilon \in R, \exists n \in N, k\ge n, така, че |a_k -a|<\epsilon$
Същестува елемент ($a_k$), за който е вярно, че всеки следващ елемент е по-близо до точката на сгъстяване

Ако една редица не е сходяща, то тя се нарича разходяща

Казваме, че една редица е разходяща към $+\infty$ ако $\forall C\in R, \exists n \in N: \forall k\ge n$ е вярно $a_k\ge C$
Т.е. за всяко число C от R можем да намерим пореден елемент $a_n$, след който всеки елемент $a_k$ е по-голям от C

Една редица е ограничена ако $\exists C>0, |a_n|<C, \forall n \in N$
Т.е. съществува C, което е по-голямо от всички елементи $a_n$

Доказателство, че $\{(-1)^n\}$ е разходяща редица:
1. Допускаме, че е е сходяща (ще направим доказателство за обратното чрез противоречие)
2. От дефицинията за сходимост избираме $\epsilon=1$, което ще означава, че $\exists n\in N, \forall k\ge n => |(-1)^n-a|<1 <=> (-1)^k \in (a-1;a+1)$ т.е. за приетите параметри общия елемент на функцията е в интервала $(a-1;a+1)$
	1. При четно k => $1 \in (a-1;a+1)$, което е възможно само $0<a<2$
	2. При нечетно k => $-1 \in (a-1;a+1)$, което е възможно само за $-2<a<0$
	3. Двете условия за не могат да бъдат верни едновременно за една и съща редица, защото няма препокриване на двата интервала => това няма как да стане
3. От 2 доказахме, че има противоречие. Единственото предположение, което направихме, е, че редицата е разходяща. Редицата е сходяща

Ако към една сходяща редица добавим или извадим краен брой числа, то получаваме редица, сходяща към същата граница - просто дефиницията за сходяща редица ни позволява да правим такива неща, защото винаги ще има някое $n\le k, |a_k -a| <\epsilon$
