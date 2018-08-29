##Instalación de Python 3.x, Virtualenv, pip.

El siguiente documento tiene como finalidad dejar instalado lo básico para iniciar un proyecto con python.  

####Python 3.x
Para instalar python 3.6 en **Ubuntu 14.04 y 16.04** puedes seguir lo siguiente:  

~~~
sudo add-apt-repository ppa:deadsnakes/ppa
sudo apt-get update
sudo apt-get install python3.6
~~~  
Luego de haber ejecutado lo anterior se puede comprobar la versión instalada con:  
~~~
python3.6 -V
~~~  
  

####PIP  

Instalar pip es un sistema de gestión de paquetes utilizado para instalar y gestionar paquetes de software que se encuentran en Python Package Index, Estos paquetes de software están escritos en Python y, por lo general, se usan para extender o mejorar una aplicación de Python.  
Mediante la terminal ejecute las siguientes lineas:  

- Actualice la lista de paquetes y actualice todo el sofware de su sistema a la última versión disponible:
~~~
sudo apt-get update && sudo apt-get -y upgrade
~~~  

- Una vez que se complete la actualización, puede continuar e instalar Pip en ubuntu:  
~~~
sudo apt-get install python-pip
~~~
- Verifica la instalación de pip en ubuntu:  
~~~
pip -V
~~~  
  
####Virtualenv  
Un entorno virtual de Python es un ambiente creado con el objetivo de aislar recursos como librerías y entorno de ejecución, del sistema principal o de otros entornos virtuales. Lo anterior significa que en el mismo sistema, maquina o computadora, es posible tener instaladas multiples versiones de una misma librería sin crear ningún tipo de conflicto.
Para instalar **virtualenv** puedes seguir lo siguiente con pip:  
~~~
sudo pip install virtualenv
//para comprobar la versión instalada
virtualenv --version
~~~