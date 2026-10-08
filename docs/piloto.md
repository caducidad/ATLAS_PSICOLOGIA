# Piloto del Atlas de la Psicología

Borrador 0.1 · 8 de octubre de 2026

Propuesta de contenido para el primer piloto. No depende del esquema base del núcleo: fija qué entra y cómo se organiza; el formato de los datos llegará con `docs/esquema-base.md` de ATLAS_NUCLEO.

**Aviso de rigor.** Fechas, cifras y estados de la evidencia de este borrador son una primera propuesta. Cada uno se comprueba en la fuente al redactar la ficha, igual que en el Atlas de la Filosofía.

## 1. Alcance del piloto: un corte vertical

El piloto de filosofía fue un **corte horizontal**: una época, la Antigüedad, completa. Para psicología se propone un **corte vertical**: el canon (círculo 1 y algo del 2) a lo largo de toda la historia de la disciplina, unos 150 años.

Por qué:

- La historia de la psicología es corta; un solo periodo dejaría el mapa casi vacío.
- El estado de la evidencia, lo más propio de este atlas, solo se entiende viendo la historia entera: un experimento de 1971 se juzga con las réplicas de 2015.
- La vista cronológica y los carriles por escuela se pueden probar desde el principio.

Tamaño orientativo: unos 140 nodos (5 contextos, 14 temáticas, 10 escuelas, unos 40 autores, unos 25 experimentos, unos 30 conceptos y teorías, una docena de obras).

## 2. Periodos

Un archivo por periodo; cada uno es también un nodo `contexto`. Los límites son convenciones historiográficas y se dan como horquilla.

| Archivo | Contexto | Horquilla | Prefijo de relaciones | De qué trata |
| --- | --- | --- | --- | --- |
| `precursores.json` | Precursores | hasta 1879 | `pre-` | Raíces filosóficas (puentes al Atlas de la Filosofía) y fisiológicas: psicofísica, localización cerebral, evolución, diferencias individuales |
| `fundacion.json` | La fundación | 1879 – c. 1913 | `fun-` | Laboratorio de Wundt en Leipzig (1879), estructuralismo y funcionalismo, primeras leyes del aprendizaje y la memoria, nacimiento del psicoanálisis y de los tests |
| `grandes-escuelas.json` | Las grandes escuelas | c. 1913 – c. 1956 | `esc-` | Manifiesto conductista de Watson (1913), Gestalt, neoconductismo, expansión del psicoanálisis, Piaget y Vygotski |
| `revolucion-cognitiva.json` | Revolución cognitiva y humanismo | c. 1956 – c. 1980 | `cog-` | Simposio del MIT (1956), crítica de Chomsky a Skinner, humanismo, edad de oro de la psicología social, apego, sesgos y heurísticos |
| `contemporanea.json` | Psicología contemporánea | c. 1980 – hoy | `con-` | Neurociencia cognitiva, psicología positiva y evolucionista, crisis de replicación y ciencia abierta |

## 3. Temáticas

Catorce, como en filosofía, para mantener la simetría de la colección:

1. Historia y métodos de investigación
2. Psicobiología
3. Sensación y percepción
4. Atención y conciencia
5. Aprendizaje
6. Memoria
7. Pensamiento, lenguaje y decisión
8. Inteligencia
9. Emoción y motivación
10. Desarrollo
11. Personalidad y diferencias individuales
12. Psicología social
13. Psicopatología
14. Psicoterapia e intervención

Las dos últimas se tratan **desde la historia de las ideas** (qué propuso cada corriente y con qué pruebas), no como orientación clínica. El lado clínico como tal sigue aparcado.

## 4. Escuelas y corrientes (carriles de la vista cronológica)

| Escuela | Naturaleza | Notas |
| --- | --- | --- |
| Estructuralismo | rótulo historiográfico | Nombre de Titchener para su programa; se aplica también, con matices, a Wundt |
| Funcionalismo | rótulo historiográfico | James, Dewey, Angell; más un clima que una escuela |
| Psicoanálisis | real | Asociación Psicoanalítica Internacional desde 1910 |
| Psicología analítica e individual | real | Escisiones de Jung y Adler; ¿carril propio o dentro de psicoanálisis? |
| Conductismo | real / rótulo | Watson, luego el neoconductismo de Skinner, Tolman y Hull |
| Gestalt | real | Escuela de Berlín: Wertheimer, Köhler, Koffka |
| Psicología sociocultural | rótulo historiográfico | Vygotski y su escuela |
| Humanismo | real | «Tercera fuerza»: Maslow, Rogers |
| Cognitivismo | rótulo historiográfico | Miller, Neisser, Bruner, Simon |
| Neurociencia cognitiva | rótulo historiográfico | Desde los años ochenta |

