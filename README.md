# Guía de Instalación

## Requisitos

### py3Dmol

Si se está instalando MoSDef a través de Anaconda:

```
conda install py3Dmol
```

O por pip:

```
pip3 install py3Dmol
```

### packmol

1. Se descargan los archivos comprimidos [aquí](https://github.com/m3g/packmol/releases), ya sea en formato `.tar.gz` or en `.zip`.
2. Se descomprimen usando:

```
tar -xvfz packmol-20.13.0.tar.gz
```

o

```
unzip -xvfz packmol-20.13.0.tar.gz
```

3. Nos aseguramos de tener `gfortran` instalado:

```
sudo apt install gfortran
```

4. Entra al directorio de `packmol` y lo instalamos usando make:

```
cd packmol-20.13.0
./configure 
make
```

### Anaconda

Para instalar las librerías de *MoSDeF* a través de Anaconda es necesario correr:

```
conda install mbuild foyer
```

`mbuild` y `foyer` son los módulos de MoSDef.
