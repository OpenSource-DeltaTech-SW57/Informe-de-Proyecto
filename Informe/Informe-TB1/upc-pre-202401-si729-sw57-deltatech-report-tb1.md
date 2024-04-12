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

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### Análisis competitivo

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Estrategias y tácticas frente a competidores

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## Entrevistas

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### Diseño de entrevistas

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

### Registro de entrevistas

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

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

EP01 (Gestión de Cuentas de Usuario): Como usuario, quiero registrarme, iniciar sesión y mantener control sobre mi cuenta para acceder de manera segura a la aplicación y gestionar mis datos personales.	

|  |  |
|---|---|
| US01 | Registro de   inversor  |
| US02 | Confirmación   de creación de cuenta |
| US03 | Verificación   de cuenta  |
| US04 | Registro   de empresa |
| US05 | Verificación   de cuenta empresa |
| US06 | Recuperación   de cuenta  |

EP02 (Gestión de Empresas y Solicitudes): Como usuario, quiero poder gestionar empresas y solicitudes, desde su registro hasta su cierre, para realizar procesos de due diligence de manera efectiva y eficiente.	

|  |  |
|---|---|
| US07 | Visualización   de empresas |
| US08 | Filtro   de empresas |
| US09 | Ordenamiento   de empresas |
| US10 | Interfaz   de búsqueda sencilla |
| US11 | Visualización   de solicitudes |
| US12 | Filtro   de solicitudes |
| US13 | Ordenamiento   de solicitudes |
| US14 | Admición   de solicitudes |
| US15 | Creación   de la solicitud |
| US16 | Consulta   de orden de solicitud |
| US17 | Actualizaciones   sobre la solicitud |
| US18 | Respuesta   de solicitud |
| US19 | Razón   de la respuesta otorgada |
| US20 | Creación   de queja |
| US22 | Cierre   de solicitud |

EP03 (Seguridad y Confidencialidad): Como usuario, quiero que mis datos y la información de las empresas sean seguros y confidenciales, evitando fugas de seguridad y limitando el acceso no autorizado, para proteger la integridad de la información.	

|  |  |
|---|---|
| US23 | Seguridad de   entrega |
| US24 | Limitación   al entregar datos |
| US25 | Alertas   de fugas de seguridad |

EP04 (Análisis Financiero): Como usuario, quiero realizar análisis financieros con los datos recibidos para evaluar adecuadamente las empresas y tomar decisiones informadas sobre mis inversiones.	

|  |  |
|---|---|
| US26 | Visualización   de análisis financieros disponibles |
| US27 | Eficacia   de los algoritmos de análisis financiero |
| US28 | conclusión   del análisis financiero |
| US21 | Visualización   de datos recibidos |

EP05 (Optimización de la API): Como desarrollador, quiero implementar funcionalidades de paginación y filtrado en los endpoints de la API para mejorar la eficiencia en la entrega de recursos y optimizar el rendimiento del sistema.	

|  |  |
|---|---|
| US29 | RESTful API   Registro de usuario |
| US30 | RESTful   API Inicio de sesión de usuario |
| US31 | Autenticación   basada en token JWT |
| US32 | Recuperación   de contraseña |
| US33 | CRUD   para recursos principales |
| US34 | Paginación   y filtrado de resultados |

EP06 (Landing Page Optimizada): Como usuario interesado, deseo una landing page intuitiva y optimizada que proporcione información clara y accesible sobre la aplicación, para facilitar la toma de decisiones informadas y la interacción con el equipo de la aplicación.	

|  |  |
|---|---|
| US35 | Descubrimiento   intuitivo |
| US36 | Contenido   informativo |
| US37 | Compatibilidad   móvil |
| US38 | Formulario   de contacto |
| US39 | Contenido   multimedia |
| US40 | Call-to-action   claro |
| US41 | Optimización   para SEO |


