# GitHub Copilot en GitHub.com

Explore los repositorios, planifique los cambios y delegue tareas de codificación a GitHub Copilot sin salir de GitHub.com.

GitHub Copilot en GitHub.com puede responder a preguntas sobre los repositorios, planificar y realizar cambios, revisar las solicitudes de incorporación de cambios y automatizar las tareas del repositorio. Puede hacer preguntas y delegar el trabajo desde el mismo cuadro de entrada o usar Copilot directamente en los flujos de trabajo de problemas y pull requests.

Para comparar dónde puede usar Copilot, consulte [Dónde usar GitHub Copilot](/es/copilot/get-started/where-to-use-github-copilot).

## Cómo Copilot ayuda en GitHub.com

Puede trabajar con Copilot de varias maneras:

- **El chat** le permite formular preguntas sobre los repositorios, comprender el código y explorar posibles soluciones.
- **Las experiencias agénticas** pueden investigar un repositorio, planear los cambios y completar tareas en varios pasos mediante la lectura de archivos, la edición de código y la ejecución de pruebas en un entorno de desarrollo en la nube.
- **La revisión del código** proporciona comentarios sobre las solicitudes de incorporación de cambios y sugiere correcciones.
- **Las automatizaciones** ejecutan tareas del repositorio según una programación o en respuesta a eventos, en lugar de requerir un mensaje nuevo cada vez.

Por ejemplo, puede usar chat para comprender cómo un repositorio gestiona la autenticación y, a continuación, pedir a un agente que planee y agregue pruebas que faltan. Una vez que los cambios se encuentren en una pull request, puede solicitar una revisión de Copilot. Para mantener la cobertura de pruebas a lo largo del tiempo, puede configurar una automatización para comprobar si faltan pruebas cada semana y proponer incorporaciones para que las revise.

## Experiencias de chat y basadas en agentes

En GitHub.com, puede pasar de hacer preguntas a delegar trabajo en la misma conversación.

### Formular preguntas

El chat puede explicar código desconocido, sugerir correcciones, generar pruebas o comparar enfoques. Las preguntas de seguimiento le permiten refinar la solicitud sin iniciar una nueva conversación.

El chat está preconfigurado con herramientas para tareas como la creación de ramas, la actualización de archivos y la creación o actualización de incidencias. También admite la búsqueda de código semántico.

### Delegar trabajo

Copilot cloud agent puede investigar un repositorio, planear los cambios e implementarlos en segundo plano. Puede editar archivos y ejecutar pruebas y linters en un entorno de desarrollo en la nube efímero, en lugar del IDE local. Consulte [GitHub Copilot en IDE](/es/copilot/concepts/copilot-surfaces/copilot-in-ides).

Puede iniciar el trabajo desde el panel de agentes, una conversación o una incidencia o un pull request en GitHub.com.

