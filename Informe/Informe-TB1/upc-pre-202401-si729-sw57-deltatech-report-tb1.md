---
title: "Universidad Peruana de Ciencias Aplicadas - Informe de Trabajo Final"
author: 
  - "Startup: DeltaTech"
  - "Producto: DiligenceTech"
  - "Profesor: Velasquez Nuñez, Angel"
  - "Integrantes:"
  - "Ortega Huaraca, Abel: U20201B380"
  - "Herrera Gonzalez, Luis: U202218227"
  - "Elsner De la Torre Ugarte, Julio: U202111654"
  - "Adrianzén Flores, Carlos: U202215705"
  - "Garayar Mori, Oscar: U202014115"
date: "2024"
subject: "Markdown"
keywords: [Markdown, Report]
subtitle: "Desarrollo de Aplicaciones Open Source - SW57"
lang: "es"
colorlinks: true
footer-left: "DeltaTech"
titlepage: true
titlepage-text-color: "FFFAFA"
titlepage-color: "DC143C"
titlepage-rule-height: 2
titlepage-rule-color: "FFFAFA"
book: true
classoption: oneside
code-block-font-size: \scriptsize
header-includes:
- |
  ```{=latex} 
  \usepackage{awesomebox}
  \usepackage{fontawesome5}
  \usepackage{tcolorbox}
 
  \newtcolorbox{info-box}{colback=cyan!5!white,arc=0pt,outer arc=0pt,colframe=cyan!60!black}
  \newtcolorbox{error-box}{colback=red!5!white,arc=0pt,outer arc=0pt,colframe=red!75!black}
  \newtcolorbox{norm-box}{colback=gray!5!white,arc=0pt,outer arc=0pt,colframe=gray!60!black}
  \newtcolorbox{warn-box}{colback=orange!5!white,arc=0pt,outer arc=0pt,colframe=orange!80!black}
  \newtcolorbox{attn-box}{colback=green!5!white,arc=0pt,outer arc=0pt,colframe=green!75!black}
  \newtcolorbox{code-box}{colback=pink!5!white,arc=0pt,outer arc=0pt,colframe=pink!80!black}
  \newtcolorbox{learn-box}{colback=blue!5!white,arc=0pt,outer arc=0pt,colframe=blue!40!black,title=\textbf{Objectives:}}
  \newtcolorbox{scenario-box}{colback=orange!5!white,arc=0pt,outer arc=0pt,colframe=orange!80!black,title=\textbf{Scenario:}}
  \newtcolorbox{outline-box}{colback=cyan!5!white,arc=0pt,outer arc=0pt,colframe=cyan!60!black,title=\textbf{Outline:}}
  \newtcolorbox{prereqs-box}{colback=red!5!white,arc=0pt,outer arc=0pt,colframe=red!60!black,title=\textbf{Prerequisites:}}
  \newtcolorbox{labtime-box}{colback=yellow!5!white,arc=0pt,outer arc=0pt,colframe=yellow!60!black,title=\textbf{Lab:}}

  ```
pandoc-latex-environment:
  tcolorbox: [box]
  info-box: [info]
  error-box: [error]
  norm-box: [norm]
  warn-box: [warn]
  attn-box: [attn]
  code-box: [code]
  learn-box: [learn]
  scenario-box: [scenario]
  outline-box: [outline]
  prereqs-box: [prereqs]
  labtime-box: [labtime]
  noteblock: [note]
  tipblock: [tip]
  warningblock: [warning]
  cautionblock: [caution]
  importantblock: [important]
---
**Registro de Versiones del Informe**

| Versión | Fecha | Autor | Descripción |
|---------|-------|-------|-------------|
|         |       |       |             |
|         |       |       |             |
|         |       |       |             |
|         |       |       |             |
|         |       |       |             |

**Project Report Collaboration Insights**

