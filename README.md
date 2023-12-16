# QM2515-Proyecyo-Final
Red Neuronal en Python.

# Código de Predicción de Absorbancia

## Descripción General
Este código está diseñado para predecir la absorbancia y la desviación estándar de una solución usando datos de densidad y longitud de onda. Utiliza Python con bibliotecas como pandas, numpy, tensorflow y sklearn para cargar, procesar, modelar y predecir datos de absorbancia.

## Requisitos Previos
- Python 3.x
- Bibliotecas: pandas, numpy, tensorflow, sklearn

## Instalación de Bibliotecas
Si no tiene las bibliotecas necesarias, puede instalarlas usando pip:

```bash
pip install pandas numpy tensorflow scikit-learn
```

## Preparación de los Datos
1. Descargue el archivo de datos 'Datos-UV-Visible.xlsx'.
2. Coloque el archivo de datos en la misma carpeta que el script de Python.

## Ejecución del Código
Para ejecutar el código, simplemente corra el archivo `.py` en su entorno Python.

## Funcionamiento del Código
1. **Carga de Datos:** Inicia leyendo los datos desde el archivo Excel 'Datos-UV-Visible.xlsx'.
2. **Preprocesamiento:** Selecciona columnas relevantes, reemplaza valores infinitos con NaN, convierte los datos a numéricos y rellena valores NaN con la media.
3. **Escalado de Datos:** Utiliza `StandardScaler` de sklearn para normalizar los datos.
4. **Construcción del Modelo:** Construye un modelo de red neuronal usando TensorFlow y lo entrena con los datos.
5. **Predicción:** Permite al usuario ingresar valores de densidad y longitud de onda para predecir la absorbancia y la desviación estándar.

## Uso de las Funciones
- **cargar_modelo:** Carga un modelo guardado previamente.
- **predecir_absorbancia_std_cargado:** Realiza predicciones usando el modelo cargado, basándose en la densidad y longitud de onda ingresadas por el usuario.

## Guardar y Cargar Modelos
El código incluye funcionalidad para guardar el modelo entrenado y cargarlo posteriormente para realizar predicciones.
