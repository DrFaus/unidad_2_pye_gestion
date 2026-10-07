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

1. Diagramas de Venn y operaciones con eventos.
2. Probabilidad de eventos y probabilidad condicional.
3. Combinaciones y permutaciones.

---

## 1. Diagramas de Venn y operaciones con eventos

Los estudiantes trabajan con representaciones de dos y tres conjuntos.

Se practican conceptos como:

$$
A\cap B
$$

$$
A\cup B
$$

$$
A^c
$$

$$
A-B
$$

así como expresiones equivalentes a:

- sólo $A$;
- sólo $B$;
- $A$ y $B$;
- $A$ o $B$;
- ninguno;
- exactamente dos eventos;
- al menos uno;
- los tres eventos.

En los diagramas de tres conjuntos también se distinguen las regiones:

- sólo $A$;
- sólo $B$;
- sólo $C$;
- $A\cap B$, pero no $C$;
- $A\cap C$, pero no $B$;
- $B\cap C$, pero no $A$;
- $A\cap B\cap C$;
- ninguno de los tres.

## Diagramas para completar

Algunos reactivos presentan información global sobre varios eventos y solicitan completar las regiones faltantes del diagrama.

Por ejemplo, si se conoce:

$$
|A\cap B|=25
$$

y además:

$$
|A\cap B\cap C|=10
$$

entonces la región correspondiente a **A y B solamente** contiene:

$$
25-10=15
$$

Este tipo de ejercicio busca evitar que el estudiante confunda una intersección completa con una región exclusiva del diagrama.

Cuando un reactivo contiene varias casillas, el sistema puede otorgar **crédito parcial por las regiones correctamente determinadas**.

---

## 2. Probabilidad a partir de diagramas

Los diagramas también se utilizan para calcular probabilidades.

Si una encuesta contiene $N$ personas y una región determinada contiene $x$ observaciones, entonces:

$$
P(A)=\frac{x}{N}
$$

Los reactivos permiten practicar probabilidades como:

$$
P(A)
$$

$$
P(A\cap B)
$$

$$
P(A\cup B)
$$

$$
P(A^c)
$$

así como probabilidades asociadas a regiones específicas de diagramas de dos y tres conjuntos.

### Unión de dos eventos

Para dos eventos cualesquiera:

$$
P(A\cup B)=P(A)+P(B)-P(A\cap B)
$$

La intersección se resta porque, al sumar $P(A)$ y $P(B)$, los elementos pertenecientes a ambos eventos se cuentan dos veces.

---

## Probabilidad condicional

La práctica incluye problemas de probabilidad condicional basados principalmente en información representada mediante diagramas de Venn.

Se utiliza la relación:

$$
P(A\mid B)=\frac{P(A\cap B)}{P(B)}
$$

Una idea importante es que, al condicionar por $B$, el nuevo espacio de referencia está formado únicamente por los elementos de $B$.

Por ejemplo, si 40 clientes utilizan una aplicación móvil y 18 de ellos también participan en el programa de lealtad:

$$
P(\text{Lealtad}\mid\text{Aplicación})
=
\frac{18}{40}
=
0.45
$$

Por tanto, entre los clientes que utilizan la aplicación, el 45% pertenece también al programa de lealtad.

---

## Eventos mutuamente excluyentes

También se incluyen ejercicios donde dos eventos no pueden ocurrir simultáneamente.

Si $A$ y $B$ son mutuamente excluyentes:

$$
P(A\cap B)=0
$$

y, por tanto:

$$
P(A\cup B)=P(A)+P(B)
$$

Los diagramas correspondientes muestran conjuntos sin intersección para reforzar visualmente esta propiedad.

---

## 3. Combinaciones y permutaciones

Los problemas de combinatoria están planteados principalmente mediante situaciones contextualizadas.

La idea central que debe identificar el estudiante es:

> **¿El orden de los elementos seleccionados modifica el resultado?**

### Permutaciones

Se utilizan cuando **el orden importa**.

$$
P(n,r)=\frac{n!}{(n-r)!}
$$

donde:

