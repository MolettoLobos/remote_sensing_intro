# remote_sensing_intro
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3120/)

## Objetivo de este repositorio
Este repositorio es una introducción para estudiantes que empiezan desde cero en teledetección con Python.

Incluye un entorno listo para trabajar con:
- Python 3.12
- JupyterLab / Notebook
- Librerías geoespaciales y de teledetección
- Google Earth Engine (GEE)

## 1) Instalar herramientas base
Antes de usar el repo, instala:

1. Git  
https://git-scm.com/downloads

2. Cuenta de GitHub  
https://github.com/

3. Anaconda o Miniconda  
- Anaconda: https://www.anaconda.com/download  
- Miniconda (recomendado si quieres algo liviano): https://docs.conda.io/en/latest/miniconda.html

Verifica instalación en terminal:
```bash
git --version
conda --version
python --version
```

## 2) Descargar este repositorio
Si ya tienes el repositorio en GitHub, clónalo:
```bash
git clone https://github.com/<tu-usuario>/remote_sensing_intro.git
cd remote_sensing_intro
```

Si estás trabajando localmente en esta carpeta, solo entra al directorio del proyecto:
```bash
cd remote_sensing_intro
```

## 3) Crear y activar el entorno de trabajo
Crear entorno con `environment.yml`:
```bash
conda env create -f environment.yml
```

Activar entorno:
```bash
conda activate landsat_sentinel2_downloader
```

Registrar kernel para Jupyter:
```bash
python -m ipykernel install --user --name landsat_sentinel2_downloader --display-name "Python (landsat_sentinel2_downloader)"
```

## 4) Abrir Jupyter
```bash
jupyter lab
```
o
```bash
jupyter notebook
```

## 5) Actualizar el entorno
Si editas `environment.yml`, actualiza paquetes con:
```bash
conda env update -f environment.yml --prune
```
