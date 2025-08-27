# Marcha-Aleatoria-en-1D
 Marcha Aleatoria 1D – Física Estadística
 Cómo correr el programa


1. Copia el código en un archivo `marcha_aleatoria.py` o en una celda de **Google Colab**.  
2. Ejecuta el programa.  
3. Aparecerá un menú:

```
Seleccione una opción:
1. Índice 7 (Marcha aleatoria y comparación con Gaussiana)
2. Índice 8 (Cálculo de <x>, <x^2> y constante de difusión)
```

---
 Opciones del programa

 Opción 1 – Índice 7
- Simula una marcha aleatoria de `N` pasos, repetida `n_sim` veces.  
- Grafica:
  - Un **histograma de posiciones finales** (color morado).  
  - La **distribución gaussiana teórica** predicha por el Teorema Central del Límite (color naranja).  
- Imprime:
  - Media simulada  
  - Varianza simulada (comparada con el valor esperado `N`).

Ejemplo de entrada:
```
Ingrese el número de pasos N: 1000
Ingrese el número de simulaciones: 5000
```

---

 Opción 2 – Índice 8
- Permite ingresar:
  - `N_max` → número máximo de pasos.  
  - `n_sim` → número de simulaciones para cada valor de N.  
- Calcula para cada `N`:
  - <x>  
  - <x^2>  
- Grafica:
  - <x^2> contra N (color morado).  
  - Una línea guía proporcional a N (color naranja).  
- Ajusta linealmente los datos para estimar la **constante de difusión D** con:

<x^2> ≈ 2DN

Ejemplo de entrada:
```
Ingrese el valor máximo de N: 1000
Ingrese el número de simulaciones por N: 5000
```

---
 Resultados esperados

- **Opción 1:**  
  El histograma de posiciones debe aproximarse a la gaussiana teórica, confirmando el **Teorema Central del Límite**.  

- **Opción 2:**  
  La gráfica de <x^2> contra N debe ser aproximadamente lineal.  
  El ajuste numérico debe dar una constante de difusión cercana a:

D ≈ 0.5

---


- Los resultados numéricos (media, varianza, difusión) pueden variar ligeramente en cada ejecución debido al carácter aleatorio del proceso.  
- Si se aumenta el número de simulaciones (`n_sim`), las fluctuaciones estadísticas se reducen y los resultados se acercan más a la teoría.  

---

