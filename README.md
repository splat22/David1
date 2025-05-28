# Predicción de Monto de Préstamos Digitales en Perú

Este proyecto implementa modelos de regresión lineal simple y redes neuronales para predecir el **monto de préstamos digitales** otorgados a clientes peruanos. Se desarrolla con Python, TensorFlow/Keras y se documenta en un entorno reproducible como Google Colab.

---

##  Objetivo General
Predecir el monto de préstamos digitales utilizando técnicas de regresión y redes neuronales artificiales a partir de variables disponibles en un dataset real.

---

## Objetivos Específicos
- Implementar un modelo de regresión lineal simple.
- Desarrollar una red neuronal con múltiples variables.
- Manipular y limpiar datos con Pandas y NumPy.
- Visualizar resultados con Matplotlib.
- Aplicar estructuras básicas de programación en Python.
- Usar GitHub como sistema de control de versiones.

---

##  Descripción del Dataset
El dataset fue descargado de [Kaggle](https://www.kaggle.com/) y contiene información de préstamos digitales otorgados en Perú. Las columnas más relevantes son:

- `ClienteID`: Identificador único.
- `FechaTransaccion`: Fecha de la transacción.
- `Monto`: Monto del préstamo.
- `TipoTransaccion`: Tipo de transacción (digital, presencial, etc.).
- `Ubicacion`: Ubicación geográfica.
- `FrecuenciaTransacciones`: Número de transacciones realizadas (variable creada para regresión).
- `UbicacionCodificada` y `TipoTransaccionCod`: Variables transformadas para la red neuronal.

---

## Tecnologías y Librerías Usadas
- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn
- TensorFlow / Keras
- Google Colab
- GitHub

---

## Modelos Aplicados

### 🔹 Regresión Lineal Simple
Se utiliza una sola variable predictora: `ventaPrestDig`, para estimar el `Monto`.  
Métricas: MAE, MSE  
Visualización: scatter plot con línea de regresión.

### Red Neuronal Artificial
- Variables de entrada: `promTrxDig3Um`, `trxDigitalUm`, `promSaldoPrest3Um`.
- Arquitectura:
  - 1 capa oculta (64 neuronas, ReLU)
  - 1 capa oculta adicional (32 neuronas, ReLU)
  - 1 capa de salida (lineal)
- Métricas: `mae`, `mse`
- Entrenamiento: 50 épocas, batch size de 10

 Visualizaciones:
- Evolución del error (`loss vs. epochs`)
- Comparación de valores reales vs. predichos

---

## Lógica de Programación
El código incluye:
- Un bucle `for` para calcular errores de predicción.
- Condicional `if` para filtrar predicciones cercanas.
- Uso de `listas` y `diccionarios` para almacenar resultados.

---

## Ejemplos de Visualizaciones
Agrega aquí capturas de pantalla desde el Colab:

- ![Gráfica Regresión Lineal](ruta/lineal.png)
- ![Gráfica Red Neuronal](ruta/neural.png)
- ![Error vs Épocas](ruta/loss_plot.png)

---

## Cómo Ejecutar este Proyecto
1. Abre el archivo `.ipynb` en [Google Colab](https://colab.research.google.com/).
2. Sube el dataset `prestamos_peru.csv` desde tu máquina.
3. Ejecuta cada celda secuencialmente.
4. Observa las predicciones, gráficas y métricas generadas.

---

## Conclusiones
- La regresión lineal es útil pero limitada cuando hay múltiples variables.
- Las redes neuronales capturan mejor relaciones no lineales complejas.
- Python con TensorFlow/Keras permite construir modelos potentes con poco código.
- Documentar en GitHub facilita compartir y colaborar en proyectos de ciencia de datos.

---

## Autor
**victor david huayta huaripoma**  
[GitHub](https://github.com/splat22/David1) | [Google Colad](https://colab.research.google.com/drive/1hra-xTwLFMWksw32DSZND2PtamB4kj20?usp=sharing)
