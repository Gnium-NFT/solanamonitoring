Creación de informes privados de una vulnerabilidad de seguridad
Algunos repositorios públicos configuran avisos de seguridad para que cualquier usuario pueda notificar vulnerabilidades de seguridad directamente y de forma privada a los mantenedores.

En este artículo
Acerca de la creación de informes privados de una vulnerabilidad de seguridad
Creación de informes privados de una vulnerabilidad de seguridad
Los propietarios y administradores de repositorios públicos pueden habilitar informes de vulnerabilidades privados en sus repositorios. Para obtener más información, vea «Configuración de informes de vulnerabilidades privadas para un repositorio».

Note

Si tienes permisos de administrador o seguridad para un repositorio público, no es necesario que envíes un informe de vulnerabilidades. En su lugar, puedes crear directamente el borrador de un aviso de seguridad. Para más información, consulta Creación de un aviso de seguridad de repositorio.
La capacidad de notificar de forma privada una vulnerabilidad en un repositorio no está relacionada con la presencia de un archivo SECURITY.md en la raíz de ese repositorio o un directorio docs.
El archivo SECURITY.md contiene la directiva de seguridad para el repositorio. Los administradores del repositorio pueden agregar y usar este archivo para proporcionar instrucciones públicas sobre cómo notificar una vulnerabilidad de seguridad en su repositorio. Para más información, consulta Agregar una política de seguridad a tu repositorio.
Solo puedes notificar una vulnerabilidad de forma privada para los repositorios en los que está habilitado el informe de vulnerabilidades privado y no tienes por qué seguir las instrucciones del archivo SECURITY.md. Este proceso de informes es totalmente privado y GitHub notifica tu envío directamente a los administradores del repositorio.
Acerca de la creación de informes privados de una vulnerabilidad de seguridad
A menudo, los investigadores de seguridad se sienten responsables de alertar a los usuarios de una vulnerabilidad que podría aprovecharse. Si no hay instrucciones claras sobre cómo ponerse en contacto con los mantenedores del repositorio que contienen la vulnerabilidad, es posible que los investigadores de seguridad no tengan otra opción, sino publicar sobre la vulnerabilidad en las redes sociales, enviar mensajes directos al mantenedor o incluso crear incidencias públicas. Esta situación puede dar lugar a una divulgación pública de los detalles de la vulnerabilidad.

Los informes de vulnerabilidades privados facilitan a los investigadores de seguridad notificar las vulnerabilidades directamente al mantenedor de repositorios mediante un formulario sencillo.

Para los investigadores de seguridad, las ventajas de usar informes de vulnerabilidades privados son:

Menos frustración y menos tiempo dedicado a tratar de averiguar cómo ponerse en contacto con el mantenedor.
Un proceso más sencillo para revelar y analizar los detalles de la vulnerabilidad.
La oportunidad de analizar los detalles de vulnerabilidades de forma privada con el mantenedor de repositorios.
Note

Si el repositorio no tiene habilitada la generación de informes privados de vulnerabilidades, debes iniciar el proceso de generación de informes siguiendo las instrucciones de la directiva de seguridad del repositorio o crear una incidencia que solicite a los mantenedores un contacto de seguridad preferido. Para obtener más información, vea «Acerca de la divulgación coordinada de las vulnerabilidades de seguridad».

Creación de informes privados de una vulnerabilidad de seguridad
Si el repositorio público tiene habilitada la notificación privada de vulnerabilidades, cualquiera puede notificar de manera privada una vulnerabilidad de seguridad a los mantenedores del repositorio. Los usuarios también pueden evaluar la seguridad general de un repositorio público y sugerir una directiva de seguridad. Para más información, consulta Evaluación de la configuración de seguridad de un repositorio.

En GitHub, navegue hasta la página principal del repositorio.

En el nombre del repositorio, haz clic en  Seguridad. Si no puedes ver la pestaña "Seguridad", selecciona el menú desplegable  y, a continuación, haz clic en Seguridad.

Captura de pantalla de un encabezado de repositorio en el que se muestran las pestañas. La pestaña "Seguridad" está resaltada con un contorno naranja oscuro.
Haz clic en Notificar una vulnerabilidad para abrir el formulario de asesoramiento.

Rellena el formulario de detalles de asesoramiento.

Tip

En este formato, solo el título y la descripción son obligatorios. (En el formulario de aviso de seguridad general, que inicia el mantenedor del repositorio, también se requiere especificar el ecosistema). Sin embargo, recomendamos que los investigadores de seguridad proporcionen toda la información posible en el formulario para que los mantenedores puedan tomar una decisión informada sobre el informe enviado. Puede adoptar la plantilla que usan nuestros investigadores de seguridad de GitHub Security Lab, que está disponible en el repositorio github/securitylab".

Para más información sobre los campos disponibles e instrucciones sobre cómo rellenar el formulario, consulta "Creación de un aviso de seguridad de repositorio" y "Procedimientos recomendados para escribir asesorías de seguridad del repositorio".

En la parte inferior del formulario, haz clic en Enviar informe. GitHub mostrará un mensaje que te indicará que se ha notificado a los mantenedores y que tienes un crédito pendiente para este aviso de seguridad.

Tip

Cuando se envía el informe, GitHub agrega automáticamente al informador de la vulnerabilidad como colaborador y como usuario acreditado en el aviso propuesto.

Opcionalmente, haz clic en Iniciar una bifurcación privada temporal si quieres empezar a corregir el problema. Debes tener en cuenta que solo el mantenedor del repositorio puede combinar los cambios de esa bifurcación privada en el repositorio primario.

Captura de pantalla de la parte inferior de un aviso de seguridad. Un botón, con la etiqueta "Iniciar una bifurcación temporal", está resaltado en naranja oscuro.
Los pasos siguientes dependen de la acción realizada por el mantenedor del repositorio. Para más información, consulta Administración de vulnerabilidades de seguridad notificadas de forma privada.
