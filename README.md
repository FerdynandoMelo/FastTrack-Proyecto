# FastTrack - Plataforma Gastronómica Hiperlocal en Tiempo Real
**Asignatura:** Portafolio de Título
**Institución:** Duoc UC  
**Autor / Desarrollador:** Ferdynando Melo  
**Fecha de Cierre:** 05 de octubre de 2026 (Semana 8)  
**Metodología:** Scrum (Sprints I y II - 420 Story Points completados al 100%)

---

## Descripción del Proyecto

**FastTrack** es una solución multiplataforma orientada al rubro gastronómico de comida rápida y al paso. Su objetivo principal es resolver la incertidumbre de atención mediante un indicador operativo en tiempo real (**Live Status** conmutado por la cocina), georreferenciación interactiva en mapa (Leaflet API), cartas digitales dinámicas con control de inventario y un motor de gamificación comunitaria basado en calificaciones y canje transaccional de cupones de descuento.

---

## Estructura del Entregable y Organización de Archivos

El presente directorio consolida la documentación metodológica, técnica, esquemas relacionales, métricas en hojas de cálculo y la presentación ejecutiva del proyecto:

### 1. Carpetas de Soporte y Datos
* `Anexos/`: Contenedor de recursos visuales, diagramas de alta resolución (`mapa_mental.png`, `mapa_de_actores.png`, `vision_y_cuatro_pilares.png`, `impact_mapping.png`, `story_mapping.png`, tableros Scrum, Burndown Charts, Retrospectivas, Modelo Canvas y Carta Gantt).
* `Excel/`: Hojas de cálculo oficiales de estimación y seguimiento del proyecto (`01_Product_Backlog_Estimaciones.xlsx` y `02_Sprint_Backlog_Detallado.xlsx`).
* `Primera parte/`: Documentación histórica, actas de inicio y evidencias correspondientes a la fase de diagnóstico e ideación (Semanas 1 a 3).

---

### 2. Documentación Metodológica y Diseño de Software (Documentos Word)

#### Fase de Definición, Diagnóstico y Alcance
* `Definición Proyecto APT.docx`: Documento fundacional con la formulación inicial de la problemática, objetivos del software y marco de referencia.
* `Evidencia de Arquitectura y Requisitos de Software.docx`: Levantamiento de requerimientos funcionales, no funcionales y especificación de arquitectura modular híbrida.
* `01_Analisis_de_Caso_FastTrack.docx`: Análisis contextual del mercado de comida rápida y justificación técnica/económica de la solución.
* `02_Squad_y_Responsabilidades.docx`: Definición del equipo Scrum, distribución de roles y matriz de responsabilidades.
* `03_Mapa_Mental_Estructura.docx`: Desglose conceptual de problemas, usuarios y soluciones (soporte de `mapa_mental.png`).
* `04_Mapa_de_Actores_Estructura.docx`: Identificación y caracterización de stakeholders directos, indirectos y regulatorios.
* `05_Product_Goal_FastTrack.docx`: Definición del objetivo de largo plazo y el valor diferencial del producto.
* `06_Vision_y_Cuatro_Pilares.docx`: Los 4 pilares estratégicos de FastTrack: Grupo Objetivo, Necesidades, Producto y Valor.
* `07_Epicas_del_Sistema.docx`: Agrupación modular del backlog en 5 épicas de desarrollo (Seguridad, Gestión Operativa, Geolocalización, Gamificación y Validación).
* `08_Historias_de_Usuario_con_Criterios.docx`: Detalle de las 12 Historias de Usuario con formato estándar y criterios de aceptación (Gherkin: Given-When-Then).
* `09_Impact_Mapping_Estructura.docx`: Mapeo de impacto alineando metas de negocio con entregables funcionales.
* `10_Story_Mapping_Estructura.docx`: Mapa bidimensional del viaje del usuario (User Journey) y priorización por releases.

#### Fase de Gestión Ágil y Ciclos de Desarrollo (Sprints I y II)
* `11_Sprint_Planning_Sprints_I_y_II.docx`: Planificación detallada, capacidad del equipo y compromisos de alcance (140 pts en Sprint I / 280 pts en Sprint II).
* `12_Scrum_Boards_Estructura.docx`: Estado y evolución de los tableros Kanban en cada fase (To Do, In Progress, Testing, Done).
* `13_Burndown_Charts_Estructura.docx`: Datos tabulares de reducción de esfuerzo ideal vs. real para ambos ciclos.
* `14_Daily_Meetings_Consolidado.docx`: Registro sistemático de sincronizaciones diarias (ayer, hoy e impedimentos).
* `15_Sprint_Review_Consolidado.docx`: Informes de demostración de incrementos de software potencialmente desplegables ante stakeholders.
* `16_Retrospective_Sprint_Consolidado.docx`: Análisis de mejora continua (Keep, Sad, Try) para ambos sprints.

#### Cierre Técnico, Aseguramiento de Calidad y Reportabilidad
* `17_Reporte_de_Sprints_Scrum_Definition_of_Done.docx`: Estándares de calidad y criterios técnicos requeridos para el cierre de tareas (DoD).
* `18_Reporte_de_Sprints_Scrum_Impediment_Log.docx`: Bitácora de incidencias técnicas (IMP-01 a IMP-04), análisis de impacto y acciones correctivas aplicadas.
* `19_Informe_Tecnico_Consolidado_Final_Semana_8.docx`: Dossier técnico final integrando arquitectura, modelo DDL, triggers, procedimientos y conclusiones de ingeniería.

---

### 3. Base de Datos, Presentación y Enlaces
* `SCRIPT SQL - BBDD.txt`: Script relacional normalizado en 3FN para SQLite/SQL estructurado con llaves primarias, foráneas, constraints (`CHECK`), Triggers de reputación/puntos (`TR_NUEVA_VALORACION`) y Stored Procedures atómicos de canje (`SP_CANJEAR_CUPON`).
* `Presentación FastTrack.pptx`: Presentación ejecutiva oficial de 15 diapositivas estructurada para la defensa de título de 5 a 7 minutos.
* `Links del proyecto.txt`: Enlaces directos a los repositorios de control de versiones (Git), despliegues web o tableros de gestión externa.

---

## Tecnologías Empleadas

* **Frontend:** Ionic Framework, Angular, TypeScript, SCSS, HTML5.
* **Componentes de Mapa:** Leaflet API, OpenStreetMap.
* **Persistencia Local:** SQLite (nativo móvil) con fallback reactivo en Ionic Storage (IndexedDB) para navegadores.
* **Seguridad:** JSON Web Tokens (JWT), Hashing seguro con BCrypt, Angular Route Guards.
* **Gestión y Control Ágil:** Marco de trabajo Scrum, Trello, Git/GitHub.
