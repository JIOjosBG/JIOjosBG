z = a+ i\*b

i - имагинерна единица
Re z = a
Im z = b

Модул на комплексно число
$|z| = \sqrt{a^2+b^2}$

1. Алгебричен вид
	1. събиране и изваждане
		-  $z_1 = a_1+ib_1$
		- $z_2=a_2+ib_2$
		- $z_1+z_2 = (a_1+a_2)+i(b_1+b_2)$
		- $z_1-z_2 = (a_1-a_2)+i(b_1-b_2)$
	2. Умножение и деление
		- $z_1=a+ib$
		- $z_2=c+id$
		- $z_1*z_2=(ac-db)+i(bc+ad)$ (просто разкриване на скоби)
		- $$z_1/z_2 = \frac{a+bi}{c+di} = \frac{(a+bi)(c-di)}{(c-di)^2}=\frac{(ac+bd)-i(ad-bc)}{c^2+d^2}$$
	3. Степенуване
		- $i^n = ?$
		- $i^1 = i;\ i^2 = -1;\ i^3 = -1;\ i^4=1;$
		- Можем да си ползваме формулите и триъгълника на Паскал за степенуване
		- $(a+ib)^3 = a^3 + 3a^2bi -3ab^2 - ib^3$
	4. Квадратни уравнения
		- $$D>0 =>x_{12} = \frac{-b\pm \sqrt{D}}{2a}$$
		-  $$D < 0 => x_{12}=\frac{-b\pm i \sqrt{|D|}}{2a}$$
2. Геометричен вид
	- Показване на комплексното число като вектор
	- за $z=a+ib$, а е x координатата, а b е y координатата
	- в геометрично представяне става ясно, че $|z|=\sqrt{a^2+b^2}$ всъщност е дължината на вектора
	- От този тип представяне можем да видим и тригонометричното

3. Тригонометричен вид
	- за $z=a+ib$
	- $r=|z|=\sqrt{a^2+b^2}$
	- $\cos\alpha = a/r => a= \cos\alpha *r$
	- $\sin\alpha = b/r => b= \sin\alpha *r$
	- $z = a+bi = r*\cos\alpha + r*i*\sin\alpha=r(\cos\alpha +i*\sin\alpha)$
	- $\sin$ и $\cos$ са периодична на $2k\pi$ => 
	- $\sin\alpha = \sin{\alpha+2k\pi}$
	- $\cos\alpha = \cos{\alpha+2k\pi}$
	- $\cos\alpha = \cos{-\alpha}$
	- $\sin{-\alpha} =-\sin\alpha$
	1. Умножение
		- $z_1=r_1(\cos\alpha+i\sin\alpha)$
		- $z_2=r_2(\cos\beta+i\sin\beta)$
		- $z_1 z_2 =r_1 r_2(\cos(\alpha+\beta)+i\sin(\alpha+\beta))$
	2. Степенуване
		- $z^n=r^n(\cos(n\alpha)+i\sin(n\alpha))$
	3. Делене
		- $z_1/z_2 = r_1/r_2(\cos(\alpha-\beta)+i\sin(\alpha-\beta))$
	4. Коренуване
		- $$\sqrt[n]{z} = \sqrt[n]{r}(\cos(\frac{\alpha +2k\pi}{n})+\sin(\frac{\alpha+2k\pi}{n}))$$
		- горната формула се смятат n на брой корена, като k може да бъде между 0 и n-1  включително