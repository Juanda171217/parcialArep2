# PARCIAL AREP 2

## Juan David Martinez Cardozo

Para realizar el parcial, primero se realizo el codigo para demostar la secuencia 

Pruebas del funcionamiento del progrmama localmente:

[![p1.png](https://i.postimg.cc/K8SZYscj/p1.png)](https://postimg.cc/qzwfbw3H)

[![p2.png](https://i.postimg.cc/y8HkGNZL/p2.png)](https://postimg.cc/RNgS64Gt)

Para subir el trabajo a docker, se puso el archivo Dockerfile en la raiz del proyecto

[![p5.png](https://i.postimg.cc/fRG5pmv6/p5.png)](https://postimg.cc/zyknRL6j)

Luego se creo la imagen Docker con el siguiente comando

```
docker build --tag parcialarep .

```

Se creo la imagen

[![p6.png](https://i.postimg.cc/t43VR6b0/p6.png)](https://postimg.cc/v4mm3cDX)

Luego a partir de la imagen creada se creo una instancia de un contenedor docker independiente de la consola, con el puerto 6000 enlazado a un puerto físico de la máquina

Se uso el siguiente comando 
```
docker run -d -p 5000:6000 --name dockercontainer parcialarep
```

[![p7.png](https://i.postimg.cc/cHnvjtX5/p7.png)](https://postimg.cc/S2mQYR0W)

Visualizacion imagenes

[![p8.png](https://i.postimg.cc/25Y93nBn/p8.png)](https://postimg.cc/xXs34J5d)

Luego se creo una referencia a la imagen con el nombre del repositorio creado en Docker Hub

[![p9.png](https://i.postimg.cc/bJWByW0w/p9.png)](https://postimg.cc/Kk7NQ9s6)

Se hizo push al repositorio en Docker Hub

[![p10.png](https://i.postimg.cc/6qVLkmYS/p10.png)](https://postimg.cc/rRmrWQ6C)

[![p11.png](https://i.postimg.cc/bvG0yJm1/p11.png)](https://postimg.cc/1gQVM9hz)


Luego para subir el trabajo realizado a AWS se creo la instancia EC2

[![p3.png](https://i.postimg.cc/Qd8j5K5Z/p3.png)](https://postimg.cc/F76tXRDT)

Se accedio a la maquina virtual y se instalo docker

[![p4.png](https://i.postimg.cc/15ykYhzp/p4.png)](https://postimg.cc/rzYZKHxm)

Luego a partir de la imagen creada en Dockerhub se creo una instancia de un contenedor docker independiente de la consola con el puerto 6000 enlazado a un puerto físico de la máquina 

[![p12.png](https://i.postimg.cc/J0d4z16B/p12.png)](https://postimg.cc/sG7RnRRV)


Luego se abrio el puerto 5000 que es donde correra nuestra aplicacion

[![p13.png](https://i.postimg.cc/Kz3yDnJ4/p13.png)](https://postimg.cc/bDPMz2Xj)

Por ultimo se muestra el funcionamiento de la aplicacion desplegada en AWS

[![p14.png](https://i.postimg.cc/nrKg3T7V/p14.png)](https://postimg.cc/4HdWd6Bj)

[![p15.png](https://i.postimg.cc/fT2BD6wn/p15.png)](https://postimg.cc/qzK8GDhj)

[![p16.png](https://i.postimg.cc/Z5XHypBw/p16.png)](https://postimg.cc/cvMwpKc3)

