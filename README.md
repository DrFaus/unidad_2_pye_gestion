# Práctica interactiva de probabilidad, diagramas de Venn y combinatoria

Aplicación web educativa para practicar conceptos básicos de **probabilidad, diagramas de Venn, combinaciones y permutaciones**, desarrollada como material de apoyo para estudiantes de **Gestión Empresarial**.

La herramienta está diseñada para que el estudiante interprete situaciones contextualizadas, identifique correctamente eventos y regiones de un diagrama de Venn, calcule probabilidades y utilice combinaciones o permutaciones cuando corresponda.

El objetivo no es desarrollar combinatoria avanzada, sino reforzar el razonamiento probabilístico y la interpretación correcta de la información.

## Características principales

- Banco de **194 reactivos**.
- **10 preguntas aleatorias por intento**.
- Selección balanceada entre los distintos temas.
- Respuestas directas, sin depender principalmente de opción múltiple.
- Diagramas de Venn de:
  - dos conjuntos;
  - tres conjuntos;
  - eventos con intersección;
  - eventos mutuamente excluyentes.
- Ejercicios para **completar regiones de diagramas de Venn**.
- Problemas de probabilidad condicional.
- Problemas de unión, intersección, complemento y eventos exclusivos.
- Problemas contextualizados de combinaciones y permutaciones.
- **Modo estudio** con retroalimentación inmediata.
- Opción para repasar únicamente los errores.
- Generación de reporte imprimible y exportable como PDF.
- Funciona completamente **offline**.
- Desarrollado en un único archivo HTML.
- Sin librerías externas.

## Contenido

La práctica se organiza en tres grandes bloques:

### 1. Diagramas de Venn y operaciones con eventos

Los estudiantes trabajan con representaciones de dos y tres conjuntos.

Se practican conceptos como:

\[
A\cap B
\]

\[
A\cup B
\]

\[
A^c
\]

\[
A-B
\]

así como expresiones equivalentes a:

- sólo A;
- sólo B;
- A y B;
- A o B;
- ninguno;
- exactamente dos eventos;
- al menos uno;
- los tres eventos.

En los diagramas de tres conjuntos también se distinguen las regiones:

- sólo A;
- sólo B;
- sólo C;
- A y B solamente;
- A y C solamente;
- B y C solamente;
- A, B y C;
- ninguno de los tres.

## Diagramas para completar

Algunos reactivos presentan información global sobre varios eventos y solicitan completar las regiones faltantes del diagrama.

Por ejemplo, si se conoce:

\[
|A\cap B|=25
\]

y

\[
|A\cap B\cap C|=10,
\]

entonces la región correspondiente a **A y B solamente** contiene:

\[
25-10=15.
\]

Este tipo de ejercicio busca evitar que el estudiante confunda una intersección completa con una región exclusiva del diagrama.

Cuando un reactivo contiene varias casillas, el sistema puede otorgar **crédito parcial por las regiones correctamente determinadas**.

## Probabilidad a partir de diagramas

Los diagramas también se utilizan para calcular probabilidades.

Si una encuesta contiene \(N\) personas y una región determinada contiene \(x\) observaciones:

\[
P(A)=\frac{x}{N}.
\]

Los reactivos permiten practicar probabilidades como:

\[
P(A)
\]

\[
P(A\cap B)
\]

\[
P(A\cup B)
\]

\[
P(A^c)
\]

y otras regiones observables directamente en los diagramas.

## Probabilidad condicional

La práctica incluye problemas de probabilidad condicional basados principalmente en información representada mediante diagramas de Venn.

Se utiliza la relación:

\[
P(A\mid B)=\frac{P(A\cap B)}{P(B)}.
\]

Una idea importante es que, al condicionar por \(B\), el nuevo espacio de referencia está formado únicamente por los elementos de \(B\).

Por ejemplo, si 40 clientes utilizan una aplicación y 18 de ellos también utilizan un programa de lealtad:

\[
P(\text{Lealtad}\mid\text{Aplicación})
=
\frac{18}{40}
=
0.45.
\]

## Eventos mutuamente excluyentes

También se incluyen ejercicios donde dos eventos no pueden ocurrir simultáneamente.

Si A y B son mutuamente excluyentes:

\[
P(A\cap B)=0
\]

y, por tanto:

\[
P(A\cup B)=P(A)+P(B).
\]

Los diagramas correspondientes muestran conjuntos sin intersección para reforzar visualmente esta propiedad.

## Combinaciones y permutaciones

Los problemas de combinatoria están planteados principalmente mediante situaciones contextualizadas.

### Permutaciones

Se utilizan cuando **el orden importa**.

\[
P(n,r)=\frac{n!}{(n-r)!}
\]

Ejemplo:

> Una empresa reconocerá a los tres mejores vendedores entre ocho participantes, asignando primer, segundo y tercer lugar.

Como los puestos son diferentes, importa quién ocupa cada posición:

\[
P(8,3)=336.
\]

