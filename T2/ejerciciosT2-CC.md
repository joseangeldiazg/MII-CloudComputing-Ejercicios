#Ejercícios del tema 2 de Cloud Computing

##Ejercício 1: Instalar chef en la máquina virtual que vayamos a usar.

Para instalar chef en local (workstation) usamos el siguiente comando abriendo una terminal.

  curl -L https://www.opscode.com/chef/install.sh | sudo bash

Tras lo cual tendremos el siguiente resultado que nos indica que Chef está instalado.

![Instalacion chef local](./images/installcheflocal.png "Instalacion chef local")


Para instalar chef en la máquina virtual que vamos a usar, simplemente tenremos que levantar la instancia, conectar por ssh y ejecutar el mismo comando que hemos visto anteriormente, teniendo en cuenta que para acceder como superusuario en la máquina virtual podremos usar el siguiente comando si no conocemos la contraseña como es el caso de una máquina virtual de Amazon AWS,  AMI EC2.

  sudo su -

Tras esto podemos ver el siguiente resultado que nos indica que está bien instalado.

![Instalacion chef remoto](./images/installchefmv.png "Instalacion chef remoto")
