<!-- hide -->
# K-Vecinos más cercanos - Guía paso a paso
<!-- endhide -->

- Comprender un dataset nuevo.
- Modelar los datos utilizando un KNN.
- Analizar los resultados y optimizar el modelo.

<how-to-start>

## 🌱 Cómo iniciar este proyecto

Sigue las siguientes instrucciones:

1. Crea un nuevo repositorio basado en el [proyecto de Machine Learning](https://github.com/4GeeksAcademy/machine-learning-python-template) [haciendo clic aquí](https://github.com/4GeeksAcademy/machine-learning-python-template/generate).
2. Abre el repositorio creado recientemente en Codespace usando la [extensión del botón de Codespace](https://docs.github.com/en/codespaces/developing-in-codespaces/creating-a-codespace-for-a-repository#creating-a-codespace-for-a-repository).
3. Una vez que el VSCode del Codespace haya terminado de abrirse, comienza tu proyecto siguiendo las instrucciones a continuación.

</how-to-start>


## 📝 Instrucciones


### Clasificador de Vinos con KNN

Entrena un modelo de K-Vecinos más Cercanos (KNN) para predecir la calidad de un vino tinto a partir de sus características químicas. ¿Podría una IA ayudarte a elegir un vino digno de sommelier?

Utilizaremos el siguiente dataset de vinos tintos extraido de [Wine Quality Data Set - UCI](https://archive.ics.uci.edu/dataset/186/wine+quality)

```text
https://raw.githubusercontent.com/4GeeksAcademy/k-nearest-neighbors-project-tutorial/refs/heads/main/winequality-red.csv
```

#### Descripción de las columnas

Cada fila representa un vino. Las columnas describen su composición química:

- fixed acidity, volatile acidity, citric acid

- residual sugar, chlorides

- free sulfur dioxide, total sulfur dioxide

- density, pH, sulphates, alcohol

La columna objetivo es **label**:

- 0 = Baja calidad

- 1 = Calidad media

- 2 = Alta calidad

### ¡Empecemos! 😎

1. **Carga los datos.** Carga el CSV con Pandas y explora su estructura.
2. **Entrena el modelo KNN:**
    - Separa las variables independientes (X) del objetivo (y).

    - Divide en conjunto de entrenamiento y prueba (80/20).

    - Escala los datos si es necesario (¡muy recomendable con KNN!).

    - Entrena el modelo con un valor de k inicial.

3. Evalúa el rendimiento usando:

    - `accuracy_score`

    - `confusion_matrix`

    - `classification_report`

4. **Optimización de k.** Crea un bucle para probar diferentes valores de k (por ejemplo, de 1 a 20).

    - Guarda los resultados en una lista.

    - Grafica accuracy vs k para encontrar el mejor valor.

## ¿Te sientes confiado/a?

Crea una función que reciba valores numéricos y prediga la calidad

```python
predict_wine_quality([7.4, 0.7, 0.0, 1.9, 0.076, 11.0, 34.0, 0.9978, 3.51, 0.56, 9.4])
>>> "Este vino probablemente sea de calidad media 🍷"
```

> Nota: También incorporamos muestras de solución en `./solution.ipynb` que te sugerimos honestamente que solo uses si estás atascado por más de 30 minutos o si ya has terminado y quieres compararlo con tu enfoque.

## 🚀 Haz visible tu trabajo

Trabajaste con un dataset real del [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/186/wine+quality), aplicaste modelos de clasificación supervisada, analizaste características químicas y desarrollaste una función que **simula el juicio de un sommelier usando IA**. ¡Eso merece ser contado!


### ¿Qué compartir?

Comparte una **frase de insight** que muestre cómo la IA puede clasificar la calidad del vino con base en su composición. Añade una gráfica de precisión vs. k (muy visual) o una predicción divertida con `predict_wine_quality()`.

---

### ✨ Ejemplo posteable

> **"¿Puede la inteligencia artificial predecir la calidad de un vino? 🍷 Entrené un modelo KNN con datos reales del UCI ML Repo y alcancé una precisión del 73% al clasificar vinos en baja, media y alta calidad usando solo su composición química. Los datos no mienten: ¡el alcohol y el sulfato son más reveladores que una etiqueta! 😉 #MachineLearning #DataScience #WineLovers #IA #scikitLearn"**




## 🚛 Cómo entregar este proyecto

Una vez que hayas terminado de resolver el caso práctico, asegúrate de confirmar tus cambios, haz push a tu repositorio y ve a 4Geeks.com para subir el enlace del repositorio.
