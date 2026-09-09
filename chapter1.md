## Capítulo 1
## 1.1. Startup Profile

### 1.1.1. Descripción de la Startup
**NexusLibre** es una startup tecnológica emergente conformada por estudiantes de la carrera de Ingeniería de Software de la Universidad Peruana de Ciencias Aplicadas (UPC). Nos enfocamos en diseñar, desarrollar y desplegar soluciones de software de código abierto (Open Source) escalables, accesibles y orientadas a servicios. Nuestro propósito es resolver problemáticas reales del sector logístico de cadena de suministro mediante productos digitales innovadores y sostenibles. Trabajamos bajo un entorno ágil y colaborativo, aplicando estándares de calidad de la industria para garantizar una comunicación efectiva y el cumplimiento de los objetivos técnicos y de negocio.

### 1.1.2. Perfiles de integrantes del equipo

| Foto                              | Nombres y Apellidos   | Código   | Carrera   | Conocimientos y Habilidades                                                                                                    |
| :-------------------------------: | :-------------------- | :------- | :-------- | :----------------------------------------------------------------------------------------------------------------------------- |
| ![Foto](assets/images/perfil.jpg) | Emanuel Renato Checalla Apaza | [Código] | [Carrera] | [Redactar párrafo resumen indicando principales conocimientos técnicos y habilidades que puede aportar en el equipo]           |
| ![Foto](assets/images/perfil.jpg) | Fabricio Jofred Lozano Quispe | [Código] | [Carrera] | [Redactar párrafo resumen indicando principales conocimientos técnicos y habilidades que puede aportar en el equipo]           |
| ![Foto](assets/images/chapter1/Perfil_Gabriel.jpeg) | Gabriel Augusto Peñaranda Caldas | U202210836 | Ingeniería de Software | Me apasiona la infraestructura tecnológica, me destaaco en conocimiento de sistemas operativos, Cloud infrastructure y cloud architecture, manejo bien el lenguaje de JS para frontend y backend           |
| ![Foto](assets/images/perfil.jpg) | Maria Jose Pezo Castilla | [Código] | [Carrera] | [Redactar párrafo resumen indicando principales conocimientos técnicos y habilidades que puede aportar en el equipo]           |
| ![Foto](assets/images/perfil.jpg) | Rodrigo Matias Vite Celis | [Código] | [Carrera] | [Redactar párrafo resumen indicando principales conocimientos técnicos y habilidades que puede aportar en el equipo]           |


## 1.2. Solution Profile

### 1.2.1. Antecedentes y problemática

**Técnica 5W2H**

Para comprender la raíz y el impacto de la problemática de los fletes vacíos en el sector logístico, aplicamos la técnica de las 5 'W's y 2 'H's:

* **Who (Quién):** El problema lo padecen de forma directa los transportistas independientes que llevan carga y los empresarios dueños de flotas de camiones, conformando ambos nuestros principales segmentos objetivo.

* **What (Qué):** Los vehículos de transporte de carga se ven obligados a realizar sus viajes de retorno completamente vacíos tras finalizar una entrega.

* **Where (Dónde):** El alcance geográfico de esta problemática se experimenta a nivel del departamento de Lima.

* **When (Cuándo):** Ocurre sistemáticamente en la actualidad, justo en el momento en que inicia el trayecto de regreso, generando en el conductor la frustración de estar realizando un viaje improductivo.

* **Why (Por qué):** Surge por la alta complejidad logística que implica coordinar a un vendedor cerca del punto de entrega inicial con un comprador cercano al destino final, agravado por la ausencia de una red de contactos sólida.

* **How (Cómo se soluciona hoy):** En la actualidad, los afectados intentan mitigar la situación buscando contactos de manera rudimentaria fuera de marcos tecnológicos; sin embargo, en la gran mayoría de los casos, el problema simplemente se ignora y se asume la pérdida.

* **How Much (Cuánto):** A pesar de existir un ligero ahorro de combustible al viajar sin carga, la ineficiencia representa una pérdida aproximada del 30% de rentabilidad. Además, este modelo genera un incremento innecesario en la huella de carbono y encarece significativamente los precios finales de los productos en el mercado.


**Descripción de los antecedentes**

**Enunciado del Problema**

Los transportistas y empresarios de flotas en el departamento de Lima enfrentan una pérdida de hasta el 30% en su rentabilidad y generan una excesiva huella de carbono debido a la alta complejidad logística y la falta de herramientas tecnológicas para conectar con redes de contactos confiables que les permitan aprovechar sus viajes de retorno (fletes vacíos).


**Descripción de la problemática**

**Puntos Clave a Resolver**

* **Reducción de la fricción logística:** Automatizar el emparejamiento entre transportistas con capacidad disponible y usuarios (vendedores/compradores) que necesitan enviar carga.

* **Digitalización de la red de contactos:** Trasladar la búsqueda rudimentaria de oportunidades a un ecosistema tecnológico centralizado y accesible.

* **Optimización operativa y ambiental:** Maximizar la productividad de cada viaje, mitigando el impacto económico en los precios de los productos y reduciendo la emisión innecesaria de carbono.

**Objetivos**

* Diseñar e implementar una plataforma digital que conecte eficientemente la oferta y demanda de fletes en Lima.

* Trazar rutas precisas en tiempo real para optimizar el recorrido logístico entre los puntos de recojo y entrega.

**Restricciones y Alcance**

* **Gestión de Pagos:** La plataforma no actuará como pasarela de pagos. No se procesarán transacciones económicas entre clientes, transportistas, vendedores o compradores; la negociación financiera se realizará estrictamente por fuera del sistema.

* **Conectividad:** Es un requisito indispensable contar con conexión a internet ininterrumpida para acceder a la red de proveedores y compradores.

* **Geolocalización:** El sistema requiere obligatoriamente tener la ubicación del dispositivo activada para el trazado de rutas y seguimiento en tiempo real.


**Propuesta Tecnológica (Trazza)**

Para hacer frente a esta problemática, NexusLibre presenta **Trazza**, una plataforma logística inteligente estructurada sobre una arquitectura en la nube (AWS). El sistema está desarrollado con un backend robusto en Java (Spring Boot) y un frontend web dinámico en TypeScript (Angular).

El núcleo logístico de Trazza se potencia mediante algoritmos computacionales de optimización (como Backtracking, Dijkstra, TSP y BFS) para evaluar capacidades de peso, trazar rutas eficientes y generar matrices de costos.

Además, el producto integra motores de Inteligencia Artificial avanzada para automatizar el emparejamiento (*matchmaking*) entre compradores y vendedores, analizando variables históricas y de proximidad para asignar la carga ideal al camión adecuado sin esfuerzo manual.

A nivel de escalabilidad, Trazza contempla la integración de ecosistemas IoT (Internet de las Cosas) en las flotas para monitorear el estado físico de la carga en tránsito, sumado a un sistema de seguimiento GPS por hardware que garantiza la trazabilidad continua del vehículo y la mercancía, incluso en trayectos donde la conexión a internet sea intermitente o nula.

### 1.2.2. Lean UX Process

#### 1.2.2.1. Lean UX Problem Statements

#### 1.2.2.2. Lean UX Assumptions

#### 1.2.2.3. Lean UX Hypothesis Statements

#### 1.2.2.4. Lean UX Canvas

## 1.3. Segmentos objetivo
