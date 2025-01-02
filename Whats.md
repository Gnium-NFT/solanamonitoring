Qué es Dependabot
Dependabot mantiene actualizadas las dependencias para lo cual te informa de cualquier vulnerabilidad de seguridad en ellas, y abre solicitudes de incorporación de cambios de forma automática para actualizar las dependencias a la siguiente versión segura disponible cuando se desencadena una alerta de Dependabot, o bien a la versión más reciente cuando se publica una versión.

El término "Dependabot" abarca las características siguientes:

Dependabot alerts: notificación que se muestra en la pestaña Security del repositorio y en el gráfico de dependencias de este. La alerta incluye un enlace al archivo afectado en el proyecto e información acerca de la versión arreglada.
Dependabot updates:
Dependabot security updates: actualizaciones desencadenadas para actualizar las dependencias a una versión segura cuando se desencadena una alerta.
Dependabot version updates: actualizaciones programadas para mantener actualizadas las dependencias con la versión más reciente.
Las solicitudes de incorporación de cambios que abre Dependabot pueden desencadenar flujos de trabajo que ejecutan acciones. Para más información, consulta Automatizar al Dependabot con las GitHub Actions.

De forma predeterminada:

Si habilita GitHub Actions en el repositorio, GitHub ejecuta Dependabot updates en GitHub Actions.

Si GitHub Actions no está habilitado para el repositorio, GitHub genera Dependabot alerts mediante la aplicación integrada Dependabot en GitHub.

Para más información, consulta Acerca de Dependabot en ejecutores de Acciones de GitHub.

Dependabot security updates puede corregir dependencias vulnerables en GitHub Actions. Cuando se habilitan las actualizaciones de seguridad, Dependabot generará automáticamente una solicitud de cambios para actualizar los datos vulnerables GitHub Actions usados en los flujos de trabajo a la versión con revisión mínima. Para más información, consulta Sobre las actualizaciones de seguridad de Dependabot.

Qué son las alertas de Dependabot
Dependabot alerts resalta los repositorios afectados por una vulnerabilidad recién detectada en función del gráfico de dependencias y GitHub Advisory Database, que contiene las versiones en listas de vulnerabilidades conocidas.

Dependabot realiza un examen para detectar las dependencias no seguras y envía Dependabot alerts cuando:
Se agrega un aviso nuevo a GitHub Advisory Database.
Cambia el gráfico de dependencias del repositorio.
Las Dependabot alerts se muestran en la pestaña Seguridad y en el gráfico de dependencias del repositorio. La alerta incluye un enlace al archivo afectado en el proyecto e información acerca de la versión arreglada.
Para más información, consulta Acerca de las alertas Dependabot.

Qué son las actualizaciones de Dependabot
Hay dos tipos de Dependabot updates: actualizaciones de seguridad y de versión de Dependabot. En los dos casos Dependabot genera solicitudes de incorporación de cambios automáticas para actualizar las dependencias, pero hay varias diferencias.

Dependabot security updates:

Desencadenada por una alerta de Dependabot
Actualizan las dependencias a la versión mínima que resuelve una vulnerabilidad conocida
Compatible con ecosistemas admitidos en el gráfico de dependencias
No requiere un archivo de configuración, pero puedes usar uno para invalidar el comportamiento predeterminado.
Dependabot version updates:

Requiere un archivo de configuración
Se ejecutan según una programación que configure
Actualizan las dependencias a la versión más reciente que coincida con la configuración
Compatible con un grupo diferente de ecosistemas
Para más información sobre Dependabot updates, consulta Sobre las actualizaciones de seguridad de Dependabot y Acerca de las actualizaciones a la versión del Dependabot.

Disponibilidad de características
Repositorios públicos:

Gráfico de dependencias: habilitado de forma predeterminada y no se puede deshabilitar.
Revisión de dependencias: habilitada de forma predeterminada y no se puede deshabilitar.
Dependabot alerts: no está habilitado de forma predeterminada. GitHub detecta las dependencias no seguras y muestra información en el gráfico de dependencias, pero no genera Dependabot alerts de forma predeterminada. Los propietarios de repositorios o los usuarios con acceso administrativo pueden habilitar las Dependabot alerts. También puede habilitar o deshabilitar las alertas de Dependabot para todos los repositorios que pertenecen a la cuenta de usuario u organización. Para más información, consulta Administración de la configuración de seguridad y análisis para la cuenta personal o Administrar la configuración de seguridad y análisis de su organización.
Repositorios privados:

Gráfico de dependencias: no está habilitado de forma predeterminada. Los administradores del repositorio pueden habilitar la característica. Para más información, consulta Explorar las dependencias de un repositorio.

Revisión de dependencias: disponible en los repositorios privados propiedad de las organizaciones que usan GitHub Enterprise Cloud y que tienen una licencia para GitHub Advanced Security. Para más información, vea la documentación de GitHub Enterprise Cloud.

Dependabot alerts: no está habilitado de forma predeterminada. Los propietarios de los repositorios privados o las personas con acceso administrativo puede habilitar las Dependabot alerts si habilitan la gráfica de dependencias y las Dependabot alerts para sus repositorios. También puede habilitar o deshabilitar las alertas de Dependabot para todos los repositorios que pertenecen a la cuenta de usuario u organización. Para más información, consulta Administración de la configuración de seguridad y análisis para la cuenta personal o Administrar la configuración de seguridad y análisis de su organización.

Cualquier tipo de repositorio:

Dependabot security updates: no está habilitado de forma predeterminada. Puedes habilitar las Dependabot security updates para cualquier repositorio que utilice Dependabot alerts y la gráfica de dependencias. Para obtener información sobre cómo habilitar las actualizaciones de seguridad, consulta Configuración de actualizaciones de seguridad de Dependabot.
Dependabot version updates: no está habilitado de forma predeterminada. Las personas con permisos de escritura en un repositorio pueden habilitar las Dependabot version updates. Para obtener información sobre cómo habilitar las actualizaciones de versión, consulta Configuración de las actualizaciones de versiones de Dependabot.