Desde campañas de seguridad, puede asignar alertas de análisis de código a Copilot para corregirlas. Consulte [Corrección de alertas de una campaña de seguridad](/es/code-security/how-tos/manage-security-alerts/remediate-alerts-at-scale/fixing-alerts-in-security-campaign#assigning-alerts-to-copilot-cloud-agent).

Al implementar cambios, Copilot se encarga de la creación de ramas, los mensajes de commit y el envío de cambios. Puede revisar los cambios y solicitar refinamientos antes de crear una solicitud de incorporación de cambios o solicitar una solicitud de incorporación de cambios en el mensaje inicial. También puede continuar con el trabajo usted mismo. Consulte [Investiga, planifica e itera sobre los cambios en el código con Copilot cloud agent](/es/copilot/how-tos/copilot-on-github/use-copilot-agents/research-plan-iterate).

### Contexto de sesión

En GitHub.com, Copilot Chat y Copilot cloud agent pueden compartir contexto. Al iniciar una sesión del agente desde un chat, la sesión incorpora el contexto de la conversación. Mientras se ejecuta la sesión, puede seguir conversando con Copilot sobre su progreso y dirigir el trabajo.

Copilot Chat también puede responder a preguntas sobre las solicitudes de incorporación de cambios creadas por Copilot consultando los registros de sesión del agente pertinentes. Puede preguntar qué ha cambiado, qué se validó y por qué, sin salir de la conversación.

Esta transferencia de contexto se limita a las sesiones Copilot Chat y cloud agent en las que está trabajando activamente. Es distinto de Copilot Memory, que construye una comprensión duradera de tus repositorios y preferencias a lo largo de distintas sesiones. Para obtener más información, vea [Acerca de la memoria de GitHub Copilot](/es/copilot/concepts/agents/copilot-memory).

En GitHub.com, los registros de sesión muestran el trabajo y las herramientas que se usan. Las sesiones compartidas y las solicitudes de extracción permiten que los compañeros de equipo con acceso al repositorio sigan el trabajo y revisen los cambios. Los registros no reemplazan su propia revisión y pruebas. Consulte [Gestión de sesiones del agente](/es/copilot/how-tos/copilot-on-github/use-copilot-agents/manage-and-track-agents).

### Sesiones entre dispositivos

Con el control remoto habilitado, puede supervisar y dirigir una sesión de GitHub Copilot CLI desde GitHub.com. Continúa ejecutándose en la máquina original, que debe permanecer en línea. Consulte [Control remoto de sesiones GitHub Copilot CLI](/es/copilot/concepts/agents/copilot-cli/about-remote-control).

En GitHub.com, puede consultar el historial de sesión sincronizado en todas las plataformas Copilot. Esto incluye las sesiones Copilot cloud agent y Copilot code review, y las sesiones de GitHub Copilot CLI, VS Code, JetBrains IDEs y la app de GitHub Copilot.

Solo puede consultar las sesiones que ha iniciado. La sincronización debe estar habilitada y permitida por las directivas de la organización. Consulte [Consultar sesiones anteriores](/es/copilot/how-tos/copilot-on-github/use-copilot-agents/manage-and-track-agents#query-past-sessions).

## Revisión de código

En GitHub.com, Copilot code review revisa los cambios de la pull request, identifica posibles problemas y sugiere correcciones. Usa capacidades agénticas para recopilar contexto del repositorio. Puede solicitar una revisión o configurar revisiones automáticas y, a continuación, revisar y aplicar los cambios sugeridos. Consulte [Revisión del código de GitHub Copilot](/es/copilot/concepts/agents/code-review).

Copilot también puede generar un resumen de los cambios directamente en una descripción o comentario de la pull request. Esto ayuda a los revisores a comprender los cambios, pero es independiente de revisar el código. Consulte [Creación de un resumen de solicitudes de incorporación de cambios con GitHub Copilot](/es/copilot/how-tos/copilot-on-github/copilot-for-github-tasks/create-a-pr-summary).

## Automatizaciones y flujos de trabajo agénticos

Las automatizaciones le permiten definir una tarea una vez y hacer que Copilot cloud agent la ejecute según una programación o en respuesta a los eventos del repositorio. Por ejemplo, una automatización puede evaluar los problemas entrantes o preparar notas de la versión semanales. Puede crear y administrar automatizaciones desde la pestaña **Agents** de un repositorio en GitHub.com. Las automatizaciones están disponibles en repositorios privados e internos que cumplan los requisitos. Consulte [Automatizaciones de Copilot](/es/copilot/concepts/agents/cloud-agent/about-automations).

GitHub Agentic Workflows proporciona otra manera de automatizar las tareas de los repositorios en GitHub.com. Define tareas en lenguaje natural en archivos markdown y se ejecutan como flujos de trabajo de GitHub Actions. Estos flujos de trabajo pueden usar Copilot u otro agente de codificación compatible. Consulte [Flujos de trabajo basados en agentes de GitHub](/es/copilot/concepts/agents/about-github-agentic-workflows).

## Personalizaciones

En GitHub.com, las instrucciones personalizadas le permiten guardar preferencias personales para chat, convenciones de repositorio e instrucciones de la organización.
Copilot Spaces organiza el contexto compartido para preguntas. Para el trabajo delegado, los custom agents, los prompts y las aptitudes del agente proporcionan instrucciones y recursos específicos de la tarea. Los servidores de Model Context Protocol (MCP) conectan agentes a herramientas y datos adicionales. Los hooks pueden ejecutar comandos durante el trabajo del agente para la validación o el registro. Para obtener instrucciones de configuración, consulte [Personalizar Copilot](/es/copilot/how-tos/copilot-on-github/customize-copilot).

## Modelos de IA

Puede cambiar el modelo que usa Copilot para generar respuestas. Es posible que otros modelos funcionen mejor o proporcionen respuestas más útiles, en función del tipo de preguntas que realices. Las opciones incluyen modelos premium con funcionalidades avanzadas. Para cambiar el modelo en el IDE, consulte [Cambio del modelo de IA para GitHub Copilot Chat](/es/copilot/how-tos/copilot-in-your-ide/chat-with-copilot/change-the-chat-model). Para cambiar o comparar modelos en GitHub, consulte [Hacer preguntas a GitHub Copilot en GitHub](/es/copilot/how-tos/copilot-on-github/chat-with-copilot/chat-in-github#changing-and-comparing-ai-models).

En GitHub.com, los modelos disponibles dependen de tu plan y las políticas de tu cuenta. Consulte [Modelos de IA admitidos en GitHub Copilot](/es/copilot/reference/ai-models/supported-models).

Para Copilot cloud agent, la capacidad de seleccionar un modelo también depende de cómo se inicie la tarea. Consulte [Cambio del modelo de IA para GitHub Copilot agente en la nube](/es/copilot/how-tos/use-copilot-agents/cloud-agent/changing-the-ai-model).

## Referencias al código público correspondiente

En las respuestas de chat y las sesiones del agente en GitHub.com, Copilot puede generar código que coincida con el código en repositorios públicos. Las referencias de código le ayudan a revisar el código coincidente y su información de licencia para que pueda decidir si desea usarlo, proporcionar atribución o quitarlo.

Las coincidencias aparecen en el contexto en el que está revisando la salida:

- **Respuestas de chat**: si usted o su organización permiten sugerencias que coincidan con el código público, el código coincidente en una respuesta incluye una referencia debajo de la sugerencia. La referencia identifica repositorios públicos que contienen código coincidente e información de licencias, si se encuentran.
- **Registros de sesión del agente**: cuando Copilot genera código que coincide durante una tarea delegada, los registros de sesión incluyen un vínculo a los detalles del código que coincide.

Las coincidencias se producen con poca frecuencia, por lo que la mayoría de las respuestas no contienen referencias de código. La búsqueda cubre un índice de repositorios públicos en GitHub.com, no repositorios privados ni código hospedado en otro lugar. El índice se actualiza periódicamente, por lo que puede omitir el código agregado recientemente o hacer referencia al código que se ha movido o eliminado.

Para obtener instrucciones sobre cómo ver las referencias, consulte [Encontrar código público que coincida con las sugerencias de GitHub Copilot](/es/copilot/how-tos/get-code-suggestions/find-matching-code?tool=webui).

## Acceso y disponibilidad

Las características disponibles dependen de tu plan y las directivas de tu organización. Para obtener instrucciones de configuración, consulte [Configuración de Copilot](/es/copilot/how-tos/copilot-on-github/set-up-copilot). Para ver las asignaciones de uso y los costos, consulte [GitHub Copilot: facturación y uso](/es/copilot/concepts/billing-and-usage).

Los propietarios y administradores de repositorios pueden deshabilitar Copilot cloud agent para determinados repositorios, incluso cuando el plan y las directivas le permiten usarlo. Consulte [Administración del acceso al agente en la nube de GitHub Copilot](/es/copilot/concepts/enterprise/cloud-agent-access).

## Limitaciones y compatibilidad

Tanto las experiencias de chat como las experiencias agénticas en GitHub.com pueden producir código incorrecto o poco óptimo, incluido código que contiene vulnerabilidades de seguridad. Revise y pruebe la salida antes de usarla en producción. Consulte [Tarjeta de aplicación: agentes de GitHub Copilot](/es/copilot/responsible-use/agents).

Para obtener información sobre las protecciones de seguridad integradas, consulte [Riesgos y mitigaciones para el agente en la nube de GitHub Copilot](/es/copilot/concepts/agents/cloud-agent/risks-and-mitigations).

### Trabajo agéntico

Copilot cloud agent tiene las siguientes limitaciones de flujo de trabajo:

- **Ámbito del repositorio**: Copilot solo puede realizar cambios en el repositorio especificado al iniciar una tarea. No puede realizar cambios en varios repositorios en una ejecución.
- **Acceso al contexto**: de forma predeterminada, el servidor MCP de GitHub solo proporciona acceso al contexto en el repositorio en el que está trabajando el agente, como incidencias y solicitudes de incorporación de cambios anteriores. Puede configurar acceso más amplio a través de la configuración de MCP del repositorio. Consulte [Configuración de servidores MCP para el repositorio](/es/copilot/how-tos/copilot-on-github/customize-copilot/configure-mcp-servers).
- **Ramas y solicitudes de extracción**: Copilot solo puede trabajar en una rama a la vez y puede abrir una solicitud de extracción por tarea.
- **Duración de la sesión**: cada sesión de Copilot cloud agent tiene un tiempo de ejecución máximo de 59 minutos. Este límite no se puede extender ni eludir. Si una tarea supera el límite, la sesión caduca por tiempo de espera y se detiene.

Divida las tareas complejas en tareas más pequeñas y específicas. Puede configurar un tiempo de espera más corto mediante el ajuste `timeout-minutes` en el archivo `copilot-setup-steps.yml`. Consulte [Configuración del entorno de desarrollo](/es/copilot/how-tos/copilot-on-github/customize-copilot/customize-cloud-agent/customize-the-agent-environment).

<a id="limitations-in-copilot-cloud-agents-compatibility-with-other-features"></a>

### Compatibilidad del repositorio

- **Reglas de repositorio**: si un conjunto de reglas o una regla de protección de rama no es compatible con Copilot cloud agent, se bloquea el acceso al agente. Por ejemplo, una regla que solo permite autores de confirmaciones específicos puede impedir que Copilot cree o actualice solicitudes de incorporación de cambios. Si la regla está configurada mediante conjuntos de reglas, los administradores del repositorio pueden agregar Copilot como actor de omisión para habilitar el acceso. Consulte [Creación de conjuntos de reglas de un repositorio](/es/repositories/configuring-branches-and-merges-in-your-repository/managing-rulesets/creating-rulesets-for-a-repository#granting-bypass-permissions-for-your-branch-or-tag-ruleset).
- **Hospedaje de repositorios**: Copilot cloud agent solo funciona con repositorios hospedados en GitHub. No puede funcionar en repositorios almacenados en otras plataformas de hospedaje de código.

## Lectura adicional

- [GitHub Copilot en GitHub](/es/copilot/how-tos/copilot-on-github)
- Guías prácticas de [agente en la nube de GitHub Copilot](/es/copilot/how-tos/use-copilot-agents/cloud-agent)
- [Recetario de GitHub Copilot](/es/copilot/tutorials/copilot-cookbook)
- Para delegar el trabajo desde herramientas como Microsoft Teams y Slack, consulte [integraciones de Copilot](/es/copilot/concepts/tools/about-copilot-integrations).
- Para conocer las métricas de organización y empresa sobre la creación, las fusiones y el tiempo hasta la fusión de las solicitudes de incorporación de cambios, consulte [Métricas de uso de GitHub Copilot](/es/copilot/concepts/billing-and-usage/copilot-usage-metrics/copilot-metrics).