::: note
Para acceder al Github de la organización, haga click a la [URL](https://github.com/OpenSource-DeltaTech-SW57).
:::

**Student Outcome**

El curso contribuye al cumplimiento del Student Outcome ABET: *ABET-EAC - Student Outcome 3*

* **Criterio:** *Capacidad de comunicarse efectivamente con un rango de audiencias*.

En el siguiente cuadro se describe las acciones realizadas y enunciados de conclusiones por parte del grupo, que permiten sustentar el haber alcanzado el logro del *ABET-EAC - Student Outcome 3*.

# Capítulo I: Introducción

## *Startup Profile*

### Descripción de la Startup 

**DeltaTech: Automatizando la** ***Due Diligence*** **en Línea**

DeltaTech es una startup centrada en ofrecer soluciones innovadoras para el proceso de due diligence en línea. Nos especializamos en la automatización de una variedad de procesos, desde el análisis de datos financieros de empresas hasta la revisión de sus estados de cuenta, entre otras funciones críticas.
Nuestras plataformas tecnológicas están diseñadas para proporcionar una manera eficiente y precisa de llevar a cabo una debida diligencia exhaustiva durante transacciones comerciales, como la venta de empresas. En DeltaTech, nos comprometemos a simplificar y agilizar el proceso de evaluación, permitiendo a nuestros clientes tomar decisiones informadas con confianza.
Cada solución que desarrollamos está impulsada por la búsqueda constante de la excelencia en la eficiencia operativa y la precisión en el análisis de datos. En DeltaTech, estamos transformando la forma en que se aborda la due diligence en línea, llevando la automatización al centro de las transacciones comerciales del siglo XXI.

![DeltaTech Logo](src/img/cap1/deltatech-banner.png "DeltaTech Logo")

\newpage

**Misión**

* Nuestra misión en DeltaTech es proporcionar soluciones innovadoras y eficientes para el proceso de due diligence en línea, permitiendo a nuestros clientes realizar evaluaciones exhaustivas de manera rápida y precisa durante transacciones comerciales críticas, como la venta de empresas. Nos esforzamos por automatizar y simplificar el análisis de datos financieros, brindando a los inversores las herramientas necesarias para tomar decisiones informadas y estratégicas que impulsen el éxito en sus operaciones.

**Visión**

* Nuestra visión en DeltaTech es transformar la forma en que se realiza la debida diligencia, siendo líderes en el desarrollo de plataformas tecnológicas avanzadas que agilizan el análisis de información financiera. Nos comprometemos a ofrecer una experiencia de usuario excepcional a través de interfaces intuitivas y seguras, respaldadas por algoritmos avanzados y cifrado de datos de extremo a extremo. Buscamos ser reconocidos como socios confiables y fundamentales en el éxito de las transacciones comerciales, facilitando la toma de decisiones estratégicas para nuestros clientes en todo momento.

### Perfiles de integrantes del equipo

Nuestro equipo está conformado por individuos apasionados y comprometidos, cada uno aportando sus habilidades únicas para lograr nuestros objetivos de manera efectiva y colaborativa. Aquí se muestra a nuestros miebros clave:

![](src/img/Integrantes/Abel.png) 

![](src/img/Integrantes/Arturo.png) 

![](src/img/Integrantes/Julio.png) 

![](src/img/Integrantes/Luis.png) 

![](src/img/Integrantes/Oscar.png) 

## *Solution Profile*

En el cambiante mundo empresarial actual, la debida diligencia financiera se ha convertido en un pilar fundamental para asegurar transacciones comerciales seguras y exitosas. Sin embargo, el proceso tradicional de recolección y análisis de datos financieros de empresas puede ser lento, tedioso y propenso a errores. Esta realidad ha generado una necesidad urgente de encontrar soluciones innovadoras que permitan a los inversores realizar este crucial proceso de manera más eficiente y efectiva.
En este contexto, surge una nueva era de la debida diligencia financiera, donde la tecnología y la inteligencia se unen para ofrecer soluciones ágiles y precisas. La búsqueda de métodos más inteligentes para acceder y analizar datos financieros se ha convertido en una prioridad para los profesionales que buscan tomar decisiones informadas y estratégicas en sus inversiones.

![Recurso extraído de Canva](src/img/cap1/solutionp.png) 

### Antecedentes y problemática

::: info
***What***

* El proceso tradicional de due diligence se caracteriza por ser laborioso, costoso y propenso a errores.
* Los inversores y profesionales financieros revisan una gran cantidad de documentos financieros, legales y operativos en un tiempo limitado.
* Esto puede resultar en la contratación de servicios adicionales y gastos innecesarios.
:::

::: info
***Who***

* Inversores y profesionales financieros se ven afectados por la complejidad y la carga de trabajo del proceso tradicional de due diligence.
* Propietarios de empresas enfrentan el desafío de compartir información confidencial con inversores potenciales.
:::

::: info
***Where***

Esta problemática es común en transacciones comerciales y de inversión, donde la debida diligencia es crucial.
:::

::: info
***When***

La problemática surge en cada proceso de adquisición o inversión, donde la toma de decisiones debe realizarse en un tiempo limitado.
:::

::: info
***Why***

* La falta de acceso rápido y la preocupación por la seguridad de la información sensible de la empresa dificultan la toma de decisiones.
* Existe el riesgo de que los inversores utilicen los datos sensibles con otros fines, lo que genera incertidumbre y desconfianza.
:::

::: attn
***How***

* Para abordar estos desafíos, nuestra solución se basa en el desarrollo de una *web application*.
* Implementaremos algoritmos avanzados para agilizar el proceso de análisis de datos financieros.
* Diseñaremos una interfaz intuitiva que permita a los usuarios acceder y revisar información de manera rápida y segura.
* Incorporaremos un sistema de cifrado de datos de extremo a extremo para garantizar la seguridad y confidencialidad de la información.
* Realizaremos pruebas exhaustivas y ajustes continuos para asegurar el funcionamiento óptimo de la plataforma en todo momento.
:::

::: attn
***How Much***

* Los costos asociados con la implementación de nuestra solución de Diligence Tech dependerán del tamaño y las necesidades específicas de cada empresa.
* Ofreceremos planes de suscripción flexibles para adaptarse a diferentes presupuestos y volúmenes de trabajo.
* Los costos se basarán en un modelo de suscripción mensual o anual, con opciones de escalabilidad según las demandas del usuario.
* Adicionalmente, ofreceremos servicios de capacitación y soporte técnico para garantizar una adopción exitosa y continua de la plataforma.
:::

\newpage

### *Lean UX Process*

![Recurso extraído de Canva](src/img/cap1/leanux.png)

#### *Lean UX Problem Statements*

::: note
***Problem Statement 1***

* Nuestro contexto se enfoca en mejorar la eficiencia y precisión del análisis financiero para los contadores financieros durante el proceso de due diligence.

* Hemos identificado un problema crítico que afecta a los contadores financieros al realizar el análisis exhaustivo de los documentos financieros de las empresas. Actualmente, los contadores enfrentan dificultades significativas al obtener de manera oportuna y eficiente los documentos necesarios para llevar a cabo una diligencia debida completa. Esta falta de acceso rápido y efectivo a la información financiera puede resultar en retrasos en el proceso de análisis y en la toma de decisiones, impactando negativamente la eficiencia y precisión del trabajo del contador.

* ¿Cómo podemos mejorar el acceso y la obtención eficiente de los documentos financieros para los contadores durante el proceso de due diligence, con el fin de agilizar y mejorar la calidad de su trabajo?
:::

::: note
***Problem Statement 2***

* Nuestro enfoque se centra en proporcionar a los inversores una plataforma intuitiva y eficiente para la evaluación de oportunidades de inversión durante el proceso de due diligence.

* Los inversores se enfrentan a la dificultad de realizar un análisis exhaustivo y preciso de la salud financiera y los riesgos potenciales de las empresas objetivo. Actualmente, experimentan desafíos al acceder y comparar de manera eficiente la información financiera de múltiples empresas, lo que puede llevar a decisiones de inversión subóptimas o basadas en datos incompletos.

* ¿Cómo podemos proporcionar a los inversores una plataforma intuitiva y eficiente que les permita acceder, comparar y analizar de manera efectiva la información financiera de las empresas, con el objetivo de facilitar la toma de decisiones informadas y estratégicas?
:::

\newpage

#### *Lean UX Assumptions*

***Business Assumptions:***

1. **Creo que mis clientes necesitan** una herramienta eficiente y confiable para realizar sus análisis financieros exhaustivos durante el proceso de due diligence. 

2. **Estas necesidades se pueden resolver con** nuestra plataforma inteligente que automatice el análisis financiero y que ofrezca acceso rápido y seguro a información relevante de las empresas objetivo.

3. **Mis clientes iniciales son** inversores y contadores financieros que trabajan en sell-side.

4. **El valor #1 que un cliente quiere de mi servicio es** una manera eficiente y precisa de realizar sus transacciones durante el proceso de due diligence. 

5. **El cliente también puede obtener estos beneficios adicionales** como una mayor confianza en el proceso de due diligence, una mayor seguridad de los datos financieros y una experiencia de usuario mejorada.

6. **Voy a adquirir la mayoría de mis clientes a través de** campañas de marketing dirigidas a empresas de capital privado, fondos de inversión y otros actores clave en el mercado de transacciones

7. **Haré dinero a través de** la venta de suscripciones a nuestra plataforma "Diligence Tech", ofreciendo diferentes niveles de acceso según las necesidades del cliente.

8. **Mi competencia principal en el mercado serán** otras plataformas de due diligence en línea, así como servicios tradicionales de consultoría que ofrecen análisis de datos financieros.

9. **Los venceremos debido a** nuestra capacidad para ofrecer una solución tecnológica más rápida, precisa y fácil de usar que nuestras competidoras, así como nuestro enfoque en la seguridad de los datos y la experiencia del usuario..

10. **El mayor riesgo del producto es** que la tecnología pueda no funcionar como se espera, lo que podría resultar en errores en los datos o brechas de seguridad.

11. **Resolveremos esto a través de la** implementación de rigurosas pruebas de calidad y seguridad, así como la rápida corrección de errores a medida que surjan.

12. **¿Qué otras suposiciones tenemos? ¿Eso, si se prueba que es falso, causará que nuestro negocio/proyecto no funcione?** Otras suposiciones que tenemos son si:
    - Existe una demanda significativa.
    - La automatización de datos financieros mejorará el proceso de due diligence. 
    - Garantizar la seguridad y privacidad de los datos financieros de las empresas objetivo a través de cifrado de extremo a extremo generará confianza entre los usuarios

***Business Outcomes:***

- Aumentar la eficiencia operativa de las empresas al reducir el tiempo y los recursos necesarios para completar el proceso de due diligence.
- Proporcionar una plataforma segura, intuitiva y efectiva que aumente la satisfacción del cliente y promueva la retención a largo plazo.
- Ganar una ventaja competitiva al ofrecer características avanzadas, seguridad de datos y facilidad de uso que superan a los competidores.

\newpage

***Users Assumptions:***

***User Assumption - Problem Statement 1***

1. **¿Quién es el usuario?**

    Los usuarios son los contadores financieros que buscan agilizar su proceso de due diligence e inversores que contratan empresas financieras que buscan una visualización más accesible de los resultados.

2. **¿Qué problemas tiene nuestro producto? ¿Resolver?**

    * Dificultad para acceder y analizar rápidamente datos financieros de empresas objetivo durante el proceso de debida diligencia.
    * Riesgos asociados con la falta de seguridad y privacidad de los datos financieros sensibles.
    * Falta de eficiencia en el proceso de debida diligencia debido a la dependencia de métodos manuales y lentos.

3. **¿Qué características son importantes?**

    * Automatización del análisis de datos financieros.
    * Seguridad de datos con cifrado de extremo a extremo.
    * Interfaz de usuario intuitiva y fácil de usar.
    * Acceso rápido y seguro a información financiera relevante.
    * Funcionalidades avanzadas de visualización y generación de informes.

4. **¿Dónde encaja nuestro producto en su trabajo o vida?**

    Encaja en el proceso de trabajo de los usuarios al proporcionar una plataforma centralizada y eficiente para realizar análisis exhaustivos de datos financieros de empresas

5. **¿Cuándo y cómo es usado nuestro producto?**

    Es utilizado por los usuarios durante todo el proceso de debida diligencia, desde la evaluación inicial de una empresa objetivo hasta la finalización de la transacción comercial.

6. **¿Cómo debe verse nuestro producto y cómo comportarse?**

    Debe tener una apariencia profesional y moderna, con una interfaz de usuario limpia y organizada que facilite la navegación y el acceso a las herramientas y funciones clave. El producto debe comportarse de manera fluida y rápida, brindando respuestas instantáneas a las consultas de los usuarios y garantizando la seguridad y confiabilidad de los datos financieros manipulados.

\newpage

***User Assumption - Problem Statement 2***

1. **¿Quién es el usuario?**

    Los usuarios son inversores que buscan oportunidades de inversión y necesitan realizar una diligencia debida exhaustiva para evaluar la salud financiera y los riesgos potenciales de las empresas objetivo.

2. **¿Qué problemas tiene nuestro producto? ¿Resolver?**

    * Dificultad para acceder y comparar de manera eficiente la información financiera de múltiples empresas durante el proceso de due diligence.
    * Riesgos asociados con la toma de decisiones basadas en datos financieros incompletos o inexactos.
    * Falta de una plataforma centralizada y fácil de usar para analizar y evaluar oportunidades de inversión de manera efectiva.

3. **¿Qué características son importantes?**

    * Interfaz de usuario intuitiva y eficiente que permita una navegación fluida y acceso rápido a la información financiera clave.
    * Funcionalidades avanzadas de comparación y análisis de datos financieros para facilitar la toma de decisiones informadas.
    * Seguridad de datos avanzada para garantizar la confidencialidad y protección de la información financiera sensible.
    * Herramientas de visualización y generación de informes que permitan una comprensión clara y rápida de la salud financiera de las empresas objetivo.

4. **¿Dónde encaja nuestro producto en su trabajo o vida?**

    Nuestro producto encaja en el proceso de trabajo de los inversores al proporcionar una plataforma centralizada y completa para evaluar y comparar oportunidades de inversión durante el proceso de due diligence.

5. **¿Cuándo y cómo es usado nuestro producto?**

    * Es utilizado por los inversores desde el inicio del proceso de evaluación de una empresa objetivo hasta la toma final de decisiones de inversión.
    * Los inversores utilizan nuestro producto para analizar los estados financieros, realizar comparaciones entre empresas y evaluar los riesgos y oportunidades de inversión.

6. **¿Cómo debe verse nuestro producto y cómo comportarse?**

    * Nuestro producto debe tener una apariencia profesional y moderna, con una interfaz de usuario clara y organizada que facilite la comparación y análisis de datos.
    * Debe comportarse de manera eficiente y rápida, brindando resultados precisos y actualizados de manera oportuna.
    * La seguridad y confidencialidad de los datos financieros es fundamental, por lo que el producto debe garantizar un cifrado sólido y medidas de protección avanzadas.

***User outcomes:***

- Acceso de manera rápida y eficiente a la información financiera relevante de las empresas objetivo.
- Confianza en la seguridad y privacidad de los datos financieros sensibles
- Experiencia de usuario mejorada gracias a la interfaz intuitiva y fácil de usar

\newpage

***Feature Assumptions***

**Para el Problem statement 1:**

::: box 
* **Herramientas Avanzadas de Analisis Financiero:**

    Funciones especializadas para analizar estados financieros, ratios financieros, tendencias históricas y comparaciones sectoriales.

* **Automatización de Procesos Repetitivos:**

    Capacidad de automatizar tareas como la extracción de datos financieros, el cálculo de ratios y la generación de informes estándar.

* **Integración con Fuentes de Datos Externos:**

    Posibilidad de integrar datos de múltiples fuentes, como bases de datos financieras externas o sistemas de contabilidad.

* **Seguridad y Confidencialidad Reforzadas:**

    Funciones adicionales de seguridad, como permisos de acceso específicos, para garantizar la confidencialidad de la información financiera.

* **Visualización de Datos Interactiva:**

    Gráficos interactivos y tablas dinámicas para visualizar los datos financieros de manera clara y comprensible.
:::

\newpage

**Para el Problem Statement 2:**

::: box
* **Interfaz de Usuario Intuitiva:**
    - Los inversores podrán navegar fácilmente por la plataforma y acceder a las herramientas clave de análisis financiero.
    - Se asume que una interfaz limpia y organizada facilitará la comparación y evaluación de empresas.

* **Herramientas Avanzadas de Análisis:**
    - Los inversores podrán utilizar herramientas avanzadas para comparar rápidamente los datos financieros de múltiples empresas.
    - Se asume que características como gráficos interactivos, análisis comparativos y tablas dinámicas mejorarán la eficiencia del análisis.

* **Funcionalidades de Seguridad Avanzada:**
    - Los inversores confiarán en la plataforma debido a las medidas de seguridad avanzada, como cifrado de extremo a extremo y autenticación de dos factores.
    - Se asume que la seguridad sólida garantizará la protección de los datos financieros confidenciales.

* **Generación de Informes Personalizados:**
    - Los inversores podrán crear informes personalizados basados en sus criterios de evaluación y preferencias.
    - Se asume que los informes detallados y personalizados facilitarán la toma de decisiones informadas.

* **Alertas y Notificaciones Relevantes:**
    - Los inversores recibirán alertas sobre cambios significativos en los datos financieros de las empresas en su lista de seguimiento.
    - Se asume que las alertas oportunas y relevantes mejorarán la capacidad de reacción a los cambios en las empresas objetivo.
:::

\newpage

#### *Lean UX Hypothesis Statements*

***Hypothesis - Problem Statement 1***

::: tip
* **Creemos que** los contadores financieros valoran la eficiencia y precisión en el análisis de datos financieros durante el proceso de due diligence. **Sabremos que** esto es cierto **cuando** observemos una disminución significativa en el tiempo dedicado al análisis manual de datos, medido por una reducción del 30% en el tiempo promedio necesario para completar una diligencia debida.

* **Creemos que** la seguridad y privacidad de los datos financieros sensibles es una preocupación clave para los contadores financieros durante el proceso de due diligence. **Sabremos que** esto es cierto **cuando** veamos una mayor confianza en la plataforma "DiligenceTech" por parte de los contadores, medido por una reducción del 20% en las solicitudes de soporte relacionadas con la seguridad de los datos.
:::

***Hypothesis - Problem Statement 2***

::: tip
* **Creemos que** los inversores valoran la facilidad y rapidez de acceso a información financiera relevante durante el proceso de due diligence. **Sabremos que** esto es cierto **cuando** observemos un aumento en la eficiencia y precisión en la toma de decisiones de inversión, medida a través de una reducción del tiempo dedicado a la investigación y una mayor satisfacción del usuario.

* **Creemos que** la seguridad y privacidad de los datos financieros sensibles es una preocupación clave para los inversores durante el proceso de due diligence. **Sabremos que** esto es cierto **cuando** veamos un aumento en la confianza de los inversores en la plataforma, medido por una mayor adopción de "DeltaTech" y retroalimentación positiva sobre las medidas de seguridad implementadas.
:::

\newpage

#### *Lean UX Canvas*

![Artefacto creado en Figma ([URL](https://www.figma.com/file/jX7TR5fsEkgbQVH44vAmDb/Lean-UX-Canvas-2.0?type=design&node-id=0%3A1&mode=design&t=uRI0WHIdDhIsWi2g-1))](src/img/cap1/Lean-UX-Canvas.png) 

## Segmentos objetivo

![Tabla del segmento 1](src/img/cap1/segmento-1.png) 

![Tabla del segmento 2](src/img/cap1/segmento-2.png) 

# Capítulo II: *Requirements Elicitation & Analysis*

## Competidores

1. **Datasite Diligence:** El virtual data room más utilizado en el mercado. Proporcionada por la empresa Datasite, esta solución mediante aplicación web brinda un espacio de almacenamiento y edición de archivos, los cuales se esperan que sean documentos financieros para posteriormente ser enviados por correo electrónico a quien sea desee el usuario. Entre las mecánicas más resaltantes en este competidor está la posibilidad de censura mediante IA elementos de los documentos y la modalidad Q&A. Su precio es a base de páginas que contengan los archivos, aproximadamente cuesta mil dolares anualmente.

    ![Datasite Diligence](src/img/cap2/DatasiteDiligence.svg)

    Segmentos Objetivos:

    * Agente Sell-Side (contadores financieros) de una empresa en busca de una herramienta ordenada para el proceso de Due Diligence.

    * Agente Buy-Side (asociados de auditoria) de una empresa que desea visualizar el proceso de Due Diligence de una forma asequible.

2. **iDeals:** Virtual data room online para servicios financieros, Biotech, IT y otras especializaciones del sistema que utilizan organizaciones de muchos usuarios dentro de la aplicación, la simplificación del ingreso y uso de archivos, y la seguridad del sistema en cuidarlos. Cuenta actualmente con más de 1 millón de usuarios y destaca en el mercado por su atención al cliente rápida y constante.

    ![iDeals](src/img/cap2/iDeals.svg)

    Segmentos Objetivos:

    * Agente Sell-Side (contadores financieros) de una empresa en busca de una herramienta ordenada para el proceso de Due Diligence.

    * Agente Buy-Side (asociados de auditoria) de una empresa que desea visualizar el proceso de Due Diligence de una forma asequible.

3. **Firmex:** Virtual data room para contadores financieros que permite insertar y guardar archivos al sistema con funcionalidades como Q&A y censura. Reconocido en el mercado por la seguridad que mantiene en los archivos.

    ![Firmex](src/img/cap2/Firmex.svg)

    Segmentos Objetivos:

    * Agente Sell-Side (contadores financieros) de una empresa en busca de una herramienta ordenada para el proceso de Due Diligence.

    * Agente Buy-Side (asociados de auditoria) de una empresa que desea visualizar el proceso de Due Diligence de una forma asequible.

### Análisis competitivo

xd

## Estrategias y tácticas frente a competidores

Según Michael Porter, la estrategia competitiva implica cómo una empresa compite en su mercado específico. Porter identificó tres estrategias generales que las empresas pueden emplear para competir con éxito: liderazgo en costos, diferenciación y enfoque. La estrategia de liderazgo en costos implica ofrecer productos o servicios a precios más bajos que los de los competidores, mientras que la diferenciación se basa en ofrecer productos y servicios únicos y distintivos. Por otro lado, una estrategia de enfoque se centra en un segmento de mercado específico. Para llevar a cabo eficazmente estas estrategias, las empresas necesitan tener un profundo conocimiento de sus mercados y competidores para desarrollar y mantener una ventaja competitiva sostenible a largo plazo.

Teniendo en cuenta el análisis FODA previamente presentado para DiligenceTech, proponemos las siguientes estrategias competitivas:

**Estrategias Competitivas para DiligenceTech:**

1. Liderazgo en Costos:

    Estrategia:

    DiligenceTech puede buscar optimizar sus procesos internos para reducir costos operativos y ofrecer sus servicios a precios más competitivos que los de sus competidores.

    Tácticas:

    - Implementar tecnologías eficientes que reduzcan los gastos de infraestructura y operativos.

    - Negociar acuerdos favorables con proveedores y socios para obtener mejores precios en servicios y herramientas necesarios.

    - Ofrecer modelos de precios flexibles y descuentos por volumen para atraer a clientes sensibles al costo.

2) Diferenciación a través de la Innovación:

    Estrategia:
    
    DiligenceTech puede enfocarse en desarrollar características y funcionalidades únicas que destaquen su plataforma como líder en innovación en la debida diligencia.

    Tácticas:

    - Realizar investigaciones de mercado para identificar necesidades no cubiertas y oportunidades de mejora.

    - Invertir en I+D para desarrollar herramientas avanzadas de análisis financiero y presentación de informes.

    - Promocionar activamente las nuevas características a través de campañas de marketing destacando la vanguardia tecnológica de DiligenceTech.

3) Enfoque en Segmentos Específicos del Mercado:

    Estrategia:
    
    DiligenceTech puede especializarse en atender a segmentos específicos del mercado donde pueda ofrecer un valor diferenciado y adaptado.

    Tácticas:

    - Identificar sectores de la industria con necesidades únicas de debida diligencia, como startups en crecimiento, empresas de tecnología emergente, o industrias reguladas.

    - Desarrollar soluciones personalizadas y paquetes de servicios adaptados a las necesidades específicas de cada segmento.

    - Colaborar con asociaciones y grupos de la industria para fortalecer la presencia en estos segmentos y generar confianza.

**Tácticas Específicas para DiligenceTech:**
1) Monitoreo Competitivo Continuo:

    Táctica:

    Realizar análisis periódicos de las estrategias, precios y ofertas de la competencia para identificar oportunidades y amenazas.

    Acciones:

    - Mantenerse al tanto de los movimientos de los competidores en cuanto a lanzamientos de productos, cambios de precios y campañas de marketing.

    - Utilizar herramientas de seguimiento de competidores y análisis de mercado para obtener información valiosa.

2) Estrategias de Precios y Paquetes Competitivos:
    Táctica:
    
    Ajustar estratégicamente los precios y paquetes de servicios para competir de manera efectiva en el mercado.

    Acciones:

    - Realizar análisis de precios comparativos y ajustar los precios de acuerdo con el valor percibido por los clientes.

    - Ofrecer paquetes personalizados que se ajusten a las necesidades específicas de diferentes tipos de clientes, como empresas grandes, medianas y startups.

