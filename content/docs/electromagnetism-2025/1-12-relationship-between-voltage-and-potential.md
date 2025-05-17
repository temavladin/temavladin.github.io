---
linkTitle: 1.12 Связь между напряжённостью и потенциалом
title: 1.12 Связь между напряжённостью и потенциалом
date: 2025-05-17
type: docs
authors: ["admin"]
profile: true
tags: ["Физика", "Электричество"]
weight: 13
---

Сравнивая определение работы и потенциала, получим:

{{< math >}} \[ \int\limits_1^{\infty} \vec{F} \vec{ \mathrm{d} l } = A_{\infty} = q_0 \phi = W  \] \[ \int\limits_1^{\infty} \vec{F} \vec{ \mathrm{d} l } = q_0 \int\limits_1^{\infty} \vec{E} \vec{ \mathrm{d} l } = q_0 \phi \] \[ \phi = \int\limits_1^{\infty} \vec{E} \vec{ \mathrm{d} l } \]

Продифференцируем выражение. При дифференцировании интеграла с переменным нижним пределом получим подынтегральную функцию со знаком минус: \[ \mathrm{d} \phi = - ( \vec{E} \cdot \vec{ \mathrm{d} l} ) \]

Запишем скалярное произведение через произведения соответствующих компонент векторов \[ \mathrm{d} \phi = - ( \vec{E} \cdot \vec{ \mathrm{d} l} ) = - ( E_x \mathrm{d} x + E_y \mathrm{d} y + E_z \mathrm{d} z ) \]

Теперь учтем, что потенциал – функция, зависящая от трех координат \[ \phi = \phi (x,y,z) \]

По формуле полного дифференциала от функции трёх переменных получим: \[ \mathrm{d} \phi = \dfrac{\partial \phi}{\partial x} \mathrm{d} x + \dfrac{\partial \phi}{\partial y} \mathrm{d} y + \dfrac{\partial \phi}{\partial z} \mathrm{d} z \]

Приравняем правые части: \[ - ( E_x \mathrm{d} x + E_y \mathrm{d} y + E_z \mathrm{d} z ) = \dfrac{\partial \phi}{\partial x} \mathrm{d} x + \dfrac{\partial \phi}{\partial y} \mathrm{d} y + \dfrac{\partial \phi}{\partial z} \mathrm{d} z \] Из этого следуют равенства: \[ E_x = - \dfrac{\partial \phi}{\partial x}; \; \; E_y = - \dfrac{\partial \phi}{\partial y}; \; \; E_z = - \dfrac{\partial \phi}{\partial z}; \]

Для вектора напряженности в целом получаем выражение \[ \vec{E} = -\vec{i} \dfrac{\partial \phi}{\partial x} -\vec{j} \dfrac{\partial \phi}{\partial y} -\vec{k} \dfrac{\partial \phi}{\partial z} = \] \[ = - \left( \vec{i} \dfrac{\partial}{\partial x} +\vec{j} \dfrac{\partial}{\partial y} +\vec{k} \dfrac{\partial}{\partial z}  \right) \phi = - \text{grad} \phi \]

Связь между напряжённостью и потенциалом имеет вид \[ \vec{E} = - \text{grad} \phi = - \nabla \phi\] где $\text{grad}$ — градиент, а $\nabla$ — векторный оператор набла. {{< /math >}}

Знак минус в данном выражении показывает, что вектор напряжённости {{< math >}} $\vec{E}$ {{< /math >}}  электрического поля направлен в сторону убывания потенциала.