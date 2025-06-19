# 📡 Simulador de Patrones de Radiación (Antenas / Fuentes Acústicas)

Este programa permite simular y visualizar **patrones de radiación** en coordenadas polares para distintos tipos de fuentes acústicas (o antenas ideales), como **monopolos, dipolos, tripolos y cuadripolos**.

---

## 🎯 ¿Qué hace este programa?

Permite al usuario:

1. Ingresar parámetros físicos como:

   * Frecuencia
   * Velocidad de propagación
   * Separación de fuentes
   * Amplitud
   * Distancia al punto de observación
2. Elegir un tipo de fuente o arreglo (antena):

   * Monopolo
   * Dipolo
   * Tripolo positivo
   * Tripolo negativo
   * Cuadripolo
3. Visualizar en una **gráfica polar** la distribución de amplitud (patrón de radiación)

---

## 📈 ¿Qué representa cada gráfica?

| Tipo de fuente       | Descripción física                                 |
| -------------------- | -------------------------------------------------- |
| **Monopolo**         | Fuente puntual, irradia igual en todas direcciones |
| **Dipolo**           | Dos fuentes separadas que interfieren              |
| **Tripolo positivo** | Tres fuentes con fase específica constructiva      |
| **Tripolo negativo** | Tres fuentes con fase específica destructiva       |
| **Cuadripolo**       | Patrón más complejo con fuentes múltiples          |

---

## ⚙️ Cálculos clave

* `omega = 2πf`: frecuencia angular
* `k = omega / c`: número de onda
* Se usa `np.sin(k * d * sin(θ))` para modelar cómo varía la interferencia en diferentes direcciones (ángulo `θ`)

---
## 🚀 Características

- Interfaz gráfica fácil de usar (hecha con `tkinter`)
- Ingreso de parámetros físicos:
  - Frecuencia (Hz)
  - Velocidad de propagación (m/s)
  - Separación entre fuentes (m)
  - Amplitud
  - Distancia al receptor
- Tipos de fuentes:
  - Monopolo
  - Dipolo
  - Tripolo positivo / negativo
  - Cuadripolo
- Visualización en **gráfica polar** con `matplotlib`

## 📦 Requisitos

- Python 3.x
- Librerías necesarias:

```bash
pip install numpy matplotlib
````

## ▶️ Cómo usar

1. Ejecuta el script:

   ```bash
   python simulador_antenas.py
   ```

2. Ingresa los parámetros deseados.

3. Selecciona el tipo de gráfica.

4. Haz clic en **"Graficar"** para ver el patrón de radiación.

## 📚 Aplicaciones

* Acústica
* Teoría de antenas
* Interferencia y propagación
* Ingeniería de sonido y telecomunicaciones

## 👤 Autor

**Dilan Acosta**