3) Inversión en Marketing Diferenciado:

    Táctica:
    
    Desarrollar mensajes y campañas de marketing que resalten las fortalezas únicas y la propuesta de valor de DiligenceTech.

    Acciones:

    - Crear contenido educativo y de valor que demuestre cómo DiligenceTech aborda los desafíos específicos de la debida diligencia.

    - Utilizar estudios de casos y testimonios de clientes para respaldar los beneficios y resultados de la plataforma.

4) Alianzas Estratégicas y Colaboraciones:

    Táctica:
    
    Establecer asociaciones estratégicas con empresas complementarias o instituciones que puedan ampliar el alcance y la oferta de DiligenceTech.

    Acciones:

    - Colaborar con firmas de consultoría reconocidas para ofrecer servicios combinados de asesoramiento y tecnología.

    - Formar alianzas con organizaciones financieras o legales para ofrecer paquetes completos de servicios de debida diligencia.

## Entrevistas

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### Diseño de entrevistas

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### Registro de entrevistas

**Segmento 1: Contadores financieros trabajando en sell-side en empresas financieras con la necesidad de agilizar el proceso de análisis de debida diligencia**

1. Guisella Bravo

| Nombre               | Guisella Bravo                                                                     |
|----------------------|------------------------------------------------------------------------------------|
| Edad                 | 51 años                                                                            |
| Ubicación Geográfica | Lima, Perú                                                                         |
| Profesión            | Contadora pública colegiada (por más de 25 años)                                   |
| Link Entrevista      | https://drive.google.com/file/d/1olTTIzwfcLowupWzGqNCtpvncZuFWxy-/view?usp=sharing |

    Resumen Entrevista: Guisella Bravo es contadora pública colegiada, esto quiere decir que trabaja en ámbitos financieros usualmente de una empresa, y lleva ejerciendo esta profesión por más de 25 años. Tiene experiencia con Due Diligence como participante Sell-side y Buy-side en su antiguo trabajo, y ha utilizado Dropbox y Excel como herramientas virtuales para rendir esta labor. Su conocimiento tecnológico se limita a la utilización de estas herramientas como otras empresariales como el correo electrónico. En su opinión, la propuesta de solución que hemos planteado es “muy buena” porque las alternativas comúnmente utilizadas en el Perú no se especializan en la interacción entre la empresa compradora y vendedora. En cuanto a como se hace un Due Diligence mencionó que se divide en 3 etapas: Entrega de Requerimientos de la Información, Due Diligence y el Informe Final. Los actores son en la primera etapa el agente de la empresa compradora que lo envía al agente de la empresa vendedora, Due Diligence es el proceso de entregar documentos confidenciales solicitados (.pdf y .xlsx por mayoría) a la empresa compradora mediante la separación general de estas en áreas de especialidad específicas como el área financiera, laboral, legal y tributario, que son las más comunes, y una separación particular en Ítems de Información, los cuales son una descripción completa de los documentos deseados. Esta etapa tiene como proceso intermedio el sistema de Q&A (Preguntas y Respuestas) donde, conforme se van entregando los documentos, la empresa compradora tiene la oportunidad de ordenar explicaciones a la empresa vendedora de lo que se entrega, y lo hace el agente de la empresa vendedora. Due Diligence termina si ambas partes confirman que cada ítem está completo. Finalmente, la empresa compradora hace un informe final con los datos entregados de la empresa vendedora. En cuanto a funcionalidades, piensa que el hecho de evitar la descarga de los archivos es innecesario, porque el punto de Due Diligence es entregar información confidencial a otra empresa, y opina lo mismo de la funcionalidad de censura en los documentos. Le parece que un análisis financiero hecho dentro del sistema puede ser novedoso y útil, especialmente porque son demasiados documentos. Finalmente, menciona que la herramienta de obtener información de la internet es muy útil y sería de demasiada ayuda en la recolección de documentos. En cuanto a opiniones de Due Diligence de carácter emocional, ella cree que no existe parte tediosa del proceso, porque demora aproximadamente un mes a un mes y medio. Adicionalmente, le interesa mucho la seguridad de estos documentos (que no se le envíe a una persona equivocada) y que existan herramientas hechas específicamente para el entorno, le gusta la eficiencia. Para concluir, también menciona que en cuanto a problemas en Due Diligence es importante resaltar que elegir a una empresa con intenciones maliciosas para entregar los documentos es un error que le ha pasado y provocó la creación de un competidor de su empresa. Lo cual es más un problema de la misma empresa que seleccionó a quien entregarle la información. No obstante, nos da un buen argumento en contra de nuestra posible funcionalidad de que se presente una red social que funcione como website previo a realizar un Due Diligence, donde un inversor encuentra a una empresa acreditada y publicada en nuestra plataforma para posteriormente iniciar un Due Diligence en nuestra aplicación de Due Diligence si ambas partes están de acuerdo en inicializarla.

