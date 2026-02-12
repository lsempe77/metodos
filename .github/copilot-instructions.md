# Instrucciones para la producción de contenido del libro

## Sobre el libro

**Título:** (Otro) Manual de metodología de la investigación en ciencias sociales
**Subtítulo:** Algo políticamente incorrecto y con un énfasis en lo cuantitativo
**Autor:** Lucas Sempé
**Formato:** Quarto Book (.qmd)
**Idioma:** Español latinoamericano

---

## Tono y voz

### Personalidad del autor
- **Directo y sin rodeos.** No se anda con formalidades. Dice las cosas como son, incluso cuando incomodan.
- **Irreverente pero riguroso.** Se burla de las convenciones vacías, pero respeta profundamente el método. El humor es una herramienta pedagógica, no un escape del rigor.
- **Honesto sobre el caos.** Reconoce abiertamente que investigar es desordenado, frustrante y no lineal. No romantiza el proceso ni lo simplifica.
- **Provocador con propósito.** Cuestiona las posturas del lector (y las propias) para generar reflexión, no para ofender.
- **Anti-tribal.** Crítico del sesgo de confirmación, la prédica entre apóstoles, y la investigación que solo confirma lo que ya se cree.

### Registro lingüístico
- Informal pero no descuidado. Se habla como en una conversación inteligente entre colegas, no como en un congreso ni como en un bar.
- Se usa el "tú" (no "usted" ni "ustedes" formal).
- Se permiten expresiones coloquiales latinoamericanas cuando aportan: "no paga mal", "si la burocracia no te mata", "poner el carro delante de los caballos".
- Se usa el masculino genérico siguiendo la norma RAE. Esto está explícitamente justificado en el capítulo 1.
- **NO** se usa lenguaje inclusivo con "x", "e", ni barras (a/o).
- Se evitan muletillas académicas vacías: "cabe destacar que", "es menester señalar", "en el marco de lo anterior".

### Lo que se busca generar en el lector
1. Que se ría (o al menos sonría) mientras aprende.
2. Que se sienta incómodo con sus propios supuestos.
3. Que entienda conceptos complejos a través de ejemplos concretos y cotidianos.
4. Que termine cada capítulo con ganas de aplicar lo aprendido.
5. Que no sienta que está leyendo un manual, sino teniendo una conversación con alguien que sabe del tema y lo dice sin filtros.

---

## Lógica de producción del texto

### Estructura de cada capítulo

1. **Apertura provocadora.** Empezar con una afirmación fuerte, una pregunta incómoda, o un mito a destruir. Nunca empezar con "En este capítulo veremos..."
2. **Desarrollo con ejemplos reales.** Cada concepto abstracto debe aterrizarse con un ejemplo concreto, preferiblemente latinoamericano. Los ejemplos deben ser reconocibles, no de manual.
3. **Errores señalados explícitamente.** En cada tema, mostrar qué se hace mal y por qué. Usar formato ❌/✅ cuando sea útil.
4. **Conexión con otros capítulos.** El libro es un argumento continuo, no capítulos aislados. Hacer referencias cruzadas cuando corresponda.
5. **Ejercicio práctico al final.** Cada capítulo termina con un ejercicio accionable que el lector puede hacer con su propia investigación. Usar callout `:::{.callout-tip}`.
6. **Callouts de Quarto** para notas importantes, advertencias y reflexiones. Tipos: `.callout-tip` (ejercicios), `.callout-note` (para recordar), `.callout-important` (reflexiones), `.callout-warning` (advertencias/errores graves).

### Principios de escritura

- **Una idea por párrafo.** Si cambias de idea, abre párrafo nuevo.
- **Frases cortas.** Si una frase tiene más de 3 líneas, probablemente hay que cortarla.
- **Listas y tablas para comparar.** Cuando hay opciones, tipos o categorías, usar tablas o listas en lugar de párrafos densos.
- **Negrita para conceptos clave** la primera vez que aparecen.
- **Cursiva para énfasis** retórico o para títulos de libros.
- **No abusar de las citas textuales.** Parafrasear es mejor. Reservar las citas textuales para frases que pierden fuerza al parafrasearlas.
- **Citas bibliográficas con @clave** (formato Quarto/Pandoc), referenciadas en `book.bib`.

### Qué NO hacer

- No escribir como manual académico tradicional (seco, formal, distante).
- No simplificar hasta el punto de ser impreciso. El lector merece rigor.
- No asumir que el lector sabe jerga metodológica. Explicar cada término la primera vez.
- No ser condescendiente. Informal no es lo mismo que infantil.
- No usar ejemplos exclusivamente del mundo anglosajón. Priorizar América Latina y el mundo hispanohablante.
- No repetir lo que ya dicen todos los manuales de la misma forma. Si la explicación convencional funciona, buscar un ángulo fresco para presentarla.
- No incluir bloques de código R salvo que el capítulo lo requiera explícitamente para demostrar algo (visualización, análisis).

### Hilo argumental del libro

El libro tiene un meta-argumento que atraviesa todos los capítulos:

> **La investigación en ciencias sociales requiere honestidad intelectual: con tus datos, con tus sesgos, con tus limitaciones, y con tu lector.**

Todo el contenido debe volver a esta idea de alguna forma:
- Los paradigmas exigen honestidad sobre tus supuestos.
- La pregunta exige honestidad sobre lo que realmente no sabes.
- El método exige honestidad sobre lo que puedes y no puedes hacer.
- Los resultados exigen honestidad sobre lo que encontraste (no lo que querías encontrar).
- La escritura exige honestidad sobre lo que sabes y lo que no.

### Contexto del lector objetivo

- Estudiantes de pregrado y posgrado en ciencias sociales en América Latina.
- Personas que encuentran aburrida la metodología (y tienen razón, tal como se suele enseñar).
- Investigadores junior que quieren mejorar su práctica.
- Gente curiosa que quiere entender cómo funciona la producción de conocimiento.

---

## Configuración técnica

- **Formato:** Quarto Book (`.qmd`)
- **Configuración central:** `_quarto.yml`
- **Bibliografía:** `book.bib` (formato BibTeX), citar con `@clave`
- **Estilo de cita:** APA (usar archivo CSL si es necesario)
- **Idioma del proyecto:** `lang: es` en `_quarto.yml`
- **Output:** HTML (principal), PDF y EPUB (secundarios)
- **CSS personalizado:** `style.css`
- **LaTeX header:** `preamble.tex` (para PDF)
