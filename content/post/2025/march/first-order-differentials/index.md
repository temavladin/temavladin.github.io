---
title: Решение дифференциальных уравнений первого порядка.
summary: Уравнения с разделяющимися переменными, однородные уравнения, линейные уравнения.
date: 2025-03-23
tags: ["Математический анализ"]
---
Текст данной страницы можно сохранить как PDF:
[Скачать PDF с серверов Вконтакте](https://vk.com/doc-228086099_685478384)
[Download PDF from web archive servers](https://archive.org/download/20250323_20250323_0600/Solution-of-first-order-differential-equations.pdf)

## Дифференциальные уравнения с разделяющимися переменными.
### Пример 1.

{{< math >}}
$xyy' = (y^2 - 1)$

\[ xy\dfrac{\mathrm{d} y}{\mathrm{d} x} = (y^2 - 1) \]
{{< /math >}}

Приведём к уравнению с разделёнными переменными и проинтегрируем.

{{< math >}}
\[ \int \dfrac{y \cdot \mathrm{d} y}{y^2 - 1} = \int \dfrac{\mathrm{d} x}{x} \]

\[ \dfrac{1}{2} \int \dfrac{\mathrm{d} (y^2 - 1)}{y^2 - 1} = \ln |x| + \ln |C| \]
\[ \dfrac{1}{2} \ln |y^2 - 1| = \ln |x| + \ln |C| \]
\[ \ln \sqrt{y^2 - 1} = \ln |x| + \ln |C| \]
{{< /math >}}

Уберём логарифмы и возведём в квадрат:
{{< math >}}
\[ y^2 - 1 = x^2 \cdot C' \]
{{< /math >}}
**Ответ:** {{< math >}} $ y^2 - 1 = x^2 \cdot C' $ {{< /math >}}

### Пример 2. (Лунгу № 2.1.21)
{{< math >}}
$y' - xy^2 = 0$

\[ \dfrac{\mathrm{d} y}{\mathrm{d} x} = xy^2 \]
{{< /math >}}

Приведём к уравнению с разделёнными переменными и проинтегрируем.

{{< math >}}
\[ \int \dfrac{\mathrm{d} y}{y^2} = \int x \mathrm{d} x \]

\[ - \dfrac{1}{y} = \dfrac{x^2}{2} + \dfrac{C}{2} \]

\[ y = - \dfrac{2}{x^2 + C} \]
{{< /math >}}

**Ответ:** {{< math >}} $ y = - \dfrac{2}{x^2 + C} $ {{< /math >}}

## Линейные дифференциальные уравнения первого порядка.

### Общий вид Л.Д.У.
{{< math >}}
\[ \dfrac{\mathrm{d} y}{\mathrm{d} x} + P(x) \cdot y = Q(x) \]
{{< /math >}}
### Схема решения Л.Д.У.

Здесь представлены только формулы для решения, подробный вывод читай по теме: линейные дифференциальные уравнения первого порядка. 

{{< math >}}
\[ y = u(x) \cdot v(x) \]

\[ v(x) = e^{- \int P(x) \mathrm{d} x} \]

\[ y = v(x) \cdot \left[ \int \dfrac{Q(x)}{v(x)} \mathrm{d} x + C \right]  \]

{{< /math >}}

### Пример 3.
{{< math >}}
\[ y - y' + \dfrac{3 e^x}{\sin^2 3x} = 0 \]

\[ y' - y = \dfrac{3 e^x}{\sin^2 3x} \]

Найдём $v(x)$, подставив в формулу (см. общий вид) известное $P(x)$.

\[ v(x) = e^{- \int -1 \mathrm{d} x} = e^x \]

\[ y = e^x \cdot \left[ \int \dfrac{3 e^x}{\sin^2 3x \cdot e^x} \mathrm{d} x + C \right]  \]

\[ y = e^x \cdot \left[ \int \dfrac{\mathrm{d} (3x)}{\sin^2 3x}  + C \right] \]

\[ y = e^x \cdot ( -\text{ctg} (3x)  + C ) \]
{{< /math >}}

**Ответ:** {{< math >}} $ y = e^x \cdot ( -\text{ctg} (3x)  + C ) $ {{< /math >}}

### Пример 4. (Лунгу № 2.3.2)
{{< math >}}
\[ y' - 2xy = e^{x^2} \]
{{< /math >}}

Решаем по той же схеме.

{{< math >}}
\[ v(x) = e^{- \int -2x \mathrm{d} x} = e^{x^2} \]

\[  y = e^{x^2} \cdot \left[ \int \dfrac{e^{x^2}}{e^{x^2}} \mathrm{d} x + C \right] \]

\[  y = e^{x^2} \cdot \left[ \int 1 \mathrm{d} x + C \right] \]

\[  y = e^{x^2} \cdot (x + C) \]
{{< /math >}}

**Ответ:** {{< math >}} $ y = e^{x^2} \cdot (x + C) $ {{< /math >}}

## Однородные дифференциальные уравнения первого порядка.

Однородное уравнение нулевого измерения можно привести к виду:

{{< math >}}
\[ \dfrac{\mathrm{d} y}{\mathrm{d} x} = f \left( 1, \dfrac{y}{x}\right) \]
{{< /math >}}

### Метод замены переменной.

Сделаем подстановку:

{{< math >}}
$u = \dfrac{y}{x}$, то есть $y = u \cdot x$, тогда $\dfrac{\mathrm{d} y}{\mathrm{d} x}=\dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} + u$
{{< /math >}}

Подставляя выражение производной в уравнение, получим:

{{< math >}}
\[ \dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} + u = f \left( 1, \dfrac{y}{x}\right) \]

\[ \dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} = f(1,u) - u \]
{{< /math >}}

Получили уравнение с разделяющимися переменными.

{{< math >}}
\[ \dfrac{\mathrm{d} u}{f(1,u) - u} = \dfrac{\mathrm{d} x}{x} \]

Проинтегрировав это выражение и подставив вместо $u$ отношение $y/x$, получим ответ.
{{< /math >}}

### Пример 5.
{{< math >}}
\[ y' = \dfrac{8xy - 28x^2 - 7y^2}{8x^2} \]

Разделим правую часть.

\[ y' = \dfrac{y}{x} - \dfrac{7}{2} - \dfrac{7}{8} \dfrac{y^2}{x^2}   \]

Сделаем подстановку $u = \dfrac{y}{x}$, $ \; \; \dfrac{\mathrm{d} y}{\mathrm{d} x}=\dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} + u$

\[ u + \dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} = u - \dfrac{7}{2} - \dfrac{7}{8} \cdot u^2   \]

\[ \dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} = - \dfrac{7}{2} - \dfrac{7}{8} \cdot u^2   \]

\[ \dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} = - \dfrac{7}{2} \cdot \left( 1 + \dfrac{u^2}{2^2} \right) \]

\[ \int \dfrac{\mathrm{d} u}{1 + \left( \frac{u}{2} \right)^2 } = - \dfrac{7}{2} \int \dfrac{\mathrm{d} x }{x} \]

\[ \int \dfrac{2 \cdot \mathrm{d} \left( \frac{u}{2} \right)}{1 + \left( \frac{u}{2} \right)^2 } = - 3,5 \cdot (\ln |x| + \ln |C|) \]

\[ 2 \, \text{arctg} \dfrac{u}{2} = - 3,5 \cdot \ln |Cx| \]

Подставим вместо $u$ отношение $y/x$.

\[ 2 \, \text{arctg} \left(  \dfrac{y}{2x} \right) = - 3,5 \cdot \ln |Cx| \]
{{< /math >}}

**Ответ:** {{< math >}} $ 2 \, \text{arctg} \left(  \dfrac{y}{2x} \right) = - 3,5 \cdot \ln |Cx| $ {{< /math >}}

### Пример 6. (Лунгу № 2.2.2)
{{< math >}}
\[ y \mathrm{d} x + (x + y) \mathrm{d} y = 0\]

Сделаем так, чтоб в левой части остался только $y'$.

\[ y + (x + y) \dfrac{\mathrm{d} y}{\mathrm{d} x} = 0  \]

\[ \dfrac{\mathrm{d} y}{\mathrm{d} x} = \dfrac{- y}{x + y}  \]

Сделаем подстановку $u = \dfrac{y}{x}$, $ \; \; \dfrac{\mathrm{d} y}{\mathrm{d} x}=\dfrac{\mathrm{d} u \cdot x}{\mathrm{d} x} + u$ 

\[ \dfrac{\mathrm{d} u}{\mathrm{d} x} \cdot x + u =  \dfrac{- u}{1 + u}\]

\[ \dfrac{\mathrm{d} u}{\mathrm{d} x} \cdot x = \dfrac{- 2 u - u^2}{1 + u}  \]

\[ \int \dfrac{(1 + u) \mathrm{d} u}{-2u -u^2} = \int \dfrac{\mathrm{d} x}{x} \]

Найдём интеграл слева, для этого сделаем замену. $t = -2u - u^2$, тогда $ \; \mathrm{d} t = (-2 -2u) \mathrm{d} u = - 2 (1 + u) \mathrm{d} u$

\[ \int \dfrac{(1 + u) \mathrm{d} u}{-2u -u^2} = \int \dfrac{- \dfrac{1}{2}\mathrm{d} t}{t}  \]

Подставим интеграл в уравнение.

\[ - \dfrac{1}{2} \int \dfrac{\mathrm{d} t}{t} = \int \dfrac{\mathrm{d} x}{x}   \]

\[ - \dfrac{1}{2} \ln |t| = \ln |x| + ln |C|   \]

Воспользуемся свойствами логарифмов.

\[ \dfrac{1}{\sqrt{t}} = Cx \]

\[ t = (Cx)^{-2}  \]

Перейдем от $t$, к $u$, а далее от $u$ к $y/x$.

\[ -2u - u^2 = C' \cdot x^{-2}   \]

\[ u^2 \cdot x^2 + 2 \cdot u \cdot x^2 = C'' \]

\[ y^2 + 2xy = C''  \]
{{< /math >}}

**Ответ:** {{< math >}} $ y^2 + 2xy = C $ {{< /math >}}