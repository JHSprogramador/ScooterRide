# ScooterRide - Aplicación para alquilar patinetes eléctricos 🍃

> **Realizado por** Diego Bogo, Loreanny Santos, Álvaro Rodríguez y Juan Hidalgo 

Este proyecto para el módulo de programación, está enfocado a realizar una aplicación en **Visual Basic .NET** y practicar el uso de repositorios remotos con **git** y pruebas unitarias con **NUnit**. 

##  Funcionamiento de cada formulario🛠️

 - [Formulario de inicio de sesión](#formulario-de-inicio-de-sesión)
 - [Formulario de registro](#formulario-de-registro)
 - [Formulario de alquiler de patinetes](#formulario-de-alquiler-de-patinetes)
 - [Formulario perfil](#formulario-perfil)

### Formulario de inicio de sesión
La función de este formulario es simple, permitir al usuario iniciar sesión y acceder a la aplicación **una vez tenga una cuenta** registrada. En el caso de que no lo esté, tendría que crear una en el [formulario de registro](#formulario-de-registro).

![](https://cdn.discordapp.com/attachments/961944946611462144/979858736694845460/unknown.png)
### Formulario de registro
En este formulario, el usuario podrá crear una cuenta para poder acceder posteriormente a la aplicación.

![](https://cdn.discordapp.com/attachments/961944946611462144/979858377427529739/unknown.png)

### Formulario de alquiler de patinetes
En el formulario de alquiler, el usuario puede elegir entre la lista de patinetes disponibles el patinete que desee alquilar. Cada patinete disponible tiene una **foto**, su **nombre**, el **precio por cada día de alquiler** y el **stock** restante de este.

Si el usuario desea alquilar un patinete y **tiene el saldo suficiente** para alquilarlo presionará el **botón alquilar** y el patinete elegido pasará de ser de la clase **Patinete** a la clase **PatineteAlquilado** que contiene la propiedad única de *Fecha de Alquiler*.
> En caso de que **no tenga el saldo suficiente**, saldrá un mensaje que le preguntará si quiere recargar su saldo. En caso afirmativo, se abrirá el [formulario perfil](#formulario-perfil) donde podrá añadir el saldo que quiera, en caso negativo, no hará nada

Al haber presionado el botón, **el resto de patinetes no serán alquilables** por ese usuario y los controles de los mismos se desactivarán. El usuario tan solo podrá hacer click en el botón **"Devolver"**. Una vez hecho esto, el programa **calculará el costo total** según las horas que hayan pasado desde el momento en el que se realizó el alquiler y **se descontará del saldo asociado al usuario actual**.

![](https://cdn.discordapp.com/attachments/961944946611462144/979857969233674280/unknown.png)

### Formulario perfil
El formulario perfil **muestra los datos** del usuario y **permite a este recargar su saldo** en el momento que él desee. Tiene **dos formas** de recargar su saldo, añadiendo la cantidad deseada en la caja de texto y dándole al **botón "Añadir saldo"** o presionar uno de los 3 botones con **cantidades preestablecidas** para mayor comodidad.

![](https://cdn.discordapp.com/attachments/961944946611462144/979859268096389162/unknown.png)
