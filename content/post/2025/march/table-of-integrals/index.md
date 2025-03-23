---
title: Таблица основных интегралов.
summary: Таблица основных (простейших) интегралов. Неопределённый интеграл. Первообразная функции.
date: 2025-03-21
tags: ["Математический анализ"]
---

{{< math >}}

### 1. Интеграл от нуля.

\[ \int 0 \cdot \mathrm{d}x = C \]

Интеграл от нуля равен произвольной постоянной $C$ (константа).

### 2. Интеграл от константы.

Например интеграл от единицы:

\[ \int 1 \cdot \mathrm{d}x = x + C \]

### 3. Интеграл от степенной функции.

\[ \int x^{\mu} \; \mathrm{d}x = \frac{x^{\mu + 1}}{\mu + 1} + C, \; \; (\mu \neq -1) \]

### 4. Интеграл от степени -1.

\[ \int \frac{1}{x} \; \mathrm{d}x = \ln{|x|} + C \]

### 5. Интеграл от показательной функции.

\[ \int a^x \; \mathrm{d}x = \frac{a^x}{\ln{a}}  + C\]

### 6. Интеграл от экспоненты.

\[ \int e^x \; \mathrm{d}x = e^x  + C \]

### 7. Интеграл от функции синус.

\[ \int \sin{x} \; \mathrm{d}x = -\cos{x}  + C \]

### 8. Интеграл от функции косинус.

\[ \int \cos{x} \; \mathrm{d}x = \sin{x}  + C \]

### 9. Интегралы равные тригонометрическим функциям.

Котангенс, тангенс, арксинус, арккотангенс.

\[ \int \frac{1}{\sin^2{x}} \; \mathrm{d}x = - \text{ctg } x  + C \]

\[ \int \frac{1}{\cos^2{x}} \; \mathrm{d}x = \text{tg } x  + C \]

\[ \int \frac{1}{\sqrt{1 - x^2}} \; \mathrm{d}x = \text{arcsin } x  + C \]

\[ \int \frac{1}{\sqrt{a^2 - x^2}} \; \mathrm{d}x = \text{arcsin} \, \frac{x}{a}  + C \]

\[ \int \frac{1}{1+x^2} \; \mathrm{d}x = \text{arctg } x  + C \]

\[ \int \frac{1}{a^2+x^2} \; \mathrm{d}x = \frac{1}{a} \; \text{arctg} \, \frac{x}{a}  + C \]

### 10. Интеграл <<Длинный логарифм>>.

\[ \int \frac{1}{\sqrt{x^2 \pm a^2}} \; \mathrm{d}x = \ln{\left|x + \sqrt{x^2 \pm a^2}\right|} + C \]

### 11. Интеграл <<Высокий логарифм>>.

\[ \int \frac{1}{x^2 - a^2} \; \mathrm{d}x = \frac{1}{2a} \; \ln{\left|\frac{x-a}{x+a}\right|} + C \]
{{< /math >}}