|     Epic / Story ID     |     Título     |     Descripción     |     Criterios de Aceptación     |     Relacionado con (Epic ID)    |
|---|---|---|---|---|
|     US01    |     Registro de     inversor     |     Como usuario inversionista, quisiera crear una   cuenta con el uso de mi correo electrónico     para representarme en la aplicación.    |      <br><br>Escenario 1: "Registro exitoso"                 Dado que un usuario inversionista desea crear una   cuenta,           cuando ingresa su dirección de correo electrónico   y una contraseña válida,           entonces el sistema registra con éxito su cuenta   y lo redirige a la página de inicio.                  <br><br>Escenario 2: "Correo electrónico   inválido"                 Dado que un usuario inversionista desea crear una   cuenta,           cuando ingresa una dirección de correo   electrónico inválida o incorrecta,           entonces el sistema muestra un mensaje de error   indicando que la dirección de correo electrónico es inválida.            <br><br>Escenario 3: "Correo electrónico   duplicado"           Dado que un usuario inversionista desea crear una   cuenta,           Cuando ingresa una dirección de correo   electrónico que ya está asociada con otra cuenta existente en el sistema,           Entonces el sistema muestra un mensaje de error   indicando que la dirección de correo electrónico ya está en uso y solicita al   usuario que ingrese una dirección de correo electrónico diferente.    |     EP01    |
|     US02    |     Confirmación de     creación de cuenta    |     Como usuario inversionista, quisiera recibir una   confirmación de la creación de mi cuenta a través del correo electrónico que proporcionó   para confirmar la creación de la cuenta.    |      <br><br>Escenario 1: "Correo de confirmación   enviado"           Dado que un usuario inversionista ha creado una   cuenta exitosamente,           Cuando proporciona una dirección de correo   electrónico válida durante el registro,           Entonces el sistema envía un correo electrónico   de confirmación a la dirección proporcionada.                  <br><br>Escenario 2: "Confirmación de cuenta"           Dado que un usuario inversionista ha creado una   cuenta exitosamente,           Cuando abre el correo electrónico de confirmación   enviado por el sistema,           Entonces el sistema incluye un enlace o código de   confirmación que el usuario puede utilizar para verificar su cuenta.                  <br><br>Escenario 3: "Error al enviar correo de   confirmación"           Dado que un usuario inversionista ha creado una   cuenta exitosamente,           Cuando el sistema intenta enviar el correo   electrónico de confirmación a la dirección proporcionada, pero falla debido a   un error del servidor de correo u otros problemas técnicos,           Entonces el sistema muestra un mensaje de error   indicando que no se pudo enviar el correo de confirmación y sugiere al   usuario que verifique su dirección de correo electrónico y vuelva a   intentarlo más tarde.            <br><br>Escenario 4: "Correo electrónico inválido   para confirmación"                 Dado que un usuario inversionista ha creado una   cuenta exitosamente,           Cuando el sistema detecta que la dirección de   correo electrónico proporcionada durante el registro es inválida o incorrecta   al intentar enviar el correo de confirmación,           Entonces el sistema muestra un mensaje de error   indicando que la dirección de correo electrónico no es válida y solicita al   usuario que verifique y proporcione una dirección de correo electrónico   válida.    |     EP01    |
|     US03    |     Verificación de     cuenta     |     Como usuario, quisiera llenar un formulario en la   creación de mi cuenta para acreditar mi nombre y mi fiabilidad.    |      <br><br>Escenario 1: "Formulario completado   correctamente"           Dado que un usuario desea crear una cuenta,           Cuando se le presente un formulario durante el   proceso de registro para ingresar su nombre y otros detalles relevantes,           Entonces el usuario puede completar el formulario   proporcionando la información requerida de manera precisa y sin errores.            <br><br>Escenario 2: "Datos guardados   correctamente"           Dado que un usuario ha completado el formulario   de registro,           Cuando hace clic en el botón de registro o envía   el formulario,           Entonces el sistema guarda los datos   proporcionados por el usuario de manera segura y asociada con su cuenta.            <br><br>Escenario 3: "Error al completar el   formulario"           Dado que un usuario desea crear una cuenta,           Cuando intenta completar el formulario de registro,   pero comete errores al ingresar su nombre u otros detalles requeridos,           Entonces el sistema muestra mensajes de error   indicando los campos que deben corregirse y no permite que el usuario   continúe hasta que se hayan corregido los errores.                  <br><br>Escenario 4: "Error al guardar datos"           Dado que un usuario ha completado el formulario   de registro,           Cuando intenta enviar el formulario, pero el   sistema encuentra un error al guardar los datos en la base de datos,           Entonces el sistema muestra un mensaje de error   indicando que no se pudieron guardar los datos y sugiere al usuario que   vuelva a intentarlo más tarde o se comunique con el soporte técnico.          |     EP01    |
|     US04    |     Registro de     empresa    |     Como usuario contador financiero, quisiera crear   una cuenta con el uso de mi correo     electrónico proporcionado por la empresa que   represento para ingresar a la aplicación.    |      <br><br>Escenario 1: "Registro exitoso"           Dado que un usuario contador financiero desea   crear una cuenta,           Cuando ingresa su dirección de correo electrónico   proporcionada por la empresa y una contraseña válida,           Entonces el sistema registra con éxito su cuenta   y lo redirige a la página de inicio.                  <br><br>Escenario 2: "Correo electrónico   válido"           Dado que un usuario contador financiero desea   crear una cuenta,           Cuando ingresa una dirección de correo   electrónico que está asociada con la empresa que representa,           Entonces el sistema acepta la dirección de correo   electrónico y permite al usuario continuar con el proceso de registro.            <br><br>Escenario 3: "Contraseña débil"           Dado que un usuario contador financiero desea   crear una cuenta,           Cuando ingresa una contraseña que no cumple con   los criterios de seguridad establecidos,           Entonces el sistema muestra un mensaje de error   indicando que la contraseña es débil y solicita al usuario que ingrese una   contraseña más segura.                  <br><br>Escenario 4: "Correo electrónico no   asociado"           Dado que un usuario contador financiero desea   crear una cuenta,           Cuando ingresa una dirección de correo   electrónico que no está asociada con la empresa que representa,           Entonces el sistema muestra un mensaje de error   indicando que la dirección de correo electrónico no está autorizada y   solicita al usuario que ingrese una dirección de correo electrónico válida   proporcionada por la empresa.    |     EP01    |
|     US05    |     Verificación de     cuenta empresa    |     Como usuario contador financiero, quisiera que se   me soliciten los datos de mi empresa para verificar la fiabilidad de esta.    |      <br><br>Escenario 1: "Solicitud de datos de la   empresa"           Dado que un usuario contador financiero desea   crear una cuenta,           Cuando el sistema solicita los datos de la   empresa que representa durante el proceso de registro,           Entonces el usuario puede proporcionar los datos   de la empresa, como el nombre, dirección, número de identificación fiscal u   otros detalles relevantes.                  <br><br>Escenario 2: "Verificación de datos de la   empresa"           Dado que un usuario contador financiero ha   proporcionado los datos de la empresa durante el registro,           Cuando el sistema verifica la autenticidad y   fiabilidad de los datos proporcionados,           Entonces el sistema procede con el registro de la   cuenta y asocia al usuario con la empresa verificada.                        <br><br>Escenario 3: "Error al solicitar datos de la   empresa"           Dado que un usuario contador financiero desea   crear una cuenta,           Cuando el sistema no solicita los datos de la   empresa durante el proceso de registro,           Entonces el usuario no puede completar el   registro y el sistema muestra un mensaje de error indicando que se requieren   los datos de la empresa para continuar.                  <br><br>Escenario 4: "Datos de empresa no   verificados"           Dado que un usuario contador financiero ha   proporcionado los datos de la empresa durante el registro,           Cuando el sistema no puede verificar la   autenticidad o fiabilidad de los datos proporcionados,           Entonces el sistema muestra un mensaje indicando   que los datos de la empresa no pudieron ser verificados y solicita al usuario   que proporcione información adicional o se comunique con el soporte técnico   para resolver el problema.                            |     EP01    |
|     US06    |     Recuperación de     cuenta     |     Como usuario, quisiera recuperar mi contraseña   por medio del correo otorgado en caso de perderla para recuperar el uso de la   cuenta.    |      <br><br>Escenario 1: "Solicitud de recuperación de   contraseña"           Dado que un usuario desea recuperar su   contraseña,           Cuando ingresa su dirección de correo electrónico   asociada con la cuenta en el formulario de recuperación de contraseña,           Entonces el sistema genera un enlace de   restablecimiento de contraseña único y lo envía por correo electrónico a la   dirección proporcionada.                  <br><br>Escenario 2: "Restablecimiento exitoso de   contraseña"           Dado que un usuario ha solicitado restablecer su   contraseña y ha recibido el correo electrónico de recuperación con el enlace,           Cuando el usuario sigue el enlace proporcionado   en el correo electrónico y establece una nueva contraseña,           Entonces el sistema actualiza la contraseña en la   base de datos y permite al usuario acceder a su cuenta con la nueva   contraseña.                  <br><br>Escenario 3: "Dirección de correo   electrónico no asociada"           Dado que un usuario desea recuperar su   contraseña,           Cuando ingresa una dirección de correo   electrónico que no está asociada con ninguna cuenta en el sistema al   solicitar la recuperación de contraseña,           Entonces el sistema muestra un mensaje de error   indicando que la dirección de correo electrónico no está asociada con ninguna   cuenta y sugiere al usuario que verifique la dirección de correo electrónico   ingresada.                  <br><br>Escenario 4: "Error al enviar correo de   recuperación"           Dado que un usuario desea recuperar su   contraseña,           Cuando el sistema intenta enviar el correo   electrónico de recuperación, pero falla debido a problemas técnicos o de   conectividad,           Entonces el sistema muestra un mensaje de error   indicando que no se pudo enviar el correo de recuperación y sugiere al   usuario que vuelva a intentarlo más tarde o se comunique con el soporte   técnico.                      |     EP01    |
|     US07    |     Visualización de     empresas    |     Como usuario inversionista, quisiera visualizar   las empresas disponibles en la aplicación     para decidir si solicitar sus datos.    |      <br><br>Escenario 1: "Visualización de empresas   disponibles"           Dado que un usuario inversionista desea explorar   las empresas disponibles,           Cuando accede a la sección designada en la   aplicación para ver la lista de empresas,           Entonces el sistema muestra una lista completa y   actualizada de todas las empresas disponibles para que el usuario las   explore.            <br><br>Escenario 2: "Detalles de la empresa"           Dado que un usuario inversionista está revisando   la lista de empresas disponibles,           Cuando selecciona una empresa específica de la   lista,           Entonces el sistema muestra información detallada   sobre esa empresa, como su nombre, sector, ubicación, tamaño, estado   financiero, y otros detalles relevantes.                  <br><br>Escenario 3: "Error al cargar empresas"           Dado que un usuario inversionista desea explorar   las empresas disponibles,           Cuando intenta acceder a la lista de empresas,   pero el sistema encuentra un error al cargar los datos,           Entonces el sistema muestra un mensaje de error   indicando que no se pudieron cargar las empresas y sugiere al usuario que   vuelva a intentarlo más tarde o se comunique con el soporte técnico.            <br><br>Escenario 4: "Empresa no encontrada"           Dado que un usuario inversionista está revisando   la lista de empresas disponibles,           Cuando busca una empresa específica pero no   encuentra ninguna coincidencia,           Entonces el sistema muestra un mensaje indicando   que la empresa no está disponible en la lista y sugiere al usuario que amplíe   su búsqueda o consulte con el equipo de soporte para obtener más información.    |     EP02    |
|     US08    |     Filtro de     empresas    |     Como usuario inversionista, quisiera filtrar la   lista de empresas disponibles para elegir las que cumplan con los requisitos.    |      <br><br>Escenario 1: "Filtrado exitoso de   empresas"           Dado que un usuario inversionista desea filtrar   la lista de empresas disponibles,           cuando selecciona los criterios de filtrado   deseados,           entonces el sistema muestra una lista de empresas   que cumplen con los criterios de filtrado seleccionados.                        <br><br>Escenario 2: "Sin resultados de   filtrado"           Dado que un usuario inversionista desea filtrar   la lista de empresas disponibles,           cuando selecciona criterios de filtrado que no   coinciden con ninguna empresa en la base de datos,           entonces el sistema muestra un mensaje indicando   que no se encontraron empresas que cumplan con los criterios de filtrado   seleccionados.    |     EP02    |
|     US09    |     Ordenamiento de empresas    |     Como usuario inversionista, quisiera ordenar la   lista de empresas disponibles para elegir las que cumplan con mis requisitos.    |      <br><br>Escenario 1: "Ordenación por nombre exitosa"                 Dado que un usuario inversionista desea ordenar   la lista de empresas disponibles,           cuando selecciona la opción de ordenar por   nombre,           entonces el sistema muestra una lista de empresas   ordenadas alfabéticamente por nombre.                        <br><br>Escenario 2: "Error de ordenación"                 Dado que un usuario inversionista desea ordenar   la lista de empresas disponibles,           cuando intenta ordenarlas, pero hay un error en   el proceso de     ordenación,           entonces el sistema muestra un mensaje de error   indicando que no se pudo completar la ordenación de las empresas.    |     EP02    |
|     US10    |     Interfaz de     búsqueda sencilla    |     Como usuario inversionista, quisiera una interfaz   de búsqueda que permita un uso rápido y     efectivo para evitar utilizar mucho tiempo en la búsqueda.    |      <br><br>Escenario 1: "Interfaz de búsqueda rápida y   efectiva"           Dado que un usuario inversionista desea encontrar   empresas de manera eficiente,           Cuando accede a la interfaz de búsqueda en la   aplicación,           Entonces la interfaz de búsqueda permite al   usuario ingresar términos de búsqueda de manera intuitiva y proporciona   resultados relevantes de manera rápida y precisa.            <br><br>Escenario 2: "Filtros de búsqueda"           Dado que un usuario inversionista desea refinar   su búsqueda,           Cuando utiliza filtros de búsqueda proporcionados   en la interfaz, como sector, ubicación, tamaño de la empresa, etc.,           Entonces la interfaz de búsqueda aplica los   filtros seleccionados y muestra resultados más específicos y relevantes según   los criterios establecidos.                  <br><br>Escenario 3: "Interfaz de búsqueda lenta o   poco eficaz"           Dado que un usuario inversionista desea encontrar   empresas de manera eficiente,           Cuando accede a la interfaz de búsqueda, pero   experimenta retrasos significativos o resultados inexactos,           Entonces el sistema muestra un mensaje indicando   que la búsqueda está tardando más de lo esperado o que los resultados no son   precisos, y sugiere al usuario que revise su consulta o intente nuevamente   más tarde.                  <br><br>Escenario 4: "Filtros de búsqueda no   funcionan correctamente"           Dado que un usuario inversionista utiliza filtros   de búsqueda para refinar sus resultados,           Cuando aplica filtros específicos pero los   resultados mostrados no coinciden con los criterios establecidos,           Entonces el sistema muestra un mensaje de error   indicando que los filtros de búsqueda no están funcionando correctamente y   sugiere al usuario que elimine o ajuste los filtros para obtener resultados   más precisos.    |     EP02    |
|     US11    |     Visualización de     solicitudes    |     Como usuario contador financiero, quisiera   visualizar las solicitudes que me han llegado para acceder a ellas.    |      <br><br>Escenario 1: "Visualización exitosa de   solicitudes"                 Dado que un usuario contador financiero desea   visualizar las solicitudes recibidas,           cuando accede a la sección correspondiente en la aplicación,           entonces el sistema muestra una lista de las   solicitudes recibidas por el contador financiero.                        <br><br>Escenario 2: "Error al cargar   solicitudes"                 Dado que un usuario contador financiero desea   visualizar las solicitudes recibidas,           cuando intenta acceder a la sección correspondiente,   pero hay un error en la carga de datos,           entonces el sistema muestra un mensaje de error   indicando que no se pueden cargar las solicitudes recibidas en este momento.    |     EP02    |
|     US12    |     Filtro de     solicitudes    |     Como usuario contador financiero, quisiera   filtrar las solicitudes recibidas según diferentes criterios para mantener un   mayor orden.    |            <br><br>Escenario 1: "Filtrado exitoso de   solicitudes"           Dado que un usuario contador financiero desea   filtrar las solicitudes recibidas,           cuando selecciona los criterios de filtrado   deseados,           entonces el sistema muestra una lista de   solicitudes que cumplen con los criterios de filtrado seleccionados.            <br><br>Escenario 2: "Sin resultados de   filtrado"           Dado que un usuario contador financiero desea   filtrar las solicitudes recibidas,           cuando selecciona criterios de filtrado que no   coinciden con ninguna solicitud en la base de datos,           entonces el sistema muestra un mensaje indicando   que no se encontraron solicitudes que cumplan con los criterios de filtrado   seleccionados.    |     EP02    |
|     US13    |     Ordenamiento de solicitudes    |     Como usuario contador financiero, quisiera ordenar   las solicitudes recibidas según diferentes criterios para mantener un mayor   orden.    |      <br><br>Escenario 1: "Ordenación exitosa de   solicitudes"           Dado que un usuario contador financiero desea   ordenar las solicitudes recibidas,           cuando selecciona un criterio de ordenación,           entonces el sistema muestra una lista de   solicitudes ordenadas según el criterio seleccionado.            <br><br>Escenario 2: "Error de ordenación"           Dado que un usuario contador financiero desea   ordenar las solicitudes recibidas,           cuando intenta ordenarlas, pero hay un error en   el proceso de ordenación,           entonces el sistema muestra un mensaje de error   indicando que no se pudo completar la ordenación de las solicitudes.    |     EP02    |
|     US14    |     Admisión de     solicitudes    |     Como usuario contador financiero, quisiera   aceptar o rechazar solicitudes que reciba para mantener un control de los   datos que estoy permitido entregar.    |      <br><br>Escenario 1: "Aceptación exitosa de   solicitud"           Dado que un usuario contador financiero desea   aceptar una solicitud recibida,           cuando selecciona la solicitud correspondiente y   elige la opción de aceptar,           entonces el sistema procesa la solicitud y   actualiza su estado como aceptada correctamente.                        <br><br>Escenario 2: "Rechazo exitoso de   solicitud"           Dado que un usuario contador financiero desea   rechazar una solicitud recibida,           cuando selecciona la solicitud correspondiente y   elige la opción de rechazar,           entonces el sistema procesa la solicitud y   actualiza su estado como rechazada correctamente.    |     EP02    |
|     US15    |     Creación de la     solicitud    |     Como usuario inversionista, quisiera solicitar   los datos que quiero conocer sobre la     empresa que elegí para realizar los análisis necesarios.    |      <br><br>Escenario 1: "Solicitud exitosa de   datos"                       Dado que un usuario inversionista desea solicitar   datos específicos sobre una empresa,           cuando selecciona la empresa deseada y especifica   los datos que desea obtener,           entonces el sistema registra la solicitud   correctamente y la envía al contador financiero correspondiente para su   procesamiento.                        <br><br>Escenario 2: "Error al enviar la   solicitud"                 Dado que un usuario inversionista desea solicitar   datos sobre una empresa,           cuando intenta enviar la solicitud, pero hay un   error en el proceso,           entonces el sistema muestra un mensaje de error   indicando que no se pudo procesar la solicitud en este momento.    |     EP02    |
|     US16    |     Consulta de     orden de solicitud    |     Como usuario inversionista, quisiera saber en qué   puesto de atención me encuentro para calcular cuándo volver a ingresar a la   aplicación al recibir el estado de mi solicitud    |      <br><br>Escenario 1: "Visualización exitosa del   puesto de atención"                       Dado que un usuario inversionista desea conocer   su puesto de atención en la cola de solicitudes,           cuando accede a la sección correspondiente en la   aplicación,           entonces el sistema muestra claramente el puesto   actual del usuario en la cola de solicitudes.                        <br><br>Escenario 2: "Error al obtener el puesto de   atención"                       Dado que un usuario inversionista desea conocer   su puesto de atención en la cola de solicitudes,           cuando intenta acceder a la sección correspondiente,   pero hay un error en el proceso,           entonces el sistema muestra un mensaje de error   indicando que no se puede mostrar el puesto de atención en este momento.    |     EP02    |
|     US17    |     Actualizaciones     sobre la solicitud    |     Como usuario inversionista, quisiera recibir   notificaciones sobre el estado de mi solicitud para mantener un trabajo más   organizado.    |      <br><br>Escenario 1: "Notificación de actualización   de estado"                 Dado que un usuario inversionista ha realizado   una solicitud,           cuando hay un cambio en el estado de su solicitud,           entonces el sistema envía una notificación al   usuario informándole sobre el     nuevo estado de su solicitud para mantenerlo   informado y facilitar la organización de su trabajo.                        <br><br>Escenario 2: "Falta de notificaciones de   estado"                       Dado que un usuario inversionista ha realizado   una solicitud,           cuando hay un cambio en el estado de su solicitud,   pero el sistema no envía notificaciones,           entonces el usuario no está informado sobre el   progreso de su solicitud, lo que puede dificultar la organización y   seguimiento de su trabajo.    |     EP02    |
|     US18    |     Respuesta de     solicitud    |     Como usuario     inversionista, quisiera recibir la respuesta   sobre mi solicitud realizada     para conocer si fue aprobada o no.    |      <br><br>Escenario 1: "Recepción de respuesta sobre   solicitud"           Dado que un usuario inversionista ha realizado   una solicitud,           cuando la solicitud ha sido procesada y se ha   tomado una decisión,           entonces el sistema envía una notificación al   usuario informándole sobre el resultado de su solicitud para mantenerlo   informado sobre el estado de su solicitud.            <br><br>Escenario 2: "Falta de respuesta sobre   solicitud"           Dado que un usuario inversionista ha realizado   una solicitud,           cuando la solicitud ha sido procesada pero el   sistema no envía una notificación con el resultado,           entonces el usuario no está informado sobre si su   solicitud fue aprobada o rechazada, lo que puede generar incertidumbre y   dificultar la toma de decisiones.    |     EP02    |
|     US19    |     Razón de la     respuesta otorgada    |     Como usuario inversionista, quisiera recibir una   explicación en caso de haberse rechazado mi solicitud para confirmar si tal   razón está bien o mal infundada.    |      <br><br>Escenario 1: "Recepción de explicación de   rechazo"                       Dado que un usuario inversionista ha tenido una   solicitud rechazada,           cuando recibe la notificación de rechazo,           entonces el sistema proporciona una explicación   detallada sobre los motivos del rechazo, permitiendo al usuario comprender completamente   la decisión y determinar si está justificada.                        <br><br>Escenario 2: "Falta de explicación de   rechazo"                 Dado que un usuario inversionista ha tenido una   solicitud rechazada,           cuando recibe la notificación de rechazo, pero no   se proporciona ninguna explicación,           entonces el usuario queda sin entender los   motivos del rechazo, lo que puede generar confusión y frustración sobre la   decisión tomada.    |     EP02    |
|     US20    |     Creación de     queja    |     Como usuario inversionista, quisiera realizar una   queja en caso se hayan entregado datos     erróneos para corregir el error realizado.    |      <br><br>Escenario 1: "Presentación exitosa de queja   por datos erróneos"           Dado que un usuario inversionista ha recibido   datos incorrectos,           cuando presenta una queja especificando los datos   incorrectos y proporcionando evidencia relevante,           entonces el sistema registra la queja   correctamente y notifica al equipo responsable para corregir el error.                  <br><br>Escenario 2: "Problemas al presentar la   queja"           Dado que un usuario inversionista ha recibido   datos incorrectos,           cuando intenta presentar una queja, pero   encuentra dificultades técnicas o de interfaz,           entonces el usuario no puede comunicar   efectivamente el problema, lo que dificulta la corrección del error.    |     EP02    |
|     US21    |     Visualización de     datos recibidos    |     Como usuario inversionista, quisiera visualizar   los datos pedidos en caso de haberse aceptado mi solicitud para evaluarlos y   utilizarlos en un análisis financiero.    |      <br><br>Escenario 1: "Visualización de datos   solicitados"           Dado que un usuario inversionista ha tenido una   solicitud aceptada,           Cuando accede a la sección designada en la   aplicación para ver los datos solicitados,           Entonces el sistema muestra una lista completa y   actualizada de todos los datos proporcionados por la empresa, incluyendo   información financiera, informes, documentos legales, y cualquier otro dato   relevante para el análisis financiero.                  <br><br>Escenario 2: "Detalle de los datos   solicitados"           Dado que un usuario inversionista está revisando   los datos solicitados,           Cuando selecciona un conjunto específico de datos   de la lista,           Entonces el sistema muestra información detallada   sobre esos datos, como su origen, fecha de entrega, formato, y cualquier otra   información relevante que pueda ser útil para el análisis financiero.                  <br><br>Escenario 3: "Error al cargar datos   solicitados"           Dado que un usuario inversionista desea ver los   datos solicitados,           Cuando intenta acceder a la lista de datos, pero   el sistema encuentra un error al cargar los datos,           Entonces el sistema muestra un mensaje de error   indicando que no se pudieron cargar los datos y sugiere al usuario que vuelva   a intentarlo más tarde o se comunique con el soporte técnico.            <br><br>Escenario 4: "Datos solicitados no   encontrados"           Dado que un usuario inversionista está revisando   la lista de datos solicitados,           Cuando busca un conjunto específico de datos,   pero no encuentra ninguna coincidencia,           Entonces el sistema muestra un mensaje indicando   que los datos solicitados no están disponibles en la lista y sugiere al   usuario que consulte con el equipo de soporte para obtener más información.                            |     EP04    |
|     US22    |     Cierre de     solicitud    |     Como usuario inversionista, quisiera visualizar   los datos obtenidos hasta cerrar y marcar como completada la solicitud para   tener el tiempo necesario con los datos sin comprometer a la empresa a la   cual solicité.    |      <br><br>Escenario 1: "Visualización de datos   obtenidos"           Dado que un usuario inversionista ha realizado   una solicitud y ha obtenido datos de una empresa,           Cuando accede a la sección designada en la   aplicación para ver los datos obtenidos,           Entonces el sistema muestra una lista completa y   actualizada de todos los datos proporcionados por la empresa, incluyendo   información financiera, informes, documentos legales, y cualquier otro dato   relevante.                  <br><br>Escenario 2: "Cierre de solicitud y marcado   como completada"           Dado que un usuario inversionista ha obtenido los   datos que necesita y no desea comprometer a la empresa solicitada,           Cuando cierra y marca como completada la   solicitud correspondiente,           Entonces el sistema detiene cualquier acción   adicional relacionada con la solicitud y garantiza que los datos obtenidos   permanezcan accesibles para el usuario sin comprometer a la empresa   solicitada.                  <br><br>Escenario 3: "Error al cargar datos   obtenidos"           Dado que un usuario inversionista desea ver los   datos obtenidos,           Cuando intenta acceder a la lista de datos, pero   el sistema encuentra un error al cargar los datos,           Entonces el sistema muestra un mensaje de error   indicando que no se pudieron cargar los datos y sugiere al usuario que vuelva   a intentarlo más tarde o se comunique con el soporte técnico.                  <br><br>Escenario 4: "Error al cerrar la   solicitud"           Dado que un usuario inversionista intenta cerrar   y marcar como completada una solicitud,           Cuando el sistema encuentra un error al procesar   esta acción,           Entonces el sistema muestra un mensaje de error   indicando que no se pudo completar la solicitud y sugiere al usuario que   vuelva a intentarlo más tarde o se comunique con el soporte técnico.    |     EP02    |
|     US23    |     Seguridad de     entrega    |     Como usuario contador financiero, quisiera   entregar los datos solicitados sabiendo que se realizará la entrega a través   de un canal seguro para mantener la seguridad de mi compañía.    |      <br><br>Escenario 1: "Entrega segura de datos   solicitados"           Dado que un usuario contador financiero desea   entregar los datos solicitados,           cuando procede con la entrega de los datos a   través del canal designado por la aplicación,           entonces el sistema garantiza que la entrega se   realice de manera segura, utilizando medidas de cifrado y protección de   datos, para salvaguardar la información confidencial de la compañía.                        <br><br>Escenario 2: "Preocupaciones sobre la   seguridad del canal de entrega"           Dado que un usuario contador financiero desea   entregar los datos solicitados,           cuando existe incertidumbre o falta de claridad   sobre la seguridad del canal de entrega proporcionado por la aplicación,           entonces el usuario se muestra renuente a   proceder con la entrega de los datos, lo que puede generar preocupaciones   sobre la seguridad de la información de la compañía.    |     EP03    |
|     US24    |     Limitación al     entregar datos    |     Como usuario contador financiero, quisiera que no   se permita descargar ni tomar captura de pantalla de los datos compartidos   para mantener la confidencialidad de la empresa.    |      <br><br>Escenario 1: "Restricción de descarga de   datos"           Dado que un usuario contador financiero desea   mantener la confidencialidad de los datos compartidos,           Cuando accede a la sección designada en la   aplicación para ver los datos compartidos,           Entonces el sistema implementa medidas de   seguridad que impiden la descarga de los datos en formato descargable, como   archivos PDF o documentos.            <br><br>Escenario 2: "Restricción de captura de   pantalla"           Dado que un usuario contador financiero desea   mantener la confidencialidad de los datos compartidos,           Cuando visualiza los datos en la aplicación,           Entonces el sistema implementa medidas de   seguridad que detectan y previenen la captura de pantalla de los datos, como   deshabilitar la función de captura de pantalla mientras se visualizan los   datos sensibles.                  <br><br>Escenario 3: "Descarga no restringida"           Dado que un usuario contador financiero desea   mantener la confidencialidad de los datos compartidos,           Cuando accede a la sección designada en la   aplicación para ver los datos compartidos, y el sistema permite la descarga   de los datos en formatos descargables, como archivos PDF o documentos,           Entonces el sistema no cumple con los requisitos   de seguridad establecidos y se requiere una mejora para restringir la   descarga de los datos.            <br><br>Escenario 4: "Captura de pantalla   habilitada"           Dado que un usuario contador financiero desea   mantener la confidencialidad de los datos compartidos,           Cuando visualiza los datos en la aplicación, y el   sistema no impide la captura de pantalla de los datos sensibles,           Entonces el sistema no cumple con los requisitos   de seguridad establecidos y se requiere una mejora para prevenir la captura   de pantalla de los datos sensibles.                |     EP03    |
|     US25    |     Alertas de fugas     de seguridad    |     Como usuario contador financiero, quisiera   recibir alertas de violaciones de seguridad para informar a la empresa sobre   el problema.    |      <br><br>Escenario 1: "Recepción de alerta de   violación de seguridad"           Dado que un usuario contador financiero desea   estar al tanto de posibles violaciones de seguridad,           cuando se detecta una actividad sospechosa o una   violación de seguridad en la aplicación,           entonces el sistema envía una alerta inmediata al   usuario contador financiero, notificándole sobre el problema y proporcionando   detalles pertinentes para que pueda informar rápidamente a la empresa y tomar   las medidas necesarias para abordar la situación.            <br><br>Escenario 2: "Falta de alertas de   violaciones de seguridad"           Dado que un usuario contador financiero desea   estar al tanto de posibles violaciones de seguridad,           cuando ocurre una violación de seguridad, pero el   sistema no envía ninguna alerta al usuario,           entonces el usuario no es consciente del   incidente y la empresa puede no ser informada oportunamente, lo que aumenta   el riesgo de daños adicionales o pérdida de datos.    |     EP03    |
|     US26    |     Visualización de     análisis financieros disponibles    |     Como usuario inversionista, quisiera visualizar   los análisis financieros disponibles con los datos que me entregaron para   conocer si los datos solicitados fueron los correctos.    |      <br><br>Escenario 1: "Visualización exitosa de análisis   financieros"                 Dado que un usuario inversionista desea revisar   los análisis financieros disponibles,           cuando accede a la sección correspondiente en la aplicación,           entonces el sistema muestra una lista completa de   los análisis financieros disponibles, generados a partir de los datos   entregados, permitiendo al usuario revisar y evaluar la calidad de la   información recibida.                        <br><br>Escenario 2: "Falta de análisis financieros   disponibles"                       Dado que un usuario inversionista desea revisar   los análisis financieros disponibles,           cuando accede a la sección correspondiente en la aplicación,   pero no se muestran análisis financieros,           entonces el usuario no puede verificar la   precisión de los datos entregados y puede tener dudas sobre la calidad de la   información proporcionada.    |     EP04    |
|     US27    |     Eficacia de los     algoritmos de análisis financiero    |     Como usuario inversionista, quisiera realizar   cualquier análisis financiero disponible de     manera rápida y sencilla para agilizar el proceso   de evaluación.    |      <br><br>Escenario 1: "Realización exitosa de   análisis financiero"           Dado que un usuario inversionista desea realizar   un análisis financiero,           cuando accede a la herramienta de análisis   financiero disponible en la aplicación,           entonces el sistema le proporciona una interfaz   intuitiva y fácil de usar que le permite seleccionar los parámetros deseados   y ejecutar el análisis de manera rápida y eficiente, agilizando así el   proceso de evaluación.                  <br><br>Escenario 2: "Problemas de usabilidad en la   herramienta de análisis financiero"           Dado que un usuario inversionista desea realizar   un análisis financiero,           cuando intenta utilizar la herramienta de   análisis financiero, pero encuentra dificultades en la navegación o en la   comprensión de los parámetros,           entonces el usuario experimenta frustración y el   proceso de evaluación se vuelve lento y complicado, afectando negativamente   su experiencia con la aplicación.    |     EP04    |
|     US28    |     conclusión del     análisis financiero    |     Como usuario inversionista, quisiera recibir un   veredicto en base a los análisis que se     realizaron con la aplicación para tener otra   perspectiva sobre la evaluación.    |      <br><br>Escenario 1: "Veredicto claro y   fundamentado"           Dado que un usuario inversionista ha realizado análisis   utilizando la aplicación,           cuando finaliza los análisis financieros,           entonces el sistema proporciona un veredicto   claro y fundamentado basado en     los resultados de los análisis, ofreciendo al   usuario una perspectiva adicional para su evaluación.            <br><br>Escenario 2: "Falta de veredicto o   información insuficiente"           Dado que un usuario inversionista ha realizado   análisis utilizando la aplicación,           cuando finaliza los análisis financieros pero el   sistema no proporciona un veredicto o la información proporcionada es   insuficiente para tomar una     decisión informada,           entonces el usuario puede sentirse frustrado y   enfrentar dificultades para obtener una perspectiva adicional sobre la   evaluación de la empresa.    |     EP04    |
|     US29    |     RESTful     API Registro de usuario    |     Como desarrollador, quiero implementar un   endpoint de registro de usuario para permitir que los usuarios se registren   en la aplicación mediante la API RESTful.    |      <br><br>Escenario 1: "Registro exitoso"                 Dado que un usuario desea registrarse en la   aplicación a través de la API RESTful,           cuando envía una solicitud de registro con la   información requerida al endpoint correspondiente,           entonces el sistema procesa la solicitud   correctamente, crea la cuenta del usuario y devuelve una respuesta con un   código de estado HTTP 201 y     un mensaje indicando el éxito del registro.                  <br><br>Escenario 2: "Fallo en el registro"                       Dado que un usuario intenta registrarse en la   aplicación a través de la API RESTful,           cuando envía una solicitud de registro al   endpoint correspondiente, pero la     información proporcionada no cumple con los   requisitos mínimos,                 entonces el sistema devuelve una respuesta con un   código de estado HTTP 400 y un mensaje de error indicando la causa del fallo   en el registro.    |     EP05    |
|     US30    |     RESTful API Inicio de sesión de usuario    |     Como desarrollador, quiero implementar un   endpoint de inicio de sesión para permitir que los usuarios accedan a sus   cuentas mediante la API RESTful.    |      <br><br>Escenario 1: "Inicio de sesión exitoso"                 Dado que un usuario desea iniciar sesión en la   aplicación a través de la API RESTful,           cuando envía una solicitud de inicio de sesión   con las credenciales al endpoint correspondiente,           entonces el sistema autentica al usuario, genera   un token de acceso válido y devuelve una respuesta con un código de estado   HTTP 200 junto con el token de acceso para la sesión.                  <br><br>Escenario 2: "Fallo en el inicio de   sesión"                       Dado que un usuario intenta iniciar sesión en la   aplicación a través de la API RESTful,           cuando envía una solicitud de inicio de sesión al   endpoint correspondiente, pero las credenciales proporcionadas son   incorrectas o la cuenta no existe,           entonces el sistema devuelve una respuesta con un   código de estado HTTP 401 y un mensaje de error indicando que el inicio de   sesión ha fallado.    |     EP05    |
|     US31    |     Autenticación basada en token JWT    |     Como desarrollador, para mejorar la seguridad de   la API, quiero implementar la funcionalidad de autenticación basada en token   JWT.    |      <br><br>Escenario 1: "Generación de token JWT"                 Dado que un usuario autenticado desea acceder a   recursos protegidos en la API RESTful,           cuando el sistema valida las credenciales del   usuario correctamente,           entonces el sistema genera un token JWT válido   que contiene la información de autenticación del usuario y tiene una fecha de   expiración adecuada.                        <br><br>Escenario 2: "Autenticación con token   JWT"                       Dado que un usuario desea acceder a recursos   protegidos en la API RESTful,           cuando el usuario envía una solicitud a un   endpoint protegido incluyendo el token JWT en el encabezado de autorización,           entonces el sistema verifica la validez del token   JWT y, si es válido y no ha expirado, permite al usuario acceder al recurso   solicitado.                        <br><br>Escenario 3: "Token JWT inválido"                       Dado que un usuario intenta acceder a recursos   protegidos en la API RESTful,           cuando el usuario incluye un token JWT inválido   en el encabezado de autorización de la solicitud,           entonces el sistema rechaza la solicitud y   devuelve una respuesta con un código de estado HTTP 401 indicando que la   autenticación ha fallado.    |     EP05    |
|     US32    |     Recuperación de contraseña    |     Como desarrollador, quiero implementar un   endpoint de recuperación de contraseña para permitir que los usuarios restablezcan   sus contraseñas mediante la API RESTful.    |      <br><br>Escenario 1: "Solicitud de restablecimiento de   contraseña"                       Dado que un usuario olvidó su contraseña y desea restablecerla,           cuando envía una solicitud POST al endpoint de   recuperación de contraseña con su dirección de correo electrónico registrada,           entonces el sistema verifica la existencia del   correo electrónico en la base de datos y genera un token de restablecimiento   de contraseña único asociado a la cuenta del usuario.                        <br><br>Escenario 2: "Envío de correo electrónico de   restablecimiento"                       Dado que un usuario ha solicitado restablecer su   contraseña correctamente,           cuando el sistema genera el token de   restablecimiento de contraseña,           entonces envía un correo electrónico al usuario   con un enlace único que contiene el token y las instrucciones para   restablecer la contraseña.                        <br><br>Escenario 3: "Validación del token de   restablecimiento"                       Dado que un usuario hace clic en el enlace de   restablecimiento de contraseña recibida por correo electrónico,           cuando el sistema recibe la solicitud de   restablecimiento con el token incluido,           entonces verifica la validez del token y permite   al usuario continuar con el proceso de restablecimiento si el token es   válido.                        <br><br>Escenario 4: "Restablecimiento de   contraseña"                       Dado que un usuario desea establecer una nueva contraseña   después de validar el token,           cuando completa el formulario de restablecimiento   de contraseña con una nueva contraseña,           entonces el sistema actualiza la contraseña   asociada a la cuenta del usuario y lo redirige a la página de inicio de   sesión con un mensaje de éxito.    |     EP05    |
|     US33    |     CRUD para recursos principales    |     Como desarrollador, quisiera implementar endpoint   CRUD para la gestión de recursos principales de la aplicación, como   publicaciones, comentarios, etc., utilizando la API RESTful.    |      <br><br>Escenario 1: "Creación de recursos"                 Dado que un usuario desea crear un nuevo recurso   en la aplicación,           cuando envía una solicitud POST al endpoint correspondiente   con los datos del nuevo recurso,           entonces el sistema procesa la solicitud y crea   el recurso en la base de datos, devolviendo una respuesta con el código de   estado HTTP 201 y la ubicación del recurso creado en el encabezado de la respuesta.                        <br><br>Escenario 2: "Obtención de recursos"                 Dado que un usuario desea obtener información   sobre un recurso específico en la aplicación,           cuando envía una solicitud GET al endpoint   correspondiente con el identificador del recurso,           entonces el sistema busca el recurso en la base   de datos y devuelve una respuesta con el código de estado HTTP 200 y los   datos del recurso solicitado en el cuerpo de la respuesta.                        <br><br>Escenario 3: "Actualización de   recursos"                 Dado que un usuario desea actualizar un recurso   existente en la aplicación,           cuando envía una solicitud PUT al endpoint   correspondiente con los datos actualizados del recurso y el identificador del   recurso a actualizar,           entonces el sistema busca el recurso en la base   de datos, lo actualiza con los nuevos datos proporcionados y devuelve una   respuesta con el código de     estado HTTP 200 indicando que la actualización se   realizó correctamente.                        <br><br>Escenario 4: "Eliminación de recursos"                       Dado que un usuario desea eliminar un recurso   existente en la aplicación,           cuando envía una solicitud DELETE al endpoint correspondiente   con el identificador del recurso a eliminar,           entonces el sistema busca y elimina el recurso de   la base de datos y devuelve una respuesta con el código de estado HTTP 204   (No Content) indicando que la eliminación se realizó con éxito.    |     EP05    |
|     US34    |     Paginación y filtrado de resultados    |     Como desarrollador, para mejorar la eficiencia de   la API, quiero implementar la paginación y el filtrado para los endpoints que   devuelven colecciones de recursos.    |      <br><br>Escenario 1: "Paginación de resultados"                       Dado que un usuario desea obtener una gran   cantidad de recursos de manera eficiente,           cuando realiza una solicitud a un endpoint que   devuelve una colección de recursos,           entonces el sistema paginará los resultados y   devolverá solo una cantidad específica de recursos por página, según los   parámetros de paginación proporcionados en la solicitud.                        <br><br>Escenario 2: "Filtrado de resultados"                       Dado que un usuario desea obtener recursos   específicos que cumplan ciertos criterios,           cuando realiza una solicitud a un endpoint que   admite filtrado,           entonces el sistema aplicará los filtros   especificados en la solicitud y devolverá solo los recursos que coincidan con   los criterios de filtrado proporcionados.    |     EP05    |
|     US35    |     Descubrimiento intuitivo    |     Como visitante de la landing page, quiero   encontrar una navegación intuitiva que me permita acceder fácilmente a la   información relevante sobre la aplicación y sus características principales.    |      <br><br>Escenario 1: "Navegación     intuitiva"                 Dado que soy un visitante de la landing page,           cuando accedo a la página principal,           entonces encuentro una barra de navegación clara   y bien organizada que me permite acceder fácilmente a las secciones   principales de la aplicación, como características, precios, contacto, etc.                        <br><br>Escenario 2: "Falta de navegación   clara"                       Dado que soy un visitante de la landing page,           cuando accedo a la página principal y la barra de   navegación no está claramente visible o no puedo encontrar información   relevante sobre las     características principales de la aplicación,           entonces me siento frustrado y es menos probable   que continúe explorando la página o considere utilizar la aplicación.    |     EP06    |
|     US36    |     Contenido informativo    |     Como usuario interesado, quiero encontrar   contenido detallado y fácil de entender sobre las funcionalidades y   beneficios de la aplicación en la landing page para tomar una decisión informada   sobre su uso.    |      <br><br>Escenario 1: "Contenido detallado y comprensible"                       Dado que soy un usuario interesado,           cuando visito la landing page de la aplicación,           entonces encuentro contenido detallado y fácil de   entender que describe claramente las funcionalidades y beneficios de la   aplicación, lo que me permite comprender completamente qué ofrece y cómo   puede beneficiarme.                        <br><br>Escenario 2: "Contenido confuso o   insuficiente"                       Dado que soy un usuario interesado,           cuando visito la landing page de la aplicación y   encuentro contenido confuso, incompleto o difícil de entender sobre las   funcionalidades y beneficios de la aplicación,           entonces me siento desorientado y tengo   dificultades para tomar una decisión informada sobre si debo usar la   aplicación o no.    |     EP06    |
|     US37    |     Compatibilidad móvil    |     Como usuario que accede desde dispositivos   móviles, quiero que la landing page esté optimizada para dispositivos   móviles, garantizando una experiencia de navegación fluida y accesible.    |      <br><br>Escenario 1: "Optimización para     dispositivos móviles"                       Dado que soy un usuario que accede desde   dispositivos móviles,           cuando visito la landing page de la aplicación   desde mi dispositivo móvil,           entonces encuentro que la página está   completamente optimizada para dispositivos móviles, con un diseño responsive   que se adapta perfectamente a la pantalla de mi dispositivo, lo que garantiza   una experiencia de navegación     fluida y accesible.                        <br><br>Escenario 2: "Problemas de visualización o   navegación"                       Dado que soy un usuario que accede desde   dispositivos móviles,           cuando visito la landing page de la aplicación   desde mi dispositivo móvil y encuentro problemas de visualización o   navegación, como elementos superpuestos, texto ilegible o botones difíciles   de seleccionar,           entonces me resulta frustrante y difícil   interactuar con la página, lo que afecta negativamente mi experiencia de   usuario.    |     EP06    |
|     US38    |     Formulario de contacto    |     Como usuario interesado, quiero encontrar un   formulario de contacto en la landing page para poder comunicarme con el   equipo de la aplicación y obtener respuestas a mis preguntas de manera rápida   y sencilla.    |      <br><br>Escenario 1: "Acceso rápido al formulario de   contacto"                 Dado que soy un usuario interesado en la   aplicación,           cuando visito la landing page,           entonces encuentro de manera clara y prominente   un formulario de contacto que me permite comunicarme fácilmente con el equipo   de la aplicación para realizar consultas o solicitar información adicional.                        <br><br>Escenario 2: "Falta de formulario de   contacto"                 Dado que soy un usuario interesado en la   aplicación,           cuando visito la landing page,           entonces no encuentro un formulario de contacto o   cualquier medio claro para comunicarme con el equipo de la aplicación, lo que   me deja sin la posibilidad de obtener respuestas a mis preguntas de manera   rápida y sencilla, lo que podría disminuir mi interés en la     aplicación.    |     EP06    |
|     US39    |     Contenido multimedia    |     Como visitante de la landing page, quiero   encontrar contenido multimedia, como imágenes y videos, que ilustren las   características y beneficios de la aplicación de manera visualmente   atractiva.    |      <br><br>Escenario 1: "Contenido multimedia disponible"                       Dado que soy un visitante de la landing page,           cuando navego por la página,           entonces encuentro contenido multimedia, como   imágenes y videos, que ilustran las características y beneficios de la   aplicación de manera visualmente atractiva, lo que me ayuda a comprender   mejor su funcionalidad y valor.                        <br><br>Escenario 2: "Falta de contenido   multimedia"                 Dado que soy un visitante de la landing page,           cuando navego por la página,           entonces no encuentro ningún contenido   multimedia, como imágenes o videos, que ilustre las características y   beneficios de la aplicación, lo que dificulta mi comprensión de la   funcionalidad y el valor de la aplicación, disminuyendo así mi interés en   explorarla más a fondo.    |     EP06    |
|     US40    |     Call-to-action claro    |     Como usuario potencial, quiero encontrar llamadas   claras a la acción en la landing page, como botones de registro o descarga,   que me guíen hacia el siguiente paso en mi interacción con la aplicación.    |      <br><br>Escenario 1: "Llamadas a la acción claras   presentes"           Dado que soy un usuario potencial que visita la   landing page,           cuando navego por la página,     entonces encuentro llamadas claras a la acción,   como botones de registro o descarga, que me guían hacia el siguiente paso en   mi interacción con la aplicación,            entonces facilita mi proceso de registro o   descubrimiento de esta.            <br><br>Escenario 2: "Falta de llamadas a la   acción"           Dado que soy un usuario potencial que visita la   landing page,           cuando navego por la página,     entonces no encuentro ninguna llamada a la acción   clara, como botones de registro o descarga, que me guíen hacia el siguiente   paso en mi interacción con la aplicación,            entonces mi proceso de registro o descubrimiento   de esta y puede llevarme a abandonar la página sin realizar ninguna acción.    |     EP06    |


