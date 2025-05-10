No es posible describir las distribuciones de probabilidad compleatas como un vector para las [[Variable Aleatoria#^5075d2|variables aleatorias continuas]], ya que hay infinitos valores (y, de hecho, solo se le puede asignar una probabilidad de 0 a cada valor individual que la variable aleatoria puede tomar).
La probabilidad que una VAC pueda tomar valores en $x$ suele ser definida mediante una función parametrizada de $x$, usualmente llamada una función de densidad de probabilidad
***
Por ejemplo, la distribución normal (o Gaussiana) está definida por
$$pdf(x)=\frac{1}{\sigma\sqrt{2\pi}}e^{-\frac{1}{2}(\frac{x-\mu}{\sigma})²}$$
Lo usual es calcular probabilidades para un rango de valores, usando expresiones como $$P(a<X<b)=\int_a^bpdf(x)dx$$
