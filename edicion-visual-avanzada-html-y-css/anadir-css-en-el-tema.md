Punto de partida: el tema **GeneratePress **admite que se le añada CSS adicional para modificar su apariencia por defecto. lo cual se puede hacer en `Escritorio > Apariencia > Editar CSS`

**Ejemplo práctico: **queremos reducir la altura de la barra de menú de 60px a 40px

#### 1º Cambiar en vivo el CSS en el navegador

Abrir en el navegador web \(ej. en Chrome\) `Menú > Más herramientas > Herramientas para desarrolladores`

Con el selector de objetos, detectar el ítem html y su propiedad CSS que queremos modificar. La vista "Computed" será más práctica.  ![](/assets/modificar-css-1.png)

Clic en la flecha en círculo negro para ir en la pestaña Styles donde esté definido el line-height:

![](/assets/modificar-css-2.png)

Modificar el valor de CSS en vivo y ver el efecto:

![](/assets/modificar-css-3.png)

Copiar el CSS que necesitamos:

![](/assets/modificar-css-4.png)

#### 2º Añadir el CSS en el Tema

Añadir el CSS que se ha detectado que se necesita en la zona que proporciona el tema GeneratePress, que está en `Escritorio > Apariencia > Editar CSS`

Y ahí se añade lo que se ha modificado "en vivo" en el navegador, pero sólo dejando la especificación de line-height será suficiente:

![](/assets/generatepress-css-modificado.png)