Carril «otros» para quien no encaja en ninguna (Piaget, buena parte de la psicología social).

## 5. Autores

Círculo 1 en **negrita**. `filosofia:` indica un puente: la figura vive en el Atlas de la Filosofía y aquí solo se referencia.

| Periodo | Autores |
| --- | --- |
| Precursores | filosofia:Aristóteles, filosofia:Descartes, filosofia:Locke, filosofia:Hume · **Fechner**, Weber, Helmholtz, Broca, Darwin, Galton |
| Fundación | **Wundt**, **William James**, **Ebbinghaus**, **Pávlov**, **Thorndike**, **Freud**, **Binet**, Titchener, Stanley Hall |
| Grandes escuelas | **Watson**, **Wertheimer**, Köhler, Koffka, **Skinner**, Tolman, **Piaget**, **Vygotski**, **Jung**, Adler, Anna Freud, Melanie Klein, Lewin, Bartlett |
| Revolución cognitiva | **George Miller**, Chomsky, Neisser, Bruner, **Maslow**, **Rogers**, **Bandura**, **Asch**, **Milgram**, **Festinger**, **Bowlby**, Ainsworth, Beck, Ellis, **Kahneman**, **Tversky**, Mischel, Zimbardo, Loftus, Seligman, Darley, Latané |
| Contemporánea | Damasio, Gardner, Baumeister, Nosek |

Pendiente: los puentes a Descartes, Locke y Hume apuntan a fichas que el Atlas de la Filosofía aún no tiene (su piloto es la Antigüedad). Mientras tanto, el validador avisará sin dar error. Hay que decidir también el atlas «de casa» de William James (psicología o filosofía) y de Chomsky (no hay atlas de lingüística).

## 6. Experimentos y estudios

★ marca los imprescindibles del piloto. El estado se refiere al **hallazgo** que el experimento pone a prueba (ver la escala en el apartado 7). «Ética» señala estudios hoy inadmisibles o muy discutidos por su trato a los participantes.

| | Experimento | Año | Investigadores | Estado propuesto | Ética |
| --- | --- | --- | --- | --- | --- |
| | Caso Phineas Gage | 1848 | Harlow (médico) | matizado: los relatos posteriores exageraron el cambio de personalidad | |
| ★ | Curva del olvido | 1885 | Ebbinghaus | consolidado | |
| ★ | Condicionamiento clásico | c. 1897–1903 | Pávlov | consolidado | |
| ★ | Cajas problema y ley del efecto | 1898 | Thorndike | consolidado | |
| | Fenómeno phi | 1912 | Wertheimer | consolidado | |
| ★ | El pequeño Albert | 1920 | Watson y Rayner | no replicado | Sí |
| | Aprendizaje latente | 1930 | Tolman y Honzik | consolidado | |
| | Efecto Stroop | 1935 | Stroop | consolidado | |
| ★ | Conformidad (líneas) | 1951 | Asch | matizado | |
| | Cueva de los Ladrones | 1954 | Sherif | en debate | Sí |
| | Paciente H. M. | 1957 | Scoville y Milner | consolidado | |
| ★ | Madres de alambre y de felpa | 1958 | Harlow | consolidado | Sí |
| ★ | Disonancia cognitiva (1 dólar frente a 20) | 1959 | Festinger y Carlsmith | en debate | |
| | Memoria icónica | 1960 | Sperling | consolidado | |
| ★ | Muñeco Bobo | 1961 | Bandura, Ross y Ross | matizado | |
| ★ | Obediencia a la autoridad | 1961–1963 | Milgram | matizado | Sí |
| | Indefensión aprendida | 1967 | Seligman y Maier | matizado: reinterpretado por sus propios autores en 2016 | Sí |
| ★ | Efecto espectador | 1968 | Darley y Latané | consolidado | |
| | Efecto Pigmalión | 1968 | Rosenthal y Jacobson | en debate | |
| ★ | Situación extraña | 1970 | Ainsworth y Bell | matizado | |
| ★ | Prisión de Stanford | 1971 | Zimbardo | desacreditado | Sí |
| | Malvavisco | 1972 | Mischel | en debate | |
| | «Cuerdos en lugares de locos» | 1973 | Rosenhan | en debate | Sí |
| ★ | Reconstrucción del recuerdo (accidente de coche) | 1974 | Loftus y Palmer | consolidado | |
| | Efecto marco (la «enfermedad asiática») | 1981 | Tversky y Kahneman | consolidado | |
| | Experimento de Libet | 1983 | Libet | en debate (sobre todo su interpretación) | |
| ★ | Agotamiento del yo | 1998 | Baumeister y otros | no replicado | |
| | Poses de poder | 2010 | Carney, Cuddy y Yap | no replicado | |
| ★ | Proyecto de Reproducibilidad | 2015 | Open Science Collaboration | consolidado | |

