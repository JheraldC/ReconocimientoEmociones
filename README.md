# Trabajo académico: reconocimiento de expresiones faciales

Aplicación de escritorio que permite capturar rostros, entrenar modelos y visualizar una clasificación de expresiones mediante la cámara.

## Propósito y capacidades técnicas

Python, OpenCV contrib (módulo cv2.face), NumPy y Tkinter. El entrenamiento contempla EigenFaces, FisherFaces y LBPH.

## Contenido

- [main.py](main.py): interfaz de captura, entrenamiento y reconocimiento.
- [capturandoRostrosGUI.py](capturandoRostrosGUI.py): captura de muestras.
- [entrenando.py](entrenando.py): preparación y entrenamiento.
- [ReconocimientoEmociones.py](ReconocimientoEmociones.py): reconocimiento y visualización.
- [config.json](config.json): ubicación del dataset.
- [emojis](emojis): recursos visuales.

## Ejecución

Crear y activar un entorno virtual. Instalar dependencias y ejecutar:

```bash
python -m pip install opencv-contrib-python numpy
python main.py
```

Tkinter debe estar disponible en la instalación de Python. **Antes de entrenar**, ajustar `dataPath` en `config.json` a una carpeta del equipo actual y capturar las muestras. El repositorio conserva una ruta del entorno original; el dataset y los modelos generados no se incluyen.

## Alcance

La clasificación corresponde a patrones visuales aprendidos del dataset. No determina el estado emocional interno de una persona. Se requiere cámara, entorno gráfico y validación con muestras independientes.

Este repositorio conserva un trabajo académico. Los comandos describen el uso previsto del código; la documentación no equivale a una validación de ejecución en todos los entornos.

## Versiones relacionadas

La [variante con análisis de calidad](https://github.com/JheraldC/ReconocimientoEmociones-CG) incorpora configuración de SonarQube.