2. James De La Torre Ugarte

| Nombre               | James De La Torre Ugarte                                                              |
|----------------------|---------------------------------------------------------------------------------------|
| Edad                 | 55 años                                                                               |
| Ubicación Geográfica | Lima, Perú                                                                            |
| Profesión            | Contador público (por más de 37 años)                                                 |
| Link Entrevista      | https://drive.google.com/file/d/1pVBgF5Mg19oACeViPekwY-lZtho5sloD/view?usp=drive_link |

    Resumen Entrevista: James De La Torre Ugarte, un respetado contador público con una sólida trayectoria en due diligence opina de manera favorable a nuestro diseño que consistirá en una plataforma innovadora en la nube. Esta plataforma estaría diseñada específicamente para recibir documentos empresariales relevantes, como estados financieros y otros documentos relacionados, con el objetivo de facilitar el proceso de evaluación de empresas.  La propuesta sugiere que esta plataforma no solo sirva como un repositorio seguro para los documentos financieros, sino que también permita la aplicación de diversos ratios financieros los cuales van a ser de ayuda para poder determinar si es rentable o beneficioso a largo plazo para el inversionista. Esto proporciona a James la capacidad de realizar análisis detallados y personalizados de la salud financiera de las empresas en consideración, lo cual es fundamental en su rol de due diligence.  Considerando la sensibilidad y la importancia de la información financiera en el proceso de evaluación empresarial, se enfatiza la necesidad de que esta plataforma garantice altos estándares de seguridad. James comprende plenamente la importancia de proteger la confidencialidad y la integridad de los datos financieros de las empresas, por lo que sería fundamental que la plataforma implemente medidas de seguridad robustas y cumpla con las regulaciones pertinentes.  Además, se destaca la relevancia de que esta plataforma sea intuitiva y fácil de usar, especialmente considerando la diversidad de usuarios que podrían interactuar con ella. Dado el enfoque meticuloso y analítico que caracteriza el trabajo de James, la plataforma debería ofrecer una interfaz fluida que facilite la navegación y la extracción de datos necesarios para sus evaluaciones además del uso de métricas para la evaluación de los datos como (ROE, RAE, ROI, indices de liquidez de solvencia , ratios de liquidez , ratios de solvencia).

