# 🌳 Árboles de Decisión para Regresión

<p align="center">
  <img src="https://st2.depositphotos.com/1121376/6933/i/450/depositphotos_69332881-stock-photo-mighty-oak-tree.jpg" width="500" alt="Decision Tree Regression Algorithm">
  <br>
  <b>Decision Tree Regression Algorithm</b>
</p>

## 📚 Recursos

- 📄 **Documento interactivo**: [Ver en RPubs](https://rpubs.com/Alej5ndro/DecisionTreesRegression)
- 📄 **Documento acceso a repositrio**:[Ver en GitHub](https://alej2andro.github.io/Decision-Tree-Regression-Algorithm/)
- 📖 **Referencia**: Breiman et al. (1984) - Classification and Regression Trees

## ¿De qué se trata este proyecto?

Este proyecto analiza **cómo funcionan los Árboles de Decisión** desde sus fundamentos matemáticos. No es solo ejecutar código: es entender **por qué** el algoritmo toma cada decisión.

Uso el dataset Ames Housing (precios de viviendas) para construir un modelo predictivo, pero el objetivo real es **descomponer la matemática** detrás de cada paso.

## 🎯 Lo que aprenderás aquí

- Cómo el algoritmo minimiza el error (MSE) en cada división del árbol
- Por qué la poda previene el sobreajuste
- Cómo validar que un modelo realmente funciona (no solo "parece funcionar")
- Qué significan las métricas (R², RMSE, MAE)

**Filosofía**: Entender > Ejecutar. Las matemáticas son la base de todo.

## 📊 Datos

- **Dataset**: Ames Housing (2,930 viviendas en Iowa, 2006-2010)
- **Objetivo**: Predecir precio de venta
- **Variables clave**: Calidad construcción, área habitable, tamaño garage

## 🛠️ Tecnología

- **R + RStudio**: Para análisis estadístico
- **Quarto**: Para crear documento HTML interactivo
- **Librerías**: rpart, ggplot2, caret, corrplot

## 📁 Archivos del proyecto

```
├── Arboles-decisiones-regresion.qmd    # Código fuente
├── Arboles-decisiones-regresion.html   # Documento final (abrir en navegador)
├── modelo_arbol_regresion.rds          # Modelo entrenado
└── README.md                           # Este archivo
```

## 🔍 Proceso

1. **Exploración de datos**: ¿Qué tienen los datos? ¿Hay valores raros?
2. **Construcción del árbol**: Empezar simple, luego optimizar
3. **Validación cruzada**: ¿Funciona con datos que no vio antes?
4. **Optimización**: Probar 81 combinaciones de parámetros
5. **Evaluación final**: ¿Qué tan bueno es realmente?

## 📈 Resultados

| Modelo | Error (RMSE) | Varianza Explicada (R²) |
|--------|--------------|-------------------------|
| Baseline (predecir promedio) | $79,060 | 0% |
| **Modelo Final** | **$32,120** | **93%** |

**Mejora**: 59% menos error que simplemente predecir el precio promedio.

**Variables más importantes**:
1. Calidad de construcción (36%)
2. Área habitable (28%)
3. Tamaño de garage (15%)

## 🚀 Cómo usarlo

**Instalar R y RStudio**, luego:

```r
# Instalar paquetes necesarios
install.packages(c("rpart", "rpart.plot", "caret", "ggplot2", 
                   "corrplot", "dplyr", "knitr", "AmesHousing"))

# Renderizar documento
quarto::quarto_render("Arboles-decisiones-regresion.qmd")
```

O simplemente abre el archivo `.html` en tu navegador.

## 💡 Lo que me motiva

> *"No basta con saber ejecutar algoritmos. Hay que entender la matemática que los hace funcionar."*

En Machine Learning es fácil copiar código y confiar en que "funciona". Pero **la maestría está en el "por qué"**:

- ¿Por qué este split reduce el error más que otros?
- ¿Por qué mantener outliers mejora el modelo?
- ¿Cómo sé si mi modelo es estable o tuvo suerte?

**Las matemáticas explican todo. La curiosidad es el motor del aprendizaje.**

## 📬 Contacto

**Alejandro Figueroa Rojas**

- LinkedIn: [linkedin.com/in/alejandrofigueroarojas](https://www.linkedin.com/in/alejandrofigueroarojas)
- RPubs: [rpubs.com/Alej5ndro](https://rpubs.com/Alej5ndro)
- Email: alejandro.figueroa.rojas@gmail.com

---

⭐ **Si crees que entender es mejor que memorizar, este proyecto es para ti**

💬 **¿Dudas? ¿Ideas? Escríbeme**
