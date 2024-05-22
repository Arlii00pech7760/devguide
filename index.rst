import numpy as np
import matplotlib.pyplot as plt

# Definir la función
def f(x):
    return (x - 1) / (x**2 + 2*x + 1)

# Generar valores x
x_values = np.linspace(0.5, 1.5, 400)

# Calcular los valores y
y_values = f(x_values)

# Graficar la función
plt.plot(x_values, y_values, label='$\\frac{x - 1}{x^2 + 2x + 1}$')

# Línea horizontal para el límite
plt.axhline(y=1/3, color='r', linestyle='--', label='Límite')

# Etiquetas y leyenda
plt.xlabel('x')
plt.ylabel('f(x)')
plt.title('Gráfico de $\\frac{x - 1}{x^2 + 2x + 1}$')
plt.legend()

# Mostrar la gráfica
plt.grid(True)
plt.show()
