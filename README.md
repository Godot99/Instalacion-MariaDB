1. Primero, actualizamos la información de los paquetes
```
sudo apt update
```
![imagen](https://github.com/Godot99/Instalacion-MariaDB/blob/master/Imagenes/BD1.PNG)

2. Instalamos el paquete sudo "software-properties-common"
```
sudo apt-get install software-properties-common
```

3. Importamos y añadimos la llave del repositorio
```
sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xF1656F24C74CD1D8
sudo add-apt-repository \
'deb [arch=amd64,arm64,ppc64el] http://mirror.one.com/mariadb/repo/10.4/ubuntu bionic main'
```
![imagen](https://github.com/Godot99/Instalacion-MariaDB/blob/master/Imagenes/BD2.PNG)

4. Actualizamos los paquetes de nuevo con el comando del paso 1 e instalamos
```
sudo apt install mariadb-server
```

5. Para comprobar que lo tenemos correctamente instalado, usamos
```
mysql --version
```
Y nos debería de mostrar la versión tal que así
![imagen](https://github.com/Godot99/Instalacion-MariaDB/blob/master/Imagenes/BD3.PNG)