### Combinaciones

Se utilizan cuando **el orden no importa**.

\[
C(n,r)=\frac{n!}{r!(n-r)!}
\]

Ejemplo:

> De ocho empleados se seleccionarán tres para integrar un comité.

Los mismos tres empleados forman el mismo comité independientemente del orden en que se seleccionen:

\[
C(8,3)=56.
\]

## Evaluación de combinaciones y permutaciones

La aplicación **no exige que el estudiante escriba una notación específica** como:

`C(8,3)`

o

`P(8,3)`.

En los problemas contextualizados se solicita directamente el **número de formas posibles**.

El estudiante debe decidir por su cuenta si la situación corresponde a una combinación o una permutación y realizar el cálculo.

La retroalimentación posterior sí explica:

- si el orden importa;
- si se utiliza combinación o permutación;
- la notación correspondiente;
- el cálculo realizado.

De esta manera se evita penalizar diferencias de escritura y se evalúa principalmente el razonamiento y el resultado.

## Respuestas numéricas flexibles

En los reactivos de probabilidad, el sistema permite distintas formas equivalentes de expresar una respuesta.

Por ejemplo, una probabilidad de:

\[
0.25
\]

puede introducirse como:

- `0.25`
- `.25`
- `25%`
- `1/4`

cuando el tipo de reactivo permite dichas representaciones.

## Contextos utilizados

Los ejercicios están orientados principalmente a situaciones relacionadas con **Gestión Empresarial**, entre ellas:

- clientes;
- canales de venta;
- métodos de pago;
- satisfacción del cliente;
- campañas de marketing;
- selección de personal;
- comités de trabajo;
- capacitación;
- proveedores;
- auditorías;
- promociones;
- zonas comerciales;
- productos;
- desempeño de vendedores;
- beneficios empresariales;
- servicios utilizados por los clientes;
- indicadores administrativos.

El propósito es que los ejercicios se perciban como pequeñas situaciones que podrían presentarse en el ámbito empresarial y no únicamente como cálculos abstractos.

## Estructura de cada intento

Cada intento contiene **10 reactivos** seleccionados aleatoriamente del banco.

La selección se controla para mantener variedad entre:

- combinaciones;
- permutaciones;
- diagramas de Venn de dos conjuntos;
- diagramas de Venn de tres conjuntos;
- cálculo de probabilidades;
- probabilidad condicional;
- eventos mutuamente excluyentes;
- interpretación de regiones;
- ejercicios de llenado de diagramas.

El objetivo es evitar que un intento quede concentrado únicamente en un tipo de ejercicio.

## Modo estudio

Al activar **Modo estudio**, el estudiante recibe retroalimentación después de responder.

La explicación indica brevemente:

- el procedimiento correcto;
- qué región del diagrama debe utilizarse;
- por qué corresponde una combinación o permutación;
- cómo se obtiene la probabilidad;
- qué error conceptual pudo haberse cometido.

## Modo de evaluación

Con el modo estudio desactivado, las respuestas no se califican inmediatamente.

El estudiante completa las 10 preguntas y posteriormente selecciona:

**Calificar intento**

La aplicación muestra entonces:

- número de respuestas correctas;
- porcentaje obtenido;
- desempeño por tema;
- respuestas correctas e incorrectas;
- explicaciones.

## Reporte

Después de calificar un intento puede generarse un reporte que incluye:

- nombre del estudiante;
- fecha;
- número de intento;
- calificación;
- reactivos presentados;
- respuestas proporcionadas;
- respuestas correctas;
- explicaciones;
- diagramas utilizados.

El reporte puede guardarse como PDF mediante la función de impresión del navegador.

## Tecnologías utilizadas

El proyecto está desarrollado únicamente con:

- HTML5;
- CSS;
- JavaScript;
- Canvas API.

No requiere frameworks ni bibliotecas externas.

Todo el proyecto se encuentra contenido en **un único archivo HTML**.

## Ejecución

No requiere instalación.

1. Descargar el archivo HTML.
2. Abrirlo con un navegador moderno.
3. Escribir el nombre del estudiante.
4. Resolver las 10 preguntas.
5. Seleccionar **Calificar intento**.
6. Revisar la retroalimentación.
7. Opcionalmente generar el reporte en PDF.
8. Generar un nuevo intento para obtener una combinación diferente de reactivos.

## Uso educativo

Esta herramienta está diseñada como apoyo para cursos introductorios de **Probabilidad y Estadística** en Gestión Empresarial.

Su finalidad es favorecer la interpretación de eventos, diagramas y situaciones probabilísticas antes que la memorización mecánica de fórmulas.

En particular, busca reforzar tres preguntas fundamentales:

1. **¿Qué representa cada región o evento?**
2. **¿Qué información necesito para calcular la probabilidad solicitada?**
3. **¿Importa o no importa el orden de los elementos seleccionados?**

## Autor

Material educativo desarrollado para la enseñanza de Probabilidad y Estadística.
