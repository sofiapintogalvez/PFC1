# Detección de Clones de Código: Un análisis comparativo de enfoques de detección

## Descripción

Este repositorio contiene las implementaciones, adaptaciones y resultados experimentales de dos técnicas de detección de clones de código evaluadas sobre BigCloneBench.

## Técnicas implementadas

### Toma - Feng et al.

- Enfoque basado en tokens.
- Seis medidas de similitud.
- Clasificador Random Forest.
- Validación cruzada de 10 pliegues.
- Implementación en Python.

### Almatrafi et al.

- Enfoque basado en modelos de lenguaje.
- Qwen2.5-Coder-1.5B-Instruct.
- Ajuste mediante QLoRA.
- Cuantización de 4 bits.
- Implementación en Google Colab.

## Dataset

BigCloneBench, compuesto por pares de funciones Java.

| Característica | Toma | Almatrafi |
|---|---:|---:|
| Total de pares utilizados | 548477 | 2200 |
| Pares clon | 269631 | 1100 |
| Pares no clon | 278846 | 1100 |

## Resultados experimentales

| Técnica | Experimento | Precisión | Recall | F1-score |
|---|---|---:|---:|---:|
| Toma | Muestra | 0.8744 | 0.8029 | 0.8369 |
| Toma | Final | 0.9295 | 0.8792 | 0.9036 |
| Almatrafi | Muestra | 0.9762 | 0.8200 | 0.8913 |
| Almatrafi | Final | 0.9865 | 0.9490 | 0.9674 |

Los resultados fueron obtenidos bajo diferentes condiciones experimentales.

## Entorno experimental

| Característica | Toma | Almatrafi |
|---|---|---|
| Entorno | macOS | Google Colab |
| Hardware | Apple M3 Pro | NVIDIA Tesla T4 |
| Lenguaje | Python | Python |

## Organización del repositorio

- `Toma/`: implementación y resultados experimentales.
- `Almatrafi/`: notebooks, configuración y resultados experimentales.
- `Comparacion/`: gráficos comparativos.

## Autora

Sofía Pinto Gálvez

Ciencia de la Computación

Universidad Católica San Pablo - 2026
