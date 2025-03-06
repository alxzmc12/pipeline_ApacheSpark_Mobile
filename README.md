# Proyecto Final - Análisis de Características de Teléfonos Móviles con Apache Spark

¡Bienvenido al repositorio del proyecto final del Máster en Big Data! Este trabajo se centra en el análisis de un conjunto de datos de teléfonos móviles utilizando Apache Spark en Google Colab. A continuación, se detallan los pasos para replicar el proyecto y entender su estructura.

---

## 📋 Descripción del Proyecto
El objetivo de este proyecto es analizar un dataset de características de teléfonos móviles para extraer información relevante mediante operaciones de transformación y agregación con Spark. Se generan tres tablas de salida que resumen:
1. **Información básica del dispositivo** (batería, velocidad del procesador, memoria, etc.).
2. **Calidad de la cámara** según su resolución.
3. **Relación entre el peso del dispositivo y la capacidad de la batería**, segmentada en grupos.

---

## ⚙️ Requisitos Previos
- **Google Colab**: El proyecto está diseñado para ejecutarse en este entorno.
- **Dataset**: Archivo CSV (`test.csv`) con datos de teléfonos móviles.
- **Apache Spark 3.5.4**: Configurado automáticamente en el notebook.

---

## 🛠️ Instrucciones de Configuración

### 1. Subir el archivo `.ipynb`
- Sube el notebook `ProyectoFinal_Mobile.ipynb` a tu entorno de Google Colab.

### 2. Crear la estructura de carpetas
- Dentro de Colab, crea una carpeta llamada **`input`** en el directorio raíz (`/content/`).
- Sube el archivo `test.csv` a la carpeta `input`. La ruta final debe ser:  
  `/content/input/test.csv`.

### 3. Ejecutar el Notebook
- Abre el notebook y ejecuta todas las celdas en orden. El código:
  - Instalará dependencias (Java, Spark).
  - Cargará y procesará el dataset.
  - Generará las tablas de salida con análisis específicos.

---

## 📂 Estructura del Proyecto
/content/
├── ProyectoFinal_Mobile.ipynb # Notebook principal
└── input/
└── test.csv # Dataset de entrada

## 📊 Uso del Código
### Principales operaciones realizadas:
1. **Configuración de Spark**: Instalación de Java y Spark, inicialización de la sesión.
2. **Carga y exploración de datos**:
   - Verificación de valores nulos.
   - Estadísticas descriptivas del dataset.
3. **Transformaciones**:
   - Clasificación de calidad de cámara (`fc_quality`).
   - Segmentación por peso del dispositivo y cálculo de batería promedio por grupo.
4. **Generación de tablas**:
   - Tabla 1: Información técnica básica.
   - Tabla 2: Resolución y calidad de cámara.
   - Tabla 3: Relación peso-batería.

---

## 📈 Resultados
Las tablas generadas permiten visualizar:
- Dispositivos con mayor capacidad de batería y su relación con el peso.
- Clasificación de cámaras para identificar modelos con características destacadas.
- Promedios técnicos para comparativas entre grupos.

---

## 🚨 Notas Adicionales
- **Ubicación del CSV**: Si el código falla, verifica que el archivo `test.csv` esté en `/content/input/`.
- **Personalización**: Para usar otro dataset, ajusta las columnas y transformaciones según los nuevos datos.

---

## 🎓 Conclusión
Este proyecto demuestra el uso de Spark para el procesamiento de datos en Big Data, destacando técnicas de limpieza, transformación y análisis segmentado. Es escalable para incorporar más métricas o modelos predictivos en futuras iteraciones.

¡Gracias por revisar este trabajo! Para cualquier consulta, no dudes en contactarme.  
**Estudiante del Máster en Big Data**  
[Tu nombre] | [Correo electrónico]  
