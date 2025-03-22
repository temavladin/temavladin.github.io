---
title: Дифференциалы высших порядков от функций с двумя переменными.
summary: Практика по математическому анализу. Решение двух примеров.
date: 2025-03-21
tags: ["Математический анализ"]
---

## Дифференциалы высших порядков от функций с двумя переменными.
Дифференциалы высших порядков определяются как:
{{< math >}}
$$ \mathrm{d}^n f(x,y) = \left( \dfrac{\partial}{\partial x} \mathrm{d} x + \dfrac{\partial}{\partial y} \mathrm{d} y \right)^n \cdot (f(x,y)) $$
{{< /math >}}
Иначе, разложив по формуле бинома Ньютона, получим:
{{< math >}}
$$ \mathrm{d}^n f(x,y) =  \displaystyle\sum_{k=0}^{n} C^k_n \dfrac{\partial^n f}{\partial x^{n-k} \cdot \partial y^k } \cdot \mathrm{d} x^{n-k} \cdot \mathrm{d} y^k  $$
{{< /math >}}

### Пример 1.

{{< math >}}
$f(x,y) = x \cdot \ln y \; \; \;$ Найти: $\mathrm{d}^3 f(x,y)$
{{< /math >}}