3. Patricia González

| Nombre               | Patricia González                                                                  |
|----------------------|------------------------------------------------------------------------------------|
| Edad                 | 58 años                                                                            |
| Ubicación Geográfica | Lima, Perú / Trujillo, Perú                                                        |
| Profesión            | Contadora pública colegiada (por más de 27 años)                                   |
| Link Entrevista      | https://drive.google.com/file/d/1gDNFYf4BYT09A8H1RkDDuDOOCKjXwre1/view?usp=sharing |

    Resumen Entrevista: Patricia González es contadora pública colegiada, lo cual significa que se dedica a ámbitos financieros de, en su caso, una empresa, que ejerce esta profesión por más de 27 años. Tiene experiencia con el proceso de Due Diligence como participante Sell-side en labores pasadas para una empresa trujillana. En su opinión, la propuesta de solución tiene mucho mercado interesado y mucho alcance también. Para ella el proceso de Due Diligence se divide en 3 etapas: Obtención de Información de Requerimientos, Due Diligence e Informe Final. El Due Diligence son Ítems de Información divido en áreas de especialización que suele restringirse a Laboral, Legal, Financiera y Tributaria. Cada Ítem es un contenedor de documentos y se reconocen por número. Cada ítem tiene como atributo el requerimiento completa y formalmente escrito. El proceso de Due Diligence no le parece tedioso. Opina que una herramienta para censura es una buena idea para segmentos como el RUC y razones sociales en documentos financieros. Cree que el análisis financiero puede ser apoyado por la misma solución y ayudaría mucho. Es favorable su opinión en cuanto a la agregación de la funcionalidad de recolección de documentos en páginas públicas específicas y acreditadas.

