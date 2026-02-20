# landsat_sentinel2_downloader
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Python](https://img.shields.io/badge/python-3.12-blue.svg)](https://www.python.org/downloads/release/python-3120/)
[![CI/CD Status](https://github.com/agrospace/landsat_sentinel2_downloader/actions/workflows/CICD_ETL.yaml/badge.svg)](https://github.com/agrospace/landsat_sentinel2_downloader/actions/workflows/CICD_ETL.yaml)

Repository for Sentinel-2 and Landsat data download for Sen2Like (S2L) assimilation and processing.

![Example Image](imgs/AS-S2L.drawio.png)

## Objetivo de este repositorio
Este repositorio es una introducción para estudiantes que empiezan desde cero en teledetección con Python.

Incluye un entorno listo para trabajar con:
- Python 3.12
- JupyterLab / Notebook
- Librerías geoespaciales y de teledetección para Landsat y Sentinel-2
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
git clone https://github.com/<tu-usuario>/landsat_sentinel2_downloader.git
cd landsat_sentinel2_downloader
```

Si estás trabajando localmente en esta carpeta, solo entra al directorio del proyecto:
```bash
cd landsat_sentinel2_downloader
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

## 6) Publicar el repo en GitHub (público)
1. Crea un repositorio público en GitHub (sin inicializar con README).
2. Desde esta carpeta, ejecuta:
```bash
git init
git add .
git commit -m "Initial commit: intro + conda environment"
git branch -M main
git remote add origin https://github.com/<tu-usuario>/landsat_sentinel2_downloader.git
git push -u origin main
```
