# Transformers aplicados a series de tiempo

Actividad de Deep Learning – Universidad de Cundinamarca. Autor: Daniel Contreras.

Pronóstico a 1 día de la temperatura mínima diaria de Melbourne (1981–1990) con ventanas de 30 días.

| Notebook | Contenido |
|---|---|
| `01_atencion_series_tiempo.ipynb` | LSTM con atención aditiva (Bahdanau) y visualización de pesos |
| `02_transformer_series_tiempo.ipynb` | Transformer Encoder desde cero (multi-cabeza, codificación posicional) |

## Ejecución
Abrir cada notebook en Google Colab (Archivo → Subir notebook) y ejecutar todo (Entorno de ejecución → Ejecutar todo). El dataset se descarga automáticamente.

## Resultados (conjunto de prueba, °C)
| Modelo | MAE | RMSE |
|---|---|---|
| Persistencia | 2.036 | 2.572 |
| LSTM | 1.716 | 2.201 |
| LSTM + atención | 1.716 | 2.198 |
| Transformer | 1.711 | 2.215 |

## Referencias
Vaswani et al. (2017), *Attention Is All You Need*. Bahdanau et al. (2015). Doshi (2020), *Transformers Explained Visually*.
