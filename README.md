# MetroMX Afluencia: Predicciones de Afluencia Diaria en el Metro CDMX

##  Descripción

MetroMX Afluencia es un proyecto que utiliza un modelo de series temporales (LSTM multi-input) para **predecir la afluencia diaria de pasajeros por estación en el Metro de la Ciudad de México (2021–2025)**. El objetivo es superar métodos simples y proporcionar insights accionables sobre qué tan lleno estará el sistema en una fecha dada.

---

##  Métrica de Desempeño

El modelo logra resultados que superan baseline históricos simples:

| Modelo              | MAPE (VALID)        |
|---------------------|---------------------|
| LSTM multi-input    | **17.3 %** (mejor)  |
| Naive-7             | 18.3 %              |
| Promedio 4 semanas  | 19.5 %              |

---

##  Funcionalidades

- Predicción día-a-día por estación (2021–2023 train, 2024 valid, 2025 test)  
- Comparativa con baselines históricos  
- Evaluación detallada por estación y cuartiles de afluencia  
- Visualización gráfica para casos buenos vs. difíciles  
- Uso de escalado por estación y embeddings (LSTM con identidad de estación y días de la semana)

---

##  Estructura del Repositorio

| Carpeta/Archivo                    | Descripción |
|-----------------------------------|-------------|
| `metro_notebook.ipynb`            | Notebook con todo el flujo: procesamiento, modelado, evaluación |
| `README.md`                       | Este archivo de presentación del proyecto |
| `plots/`                          | Carpeta con imágenes usadas en el README |
| `requirements.txt`                | Dependencias necesarias para ejecutar el notebook |

---

##  Cómo usar

1. **Clonar el repositorio**  
   ```bash
   git clone https://github.com/TU_USUARIO/metro-mx-afluencia.git
   cd metro-mx-afluencia
