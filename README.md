[![Abrir en Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/fcorvetto/cell-pose/blob/main/Notebook_Cellpose.ipynb)


# Segmentación automática de células con Cellpose

Notebook de Python para correr **Cellpose**, un software de segmentación de células, usando Google Colaboratory.

## ¿Qué hace?
Toma imágenes de microscopía y segmenta automáticamente células o núcleos, generando ROIs exportables para análisis en ImageJ.

## Requisitos
- Cuenta de Google (para usar Colab)
- Imágenes en formato `.png` o `.tiff` guardadas en Google Drive

## Cómo usarlo
1. Abrí el notebook en Google Colab
2. Montá tu Google Drive y copiá la ruta de tu carpeta de imágenes
3. Instalá las dependencias (hay una celda para eso)
4. Seguí las instrucciones del notebook paso a paso

## Parámetros principales
| Parámetro | Descripción | Default |
|---|---|---|
| `model_type` | Modelo de segmentación (`cyto2`, `nuclei`, etc.) | `cyto2` |
| `diametro` | Diámetro promedio de células en px (post-downscaling) | `100` |
| `flow_threshold` | Controla cantidad de ROIs detectadas | `0.4` |
| `cellprob_threshold` | Sensibilidad en áreas de poca señal | `0.0` |

## Referencia
- [Documentación oficial de Cellpose](https://cellpose.readthedocs.io/en/latest/)
