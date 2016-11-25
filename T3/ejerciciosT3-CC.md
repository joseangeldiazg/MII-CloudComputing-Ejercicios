##Ejercicio 1: Instalar una máquina virtual Debian usando Vagrant y conectar con ella.


El primer paso será instalar Vagrant en nuestro workstation. Para ello podemos hacerlo mediante terminal o en mi caso al usar sistema operativo Mac OSX simplemente descargado el pkg de la web del producto e instalandolo. Tras ese punto debemos obtener una imagen debian ``.box`` para ello podemos encontrar varias [en esta web.](http://www.vagrantbox.es ).

Una vez elegida la imagen la descargamos y añadimos a Vagrant con el comando:

``vagrant box add debian https://github.com/holms/vagrant-jessie-box/releases/download/Jessie-v0.1/Debian-jessie-amd64-netboot.box``

Tras esto podremos ver que la imagen ha sido descargada y añadida correctamente en la siguiente imagen:


![Añadir máquina virtual](./images/vm.png "Máquina virtual añadida")


El paso siguiente será levantar la máquina virtual para ello primero debemos instalar Virtualbox si no lo tenemos ya instalado ya que Vagrant trabaja principalmente bajo esta plataforma de virtualización.

Tras eso ejecutamos los siguientes comandos

```vagrant init debian```

``` vagrant up```

Con lo que levantaremos la máquina virtual, momento tras el cual podremos ver que todo ha ido correctamente. 

![Máquina virtual arrancada](./images/vm2.png "Máquina virtual arrancada")

Tras esto solo queda conectar por ssh con ``vagrant ssh``.