## *Impact Mapping*

Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with the release of Letraset sheets containing Lorem Ipsum passages, and more recently with desktop publishing software like Aldus PageMaker including versions of Lorem Ipsum.

## *Product Backlog*

|     #Orden    |     User Story id    |     Titulo    |     Descripción    |     Story points     (1 / 2 / 3 / 5 / 8)    |
|---|---|---|---|---|
|     1    |     US36    |     Contenido   informativo    |     Como usuario   interesado, quiero encontrar contenido detallado y fácil de entender sobre   las funcionalidades y beneficios de la aplicación en la landing page para   tomar una decisión informada sobre su uso.    |     3    |
|     2    |     US37    |     Compatibilidad   móvil    |     Como usuario   que accede desde dispositivos móviles, quiero que la landing page esté   optimizada para dispositivos móviles, garantizando una experiencia de   navegación fluida y accesible.    |     3    |
|     3    |     US38    |     Formulario de   contacto    |     Como usuario   interesado, quiero encontrar un formulario de contacto en la landing page   para poder comunicarme con el equipo de la aplicación y obtener respuestas a   mis preguntas de manera rápida y sencilla.    |     2    |
|     4    |     US35    |     Descubrimiento   intuitivo    |     Como   visitante de la landing page, quiero encontrar una navegación intuitiva que   me permita acceder fácilmente a la información relevante sobre la aplicación   y sus características principales.    |     2    |
|     5    |     US39    |     Contenido   multimedia    |     Como   visitante de la landing page, quiero encontrar contenido multimedia, como   imágenes y videos, que ilustren las características y beneficios de la   aplicación de manera visualmente atractiva.    |     2    |
|     6    |     US40    |     Call-to-action   claro    |     Como usuario   potencial, quiero encontrar llamadas claras a la acción en la landing page,   como botones de registro o descarga, que me guíen hacia el siguiente paso en   mi interacción con la aplicación.    |     3    |
|     7    |     US29    |     RESTful API   Registro de usuario    |     Como   desarrollador, quiero implementar un endpoint de registro de usuario para   permitir que los usuarios se registren en la aplicación mediante la API   RESTful.    |     5    |
|     8    |     US30    |     RESTful API   Inicio de sesión de usuario    |     Como   desarrollador, quiero implementar un endpoint de inicio de sesión para   permitir que los usuarios accedan a sus cuentas mediante la API RESTful.    |     5    |
|     9    |     US31    |     Autenticación   basada en token JWT    |     Como   desarrollador, para mejorar la seguridad de la API, quiero implementar la   funcionalidad de autenticación basada en token JWT.    |     5    |
|     10    |     US32    |     Recuperación   de contraseña    |     Como   desarrollador, quiero implementar un endpoint de recuperación de contraseña   para permitir que los usuarios restablezcan sus contraseñas mediante la API   RESTful.    |     2    |
|     11    |     US33    |     CRUD para   recursos principales    |     Como   desarrollador, quisiera implementar endpoints CRUD para la gestión de   recursos principales de la aplicación, como publicaciones, comentarios, etc.,   utilizando la API RESTful.    |     5    |
|     12    |     US34    |     Paginación y   filtrado de resultados    |     Como   desarrollador, para mejorar la eficiencia de la API, quiero implementar la   paginación y el filtrado para los endpoints que devuelven colecciones de   recursos.    |     3    |
|     13    |     US01    |     Registro de   inversor     |     Como usuario   inversionista, quisiera crear una cuenta con el uso de mi correo electrónico   para representarme en la aplicación.    |     3    |
|     14    |     US02    |     Confirmación   de creación de cuenta    |     Como usuario   inversionista, quisiera recibir una confirmación de la creación de mi cuenta   a través del correo electrónico que proporcionó para confirmar la creación de   la cuenta.    |     2    |
|     15    |     US03    |     Verificación   de cuenta     |     Como usuario,   quisiera llenar un formulario en la creación de mi cuenta para acreditar mi   nombre y mi fiabilidad.    |     2    |
|     16    |     US04    |     Registro de   empresa    |     Como usuario   contador financiero, quisiera crear una cuenta con el uso de mi correo   electrónico proporcionado por la empresa que represento para ingresar a la   app    |     5    |
|     17    |     US07    |     Visualización   de empresas    |     Como usuario   inversionista, quisiera visualizar las empresas disponibles en la aplicación   para decidir si solicitar sus datos.    |     3    |
|     18    |     US11    |     Visualización   de solicitudes    |     Como usuario   contador financiero, quisiera visualizar las solicitudes que me han llegado   para acceder a ellas.    |     3    |
|     19    |     US14    |     Admisión de   solicitudes    |     Como usuario   contador financiero, quisiera aceptar o rechazar solicitudes que reciba para   mantener un control de los datos que estoy permitido entregar.    |     2    |
|     20    |     US15    |     Creación de   la solicitud    |     Como usuario   inversionista, quisiera solicitar los datos que quiero conocer sobre la   empresa que elegí para realizar los análisis necesarios.    |     2    |
|     21    |     US18    |     Respuesta de   solicitud    |     Como usuario inversionista,   quisiera recibir la respuesta sobre mi solicitud realizada para conocer si   fue aprobada o no.    |     2    |
|     22    |     US21    |     Visualización   de datos recibidos    |     Como usuario   inversionista, quisiera visualizar los datos pedidos en caso de haberse   aceptado mi solicitud para evaluarlos y utilizarlos en un análisis   financiero.    |     3    |
|     23    |     US22    |     Cierre de   solicitud    |     Como usuario   inversionista, quisiera visualizar los datos obtenidos hasta cerrar y marcar   como completada la solicitud para tener el tiempo necesario con los datos sin   comprometer a la empresa a la cual solicité.    |     3    |
|     24    |     US23    |     Seguridad de   entrega    |     Como usuario   contador financiero, quisiera entregar los datos solicitados sabiendo que se   realizará la entrega a través de un canal seguro para mantener la seguridad   de mi compañía.    |     5    |
|     25    |     US24    |     Limitación al   entregar datos    |     Como usuario   contador financiero, quisiera que no se permita descargar ni tomar captura de   pantalla de los datos compartidos para mantener la confidencialidad de la   empresa.    |     5    |
|     26    |     US26    |     Visualización   de análisis financieros disponibles    |     Como usuario   inversionista, quisiera visualizar los análisis financieros disponibles con   los datos que me entregaron para conocer si los datos solicitados fueron los   correctos.    |     2    |
|     27    |     US27    |     Eficacia de   los algoritmos de análisis financiero    |     Como usuario   inversionista, quisiera realizar cualquier análisis financiero disponible de   manera rápida y sencilla para agilizar el proceso de evaluación.    |     8    |
|     28    |     US28    |     conclusión   del análisis financiero    |     Como usuario   inversionista, quisiera recibir un veredicto en base a los análisis que se   realizaron con la aplicación para tener otra perspectiva sobre la evaluación.    |     8    |
|     29    |     US25    |     Alertas de   fugas de seguridad    |     Como usuario   contador financiero, quisiera recibir alertas de violaciones de seguridad   para informar a la empresa sobre el problema.    |     5    |
|     30    |     US05    |     Verificación   de cuenta empresa    |     Como usuario   contador financiero, quisiera que se me soliciten los datos de mi empresa   para verificar la fiabilidad de esta.    |     3    |
|     31    |     US06    |     Recuperación   de cuenta     |     Como usuario,   quisiera recuperar mi contraseña por medio del correo otorgado en caso de perderla   para recuperar el uso de la cuenta.    |     3    |
|     32    |     US08    |     Filtro de   empresas    |     Como usuario   inversionista, quisiera filtrar la lista de empresas disponibles para elegir   las que cumplan con los requisitos.    |     2    |
|     33    |     US09    |     Ordenamiento   de empresas    |     Como usuario   inversionista, quisiera ordenar la lista de empresas disponibles para elegir   las que cumplan con mis requisitos.    |     2    |
|     34    |     US10    |     Interfaz de   búsqueda sencilla    |     Como usuario   inversionista, quisiera una interfaz de búsqueda que permita un uso rápido y   efectivo para evitar utilizar mucho tiempo en la búsqueda.    |     2    |
|     35    |     US12    |     Filtro de   solicitudes    |     Como usuario   contador financiero, quisiera filtrar las solicitudes recibidas según   diferentes criterios para mantener un mayor orden.    |     2    |
|     36    |     US13    |     Ordenamiento   de solicitudes    |     Como usuario   contador financiero, quisiera ordenar las solicitudes recibidas según   diferentes criterios para mantener un mayor orden.    |     2    |
|     37    |     US16    |     Consulta de   orden de solicitud    |     Como usuario   inversionista, quisiera saber en qué puesto de atención me encuentro para   calcular cuándo volver a ingresar a la aplicación al recibir el estado de mi   solicitud    |     2    |
|     38    |     US17    |     Actualizaciones   sobre la solicitud    |     Como usuario   inversionista, quisiera recibir notificaciones sobre el estado de mi   solicitud para mantener un trabajo más organizado.    |     2    |
|     39    |     US19    |     Razón de la   respuesta otorgada    |     Como usuario   inversionista, quisiera recibir una explicación en caso de haberse rechazado   mi solicitud para confirmar si tal razón está bien o mal infundada.    |     2    |
|     40    |     US20    |     Creación de queja    |     Como usuario   inversionista, quisiera realizar una queja en caso se hayan entregado datos   erróneos para corregir el error realizado.    |     2    |

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
