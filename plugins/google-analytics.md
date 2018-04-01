## Google Analytics

**¡No usar contadores de visitas! **porque incluirán propaganda y ventanas pop-up no deseadas que distorsionarán el Wordpress.

Para analizar los accesos al Wordpress, una completísima opción es usar la herramienta Google Analytics, de Google. Con Google Analytics, se conectará tu Wordpress con tu cuenta de Google GMail, y los datos y estadísticas de acceso al Wordpress quedarán registrados vinculados con tu usuario de GMail en la web de Google Analytics en [https://analytics.google.com](https://analytics.google.com).

Una forma rápida y sencilla de lograrlo es utilizar el plugin **Google Analytics Dashboard for WP \(GADWP\): **es un plugin que se conecta automáticamente con tu cuenta de GMail. A continuación se explica cómo hacerlo:

1. Instala y Activa el plugin **Google Analytics Dashboard for WP**

2. En el menú de Wordpress &gt; Google Analytics &gt; Ajustes generales, clic en Autorizar Plugin
3. ![](/assets/google-analytics-1.png)
4. Clic en "Obtener código de acceso". Si no estás conectado con tu cuenta de GMail, te solicitará iniciar sesión con una cuenta de GMail. Acto seguido se te mostrará un código que hay que copiar, para pegarlo en el Wordpress y posteriormente hacer clic en "Guardar código de acceso"
5. ![](/assets/google-analytics-2.png)
6. Ya tienes conectado Wordpress con Google Analytics. en el menú de Wordpress &gt; Google Analytics &gt; Ajustes generales debería verse los datos de conexión. 
7. ![](/assets/google-analytics-3.png)
8. Para desvincular Wordpress de Google Analytics puedes hacer clic en "Borrar autorización".

Los resultados de estadísticas de acceso los podrás ver en la web de [https://analytics.google.com](https://analytics.google.com) entrando con tu usuario de GMail, con completísima información y vistosos gráficos, tales como estos:

![](/assets/google-analytics-4.png)

Para más información sobre cómo utilizar la web de Google Analytics, en Internet encontraréis mucha información,  por ejemplo en este videotutorial: [https://www.youtube.com/watch?v=o-obgiAB1Kc](https://www.youtube.com/watch?v=o-obgiAB1Kc) o en esta web: [https://tuwebdecero.com/google-analytics-paso-a-paso/](https://tuwebdecero.com/google-analytics-paso-a-paso/)

## Ampliación: Proceso de creación de un código UA de Google Analytics

En caso que desees utilizar otro plugin para conectar Wordpress con Google Analytics, es muy probable que requieran el código identificativo de UA \(será algo similar a UA-1234567-8\) que lo proporciona Google Analytics. En estos casos, para poder usar Google Analytics, hay que conectar Wordpress con Google API. Para ello hay que ir a la web de Google Analytics [https://analytics.google.com](https://analytics.google.com/) y crear una nueva cuenta desde la zona de ADMINISTRADOR:

![](/assets/g_embedder_paso1.png)

Rellenamos los datos de la cuenta de Universal Analytics:

![](/assets/g_embedder_paso2.png)

Y podemos desactivar las opciones de Compartición de datos, haciendo clic en el botón de Obtener ID de seguimiento:

![](/assets/g_embedder_paso3.png)

En la Configuración de la propiedad, podremos obtener el Id de seguimiento de Universal Analytics:

![](/assets/g_embedder_paso4.png)

![](/assets/g_embedder_paso5.png)

Finalmente, este ID de seguimiento es el que tendremos que copiar y pegar en los plugins de Wordpress para que envíen la información a Google Analytics y poder visualizar las estadísticas en [https://analytics.google.com](https://analytics.google.com/)

