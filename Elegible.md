Establecimiento de la configuración predeterminada para el examen de código a gran escala
Puedes configurar rápidamente el code scanning para los repositorios de toda la organización usando la configuración predeterminada.

¿Quién puede utilizar esta característica?
Propietarios de la organización, administradores de seguridad y miembros de la organización con el rol de administrador

Code scanning está disponible para los siguientes tipos de repositorios:

Repositorios públicos en GitHub.com
Repositorios propiedad de la organización en GitHub Enterprise Cloud con GitHub Advanced Security habilitado
En este artículo
Acerca del establecimiento de la configuración predeterminada a gran escala
Establecimiento de la configuración predeterminada para todos los repositorios aptos de una organización
Acerca del establecimiento de la configuración predeterminada a gran escala
La configuración predeterminada para el code scanning permite proteger rápidamente el código de los repositorios de toda la organización.

Puedes habilitar code scanning para todos los repositorios aptos en tu organización para la configuración predeterminada. Después de habilitar la configuración predeterminada, el código escrito en lenguajes compatibles con CodeQL en repositorios de la organización se analizará:

En cada envío de cambios a la rama predeterminada del repositorio o cualquier rama protegida. Para más información sobre las ramas protegidas, consulta Acerca de las ramas protegidas.
Al crear o confirmar una solicitud de cambios basado en la rama por defecto del repositorio, o cualquier rama protegida, excluyendo pull requests de forks.
Según una programación semanal.
Para obtener más información, consulta Establecimiento de la configuración predeterminada para todos los repositorios aptos de una organización.

También puedes crear configuraciones predeterminadas diferentes para repositorios individuales. Para obtener más información sobre cómo establecer la configuración predeterminada a nivel de repositorio, consulta Establecimiento de la configuración predeterminada para el examen del código.

En el caso de los repositorios que no son aptos para la configuración predeterminada, puedes establecer la configuración avanzada a nivel de repositorio o a nivel de la organización con un script. Para más información, consulta Establecimiento de la configuración avanzada para el examen de código con CodeQL a gran escala.


Repositorios aptos para la configuración predeterminada de CodeQL a gran escala
Un repositorio debe cumplir todos los criterios siguientes para ser aptos para la configuración predeterminada; de lo contrario, debes usar la configuración avanzada.

Code scanning aún no está habilitada.
GitHub Actions se han habilitado.
Visible públicamente.
Se recomienda habilitar la configuración predeterminada para repositorios aptos si hay alguna posibilidad de que los repositorios incluyan al menos un lenguaje compatible con CodeQL en el futuro. Si habilitas la configuración predeterminada en un repositorio que no incluya ningún lenguaje compatible con CodeQL, la configuración predeterminada no ejecutará ningún análisis ni usará ningún minuto de GitHub Actions. Si se agregan al repositorio lenguajes compatibles con CodeQL, la configuración predeterminada comenzará automáticamente a analizar los lenguajes compatibles con CodeQL y a usar minutos de GitHub Actions. Para más Información sobre los lenguajes compatibles con CodeQL, consulta "Acerca del examen de código con CodeQL".

Acerca de la adición de lenguajes a una configuración predeterminada
Si el código de un repositorio cambia para incluir un lenguaje admitido por CodeQL, GitHub actualizará automáticamente la configuración de code scanning para incluir el nuevo lenguaje. Si el code scanning da error con la nueva configuración, GitHub reanuda automáticamente la configuración anterior para que el repositorio no pierda la cobertura de code scanning.

Establecimiento de la configuración predeterminada para todos los repositorios aptos de una organización
Puedes habilitar la configuración predeterminada para todos los repositorios aptos de tu organización. Para más información, consulta Habilitación de características de seguridad a gran escala.

Extensión de la cobertura de CodeQL en la configuración predeterminada
En la página de configuración de seguridad de la organización, puedes extender la cobertura en la configuración predeterminada utilizando paquetes de modelos para todos los repositorios aptos de la organización. P
