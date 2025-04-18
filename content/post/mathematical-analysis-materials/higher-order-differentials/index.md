---
title: Дифференциалы высших порядков от функций с двумя переменными.
summary: Практика по математическому анализу. Решение двух примеров.
date: 2025-03-22
tags: ["Математический анализ"]
---

## Формула для вычисления дифференциалов высших порядков от функций с двумя переменными.
Дифференциалы высших порядков определяются как:
{{< math >}}
$$ \mathrm{d}^n f(x,y) = \left( \dfrac{\partial}{\partial x} \mathrm{d} x + \dfrac{\partial}{\partial y} \mathrm{d} y \right)^n \cdot (f(x,y)) $$
{{< /math >}}
Иначе, разложив по формуле бинома Ньютона, получим:
{{< math >}}
$$ \mathrm{d}^n f(x,y) =  \displaystyle\sum_{k=0}^{n} C^k_n \dfrac{\partial^n f}{\partial x^{n-k} \cdot \partial y^k } \cdot \mathrm{d} x^{n-k} \cdot \mathrm{d} y^k  $$
{{< /math >}}
## Пример 1.
{{< math >}}
$f(x,y) = x \cdot \ln y \; \; \;$ Найти: $\mathrm{d}^3 f(x,y)$
{{< /math >}}

Формула для вычисления дифференциала третьего порядка от функции двух переменных:
{{< math >}}
$$ \mathrm{d}^3 f(x,y) = C^0_3 \cdot \dfrac{\partial^3 f}{\partial x^3} \cdot \mathrm{d} x^3 + C^1_3 \cdot \dfrac{\partial^3 f}{\partial x^2 \partial y} \cdot \mathrm{d} x^2 \cdot \mathrm{d} y + $$
{{< /math >}}
{{< math >}}
$$ + C^2_3 \cdot \dfrac{\partial^3 f}{\partial x \partial y^2} \cdot \mathrm{d} x \cdot \mathrm{d} y^2 + C^3_3 \cdot \dfrac{\partial^3 f}{\partial y^3} \cdot \mathrm{d} y^3  $$
{{< /math >}}
Вычислим частные производные:
{{< math >}}
$$\dfrac{\partial f}{\partial x} = \ln y; \; \; \; \; \dfrac{\partial^2 f}{\partial x^2} = 0; \; \; \; \;  \dfrac{\partial^3 f}{\partial x^3} = 0;$$
$$ \dfrac{\partial f}{\partial y} = \dfrac{x}{y}; \; \; \; \; \dfrac{\partial^2 f}{\partial y^2} = - \dfrac{x}{y^2}; \; \; \; \;  \dfrac{\partial^3 f}{\partial y^3} = \dfrac{2x}{y^3}; $$
$$ \dfrac{\partial^3 f}{\partial x^2 \partial y} = 0; \; \; \; \; \dfrac{\partial^3 f}{\partial x \partial y^2} = -\dfrac{1}{y^2}$$
{{< /math >}}
Подставим значения в формулу:
{{< math >}}
\[ \mathrm{d}^3 f(x,y) = 1 \cdot 0 \cdot \mathrm{d} x^3 + 3 \cdot 0 \cdot \mathrm{d} x^2 \cdot \mathrm{d} y + \]
\[ + 3 \cdot \left( - \dfrac{1}{y^2}\right) \cdot \mathrm{d} x \cdot \mathrm{d} y^2 + 1 \cdot \dfrac{2x}{y^3} \cdot \mathrm{d} y^3 \]
{{< /math >}}
Вычислим оставшееся:
{{< math >}}
\[ \mathrm{d}^3 f(x,y) = 0 + 0 - \dfrac{3}{y^2} \cdot \mathrm{d} x \cdot \mathrm{d} y^2 + \dfrac{2x}{y^3} \cdot \mathrm{d} y^3 \]
\[ \mathrm{d}^3 f(x,y) = - \dfrac{3}{y^2} \cdot \mathrm{d} x \cdot \mathrm{d} y^2 + \dfrac{2x}{y^3} \cdot \mathrm{d} y^3 \]
{{< /math >}}

**Ответ:** {{< math >}} $ - \dfrac{3}{y^2} \cdot \mathrm{d} x \cdot \mathrm{d} y^2 + \dfrac{2x}{y^3} \cdot \mathrm{d} y^3$ {{< /math >}}

## Пример 2. (Лунгу № 11.5.7)
{{< math >}}
$z=f(x,y)= \sin x \cdot \sin y \; \;$ Найти: $\mathrm{d}^2 z$
{{< /math >}}

Формула для вычисления дифференциала второго порядка от функции двух переменных:
{{< math >}}
\[ \mathrm{d}^2 z = C^0_2 \cdot \dfrac{\partial^2 z}{\partial x^2} \cdot \mathrm{d} x^2 + C^1_2 \cdot \dfrac{\partial^2 z}{\partial x \partial y} \cdot \mathrm{d} x \cdot \mathrm{d} y + C^2_2 \cdot \dfrac{\partial^2 z}{\partial y^2} \cdot \mathrm{d} y^2 \]
{{< /math >}}
Вычислим частные производные:
{{< math >}}
\[ \dfrac{\partial z}{\partial x} = \cos x \cdot \sin y; \; \; \; \; \dfrac{\partial^2 z}{\partial x^2} = - \sin x \cdot \sin y; \]
\[ \dfrac{\partial z}{\partial y} = \sin x \cdot \cos y; \; \; \; \; \dfrac{\partial^2 z}{\partial y^2} = - \sin x \cdot \sin y; \]
\[ \dfrac{\partial^2 z}{\partial x \partial y} = \cos x \cdot \cos y; \]
{{< /math >}}
Подставим значения в формулу:
{{< math >}}
\[ \mathrm{d}^2 z = 1 \cdot (- \sin x \sin y) \cdot \mathrm{d} x^2 + 2 \cdot \cos x \cos y \cdot \mathrm{d} x \cdot \mathrm{d} y + 1 \cdot (- \sin x \sin y) \cdot \mathrm{d} y^2 \]
\[ \mathrm{d}^2 z = - \sin x \sin y \cdot \mathrm{d} x^2 + 2 \cos x \cos y \cdot \mathrm{d} x \cdot \mathrm{d} y - \sin x \sin y \cdot \mathrm{d} y^2 \]
{{< /math >}}
**Ответ:** {{< math >}} $ - \sin x \sin y \cdot \mathrm{d} x^2 + 2 \cos x \cos y \cdot \mathrm{d} x \cdot \mathrm{d} y - \sin x \sin y \cdot \mathrm{d} y^2 $ {{< /math >}}

## Сохранить эту страницу PDF

Текст данной страницы можно сохранить как PDF:
[Скачать PDF с серверов Вконтакте](https://vk.com/doc-228086099_685478382)
[Download PDF from web archive servers](https://archive.org/download/20250323_20250323_0600/Higher-order-differentials-from-functions-with-two-variables.pdf)