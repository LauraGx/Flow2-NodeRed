# Flow2-NodeRed
Este es el segundo ejercicio utilizando NodeRed.

## Introducción

El flow 2 es el segundo ejercicio a realizar  con NodeRed. El siguiente ejercicio consiste en conectar un nodo Inject con un nodo Debug y automatizarlo para que genere un TimeStamp cada un segundo y agregando un nodo function  que convierta timestamp en fecha legible.

## Material Necesario

Para realizar este flow necesitas lo siguiente:

- [Ubuntu 20.04](https://releases.ubuntu.com/20.04/)
- [NodeJS](https://nodejs.org/es/)
    - [NPM](https://www.npmjs.com/)
    - [NodeRed](https://nodered.org/docs/getting-started/local)

## Material de referencia

En los siguientes enlaces puedes encontrar cursos en la plataforma de edu.codigoiot.com que te permitirán realiar las configuraciones necesarias

- [Instalación de Virutal Box y Ubuntu 20.04](https://edu.codigoiot.com/course/view.php?id=812)
- [Instalación de NodeRed](https://edu.codigoiot.com/course/view.php?id=817)
- [Introducción a NodeRed](https://edu.codigoiot.com/course/view.php?id=278)

## Instrucciones

### Requisitos previos

Para que este flow funcione, debes cumplir con los siguientes requisitos previos

1. Instalación de NodeJS. Se recomienda tener instalado NodeJS en alguna versión LTS. Al momento de creación de este documento, se usó la versión 18.12LTS. Esta instalación debe incluir las Build-Tools para hacer uso de NPM
2. Instalación de NodeRed. La instalación se realiza por NPM. Al momento de la creación de este contenido, se usó la versión 3.0.2

### Instrucciones de preparación del entorno

Para ejecutar este flow, es necesario lo siguiente

- Arrancar NodeRed con el comando node-red
- Exportar el flow1 (trabajo anterior) e importarlo y cambiar el nombre a flow2.
- Modificar el nodo Inject con intervalo de un segundo para mandar el TimeStamp
- Por ultimo agregar un nodo function y en la pestaña "On Message" que colocará el siguiente codigo.

// Lo que está después de “//” son comentarios // Crea un objeto Date a partir del payload enviado por timestamp var date = new Date(msg.payload); // Cambia el payload para que sea una fecha con formato msg.payload = date.toString(); // Regresa el mensaje para que se envíe al sigueinte nodo return msg;
- Guardar cambios con Deploy

### Instrucciones de operación

Para observar el resutlado de este flow, sólo es necesario abrir la pestaña Debug.

## Resultados

A continuación puede verse una vista previa del resultado del flow 2

![](https://github.com/Cecilia-X-M/flow2-NodeRed/blob/main/flow2.png)

# Créditos

Desarrollado por Diana Laura Aragon 

- [GitHub](https://github.com/LauraGx)
