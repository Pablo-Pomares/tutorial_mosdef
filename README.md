# Guía de Instalación

## Requisitos

Tener Anaconda intalado es recomendado.   

```
conda install -n base conda-libmamba-solver
conda env create -f enviroment.yml --solver=libmamba
conda activate tutorial_mosdef
```

### packmol

Este proceso solo aplica para Linux, para instalación en Windows vaya [aquí](https://m3g.github.io/packmol/download.shtml).

1. Se descargan los archivos comprimidos [aquí](https://github.com/m3g/packmol/releases), ya sea en formato `.tar.gz` or en `.zip`.
2. Se descomprimen usando:

```
tar -xvfz packmol-20.13.0.tar.gz
```

o

```
unzip -xvfz packmol-20.13.0.zip
```

3. Nos aseguramos de tener `gfortran` instalado:

```
sudo apt install gfortran
```

(En caso de no contar con un sistema basado en Debian sustituya con el administrador de paquetes correspondiente).

4. Entra al directorio de `packmol` y lo instalamos usando make:

```
cd packmol-20.13.0
./configure 
make
```

## Instalación de MoSDef

Para instalar las librerías de *MoSDeF* a través de Anaconda es necesario correr:

```
conda install mbuild foyer gmso
```

`mbuild`, `foyer` y `gmso` son los módulos de MoSDef.
