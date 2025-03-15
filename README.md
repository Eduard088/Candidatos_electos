# Reportes de Candidaturas Electas en México (2018-2023)

## Descripción del Proyecto

Este proyecto tiene como objetivo la limpieza, transformación y análisis de los reportes de candidaturas electas en México entre 2018 y 2023, utilizando los datos del Sistema de Estadística de Consulta de los Procesos Electorales del INE. La estructura del proyecto está organizada para facilitar el procesamiento de los datos y su posterior análisis mediante R y Quarto.

## Estructura del Proyecto

```
.
├── models/                   # Contiene los modelos y scripts relacionados
│   ├── R/                    # Carpeta para scripts en R
│   │   ├── script.R          # Script para el análisis y modelado de datos
│
├── {{cookiecutter.project_slug}}/  # Carpeta principal del proyecto
│   ├── data/                 # Datos utilizados en el proyecto
│   │   ├── raw/              # Datos originales sin procesar
│   │   ├── preprocessed/     # Datos con transformaciones iniciales
│   │   ├── processed/        # Datos limpios y estructurados
│   │   ├── final/            # Datos finales listos para análisis o modelado
│   │
│   ├── notebooks/            # Notebooks de Quarto con los análisis
│   │   ├── electos/          # Notebooks específicos sobre candidaturas electas
│   │   │   ├── 01_transformacion_datos.qmd
│   │   │   ├── 02_transformacion_datos.qmd
│   │   │   ├── 03_transformacion_datos.qmd
│   │
└── README.md                 # Documentación del proyecto
```

## Requisitos

- R (versión 4.0 o superior)
- Paquetes de R: `tidyverse`, `ggplot2`, `dplyr`, `readr`, `janitor`, `quarto`

## Instalación

1. Clona este repositorio:
    ```sh
    git clone https://github.com/tu_usuario/tu_repositorio.git
    ```
2. Instala los paquetes necesarios en R:
    ```r
    install.packages(c("tidyverse", "ggplot2", "dplyr", "readr", "janitor", "quarto"))
    ```

## Uso

### Limpieza y Transformación de Datos

Ejecuta los notebooks de Quarto en orden para realizar la limpieza y transformación de los datos:

```sh
quarto render notebooks/electos/01_transformacion_datos.qmd
quarto render notebooks/electos/02_transformacion_datos.qmd
quarto render notebooks/electos/03_transformacion_datos.qmd
```

### Análisis en R

Para realizar el análisis en R, ejecuta el siguiente script:

```r
source("models/R/script.R")
```

## Contribuciones

Las contribuciones son bienvenidas. Para reportar errores o sugerencias, abre un issue o envía un pull request en el repositorio.

## Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## Contacto

Para cualquier consulta, puedes escribirme a: **[eduardobareapoot@outlook.com]**