# Guía de Instalación

## Requisitos

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

(O con el administrador de paquetes del sitema)

4. Entra al directorio de `packmol` y lo instalamos usando make:

```
cd packmol-20.13.0
./configure 
make
```

## Instalación de MoSDeF


Se pueden instalar los requisitos a través de Anaconda siguiendo:

```
git clone https://github.com/Pablo-Pomares/tutorial_mosdef
cd tutorial_mosdef
conda install -n base conda-libmamba-solver
conda env create -f enviroment.yml --solver=libmamba
conda activate tutorial_mosdef
```

Se recomienda realizar la instalación con anticipación ya que puede tardar un poco.
Una manera más rápida (opcional) es a través de `mamba` en miniforge:

```
git clone https://github.com/Pablo-Pomares/tutorial_mosdef
cd tutorial_mosdef
mamba env create -f enviroment.yml 
mamba activate tutorial_mosdef
```