- $n$ es el número total de elementos disponibles;
- $r$ es el número de elementos que se seleccionan y ordenan.

Por ejemplo:

> Una empresa reconocerá a los tres mejores vendedores entre ocho participantes, asignando primer, segundo y tercer lugar.

Los puestos son diferentes, por lo que el orden importa.

$$
P(8,3)=\frac{8!}{(8-3)!}
$$

$$
P(8,3)=\frac{8!}{5!}
$$

$$
P(8,3)=8(7)(6)=336
$$

Por tanto, existen:

$$
\boxed{336}
$$

formas distintas de asignar los tres lugares.

---

### Combinaciones

Se utilizan cuando **el orden no importa**.

$$
C(n,r)=\frac{n!}{r!(n-r)!}
$$

Por ejemplo:

> De ocho empleados se seleccionarán tres para integrar un comité.

Los mismos tres empleados forman el mismo comité independientemente del orden en que sean seleccionados.

$$
C(8,3)=\frac{8!}{3!5!}
$$

$$
C(8,3)=56
$$

Por tanto, pueden formarse:

$$
\boxed{56}
$$

comités diferentes.

---

## Evaluación de combinaciones y permutaciones

La aplicación **no exige que el estudiante escriba una notación específica** como:

`C(8,3)`

o

`P(8,3)`.

En los problemas contextualizados se solicita directamente el **número de formas posibles**.

Por ejemplo:

> De 10 candidatos se seleccionarán 4 para integrar un comité.  
> ¿Cuántos comités diferentes pueden formarse?

El estudiante debe determinar que el orden no importa y calcular:

$$
C(10,4)=210
$$

La respuesta que debe introducir es:

`210`

La retroalimentación posterior explica:

- si el orden importa;
- si corresponde combinación o permutación;
- la notación correspondiente;
- el procedimiento;
- el resultado.

De esta manera se evita penalizar al estudiante por escribir la notación de una forma distinta a la esperada por el programa.

---

## Factorial

La notación factorial se utiliza en las fórmulas de combinaciones y permutaciones.

Por ejemplo:

$$
5!=5(4)(3)(2)(1)=120
$$

Por definición:

$$
0!=1
$$

---

## Respuestas numéricas flexibles

En los reactivos de probabilidad, el sistema permite distintas formas equivalentes de expresar una respuesta.

Por ejemplo, si la respuesta correcta es:

$$
P(A)=0.25
$$

el estudiante puede introducir formas equivalentes como:

- `0.25`
- `.25`
- `25%`
- `1/4`

cuando el tipo de reactivo permite dichas representaciones.

En los ejercicios de combinaciones y permutaciones se compara directamente el **resultado numérico final**.

---

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

---

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

---

## Modo estudio

Al activar **Modo estudio**, el estudiante recibe retroalimentación después de responder.

La explicación puede indicar:

- el procedimiento correcto;
- qué región del diagrama debe utilizarse;
- por qué corresponde una combinación o una permutación;
- cómo se obtiene la probabilidad;
- qué error conceptual pudo haberse cometido.

Este modo permite utilizar la aplicación como herramienta de práctica y autoestudio.

---

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

---

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

El reporte puede guardarse como PDF utilizando la función de impresión del navegador.

---

## Tecnologías utilizadas

El proyecto está desarrollado únicamente con:

- HTML5;
- CSS;
- JavaScript;
- Canvas API.

No requiere frameworks ni bibliotecas externas.

Todo el proyecto se encuentra contenido en **un único archivo HTML**.

---

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

---

## Uso educativo

Esta herramienta está diseñada como apoyo para cursos introductorios de **Probabilidad y Estadística** en Gestión Empresarial.

Su finalidad es favorecer la interpretación de eventos, diagramas y situaciones probabilísticas antes que la memorización mecánica de fórmulas.

En particular, busca reforzar tres preguntas fundamentales:

1. **¿Qué representa cada región o evento?**
2. **¿Qué información necesito para calcular la probabilidad solicitada?**
3. **¿Importa o no importa el orden de los elementos seleccionados?**

---

## Autor

Material educativo desarrollado para la enseñanza de Probabilidad y Estadística.