**Segmento 2: Inversores que contratan empresas financieras para servicios sell-side que buscan una visualización más accesible de los resultados**

### Análisis de entrevistas

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Needfinding*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *User Personas*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *User Task Matrix*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *User Journey Mapping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Empathy Mapping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *As-is Scenario Mapping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Ubiquitous Language*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Capítulo III: *Requirements Specification*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *To-Be Scenario Mapping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *User Stories*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Impact Mapping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Product Backlog*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Capítulo IV: *Product Design*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Style Guidelines*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *General Style Guidelines*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Web Style Guidelines*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Information Architecture*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Organization Systems*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Labeling Systems*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *SEO Tags and Meta Tags*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Searching Systems*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Navigation Systems*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Landing Page UI Design*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Landing Page Wireframe*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Landing Page Mock-up*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Web Applications UX/UI Design*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Web Applications Wireframes*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Web Applications Wireflow Diagrams*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Web Applications Mock-ups*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Web Applications User Flow Diagrams*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Web Applications Prototyping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Domain-Driven Software Architecture*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Software Architecture Context Diagram*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Software Architecture Container Diagrams*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Software Architecture Components Diagrams*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Software Object-Oriented Design*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Class Diagrams*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Class Dictionary*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Database Design*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Database Diagram*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Capítulo V: *Product Implementation, Validation & Deployment*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Software Configuration Management*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Software Development Environment Configuration*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Source Code Management*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Source Code Style Guide & Conventions*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Software Deployment Configuration*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Landing Page, Services & Applications Implementation*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### *Sprint n*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Sprint Planning n*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Sprint Backlog n*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Development Evidence for Sprint Review*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Testing Suite Evidence for Sprint Review*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Execution Evidence for Sprint Review*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Services Documentation Evidence for Sprint Review*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Software Deployment Evidence for Sprint Review*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

#### *Team Collaboration Insights during Sprint*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Conclusiones

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Conclusiones y recomendaciones

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Video *About-the-Team*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

# Bibliografía

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.