Fuentes que sostienen los estados más delicados, por comprobar al redactar: réplica de Ebbinghaus (Murre y Dros, 2015); réplica parcial de Milgram (Burger, 2009) y archivos (Perry, 2013); críticas a Stanford (Le Texier, 2018); réplica multilaboratorio de la disonancia por complacencia inducida (Vaidis y otros, 2024); seguimiento del malvavisco (Watts, Duncan y Quan, 2018); investigación sobre Rosenhan (Cahalan, 2019); réplica multilaboratorio del agotamiento del yo (Hagger y otros, 2016); poses de poder (Ranehill y otros, 2015); revisión de la indefensión aprendida (Maier y Seligman, 2016); Cueva de los Ladrones (Perry, 2018); metaanálisis del efecto espectador (Fischer y otros, 2011).

## 7. Estado de la evidencia: escala propuesta

Campo `estadoEvidencia` del nodo (teoría, hallazgo o tesis), distinto de la `certeza` de las relaciones:

| Valor | Significado |
| --- | --- |
| `consolidado` | Replicado de forma independiente y robusta |
| `matizado` | El hallazgo central se sostiene, pero se han corregido su alcance, su tamaño o su interpretación |
| `en_debate` | Hay réplicas a favor y en contra, o críticas serias sin resolver |
| `no_replicado` | Réplicas rigurosas no han encontrado el efecto |
| `desacreditado` | Problemas graves de método o de integridad invalidan el estudio como prueba, aunque siga siendo históricamente importante |
| `superado` | Teoría abandonada por la disciplina y sustituida por otra (la frenología, la introspección como método único) |

Como las certezas y las fiabilidades, la app nunca muestra la etiqueta suelta, sino su significado, y la ficha dice **desde cuándo** y **por qué** tiene ese estado.

## 8. Retos «predice el resultado»

Primeros candidatos, porque la intuición falla de forma instructiva. Las cifras se comprueban en el artículo original:

- **Milgram:** ¿cuántos de 40 participantes llegaron a la descarga máxima? Los psiquiatras consultados de antemano predijeron casi ninguno; fueron 26.
- **Darley y Latané:** ¿ayuda más quien cree estar solo o quien cree que hay más testigos? Solos, la gran mayoría ayudó; con más testigos, menos de un tercio.
- **Festinger y Carlsmith:** ¿quién acabó valorando mejor una tarea aburrida, a quien le pagaron 1 dólar o 20 por mentir sobre ella? El de 1 dólar. Buen ejemplo, además, para enseñar que el hallazgo hoy está en debate.
- **Loftus y Palmer:** ¿cambia la velocidad recordada según el verbo de la pregunta («se estrellaron» frente a «se tocaron»)? Sí.

## 9. Puentes previstos

Pocos y valiosos al principio (decisión 10 del plan):

- **Filosofía:** Aristóteles (*Acerca del alma*), Descartes (dualismo), Locke (la mente como tabla rasa, asociación de ideas), Hume (asociacionismo). `migra_desde` para conceptos como la asociación de ideas.
- **Sociología:** George Herbert Mead, Kurt Lewin, la psicología social en su conjunto.
- **Antropología:** Freud (*Tótem y tabú*), Bartlett (el recuerdo como reconstrucción cultural), Vygotski.

## 10. Preguntas abiertas para Juan

1. ¿Corte vertical (el canon de toda la historia) o corte horizontal (un periodo completo)?
2. ¿Las 14 temáticas, o alguna sobra o falta?
3. ¿Jung y Adler en el carril del psicoanálisis o en uno propio?
4. ¿Los seis valores del estado de la evidencia, o simplificamos?
