# Piloto del Atlas de la Psicología

Versión 0.2 · 8 de octubre de 2026 · con las decisiones de Juan (apartado 10)

Propuesta de contenido para el primer piloto: fija qué entra y cómo se organiza. El formato de los datos es el de [`docs/esquema-base.md`](https://github.com/caducidad/ATLAS_NUCLEO/blob/main/docs/esquema-base.md) de ATLAS_NUCLEO, ampliado con el `atlas.json` de este atlas. El ejemplo `ejemplos/atlas-minimo/` del núcleo ya declara el tipo `experimento`, las relaciones `pone_a_prueba` y `replica` y la lente de la evidencia.

**Aviso de rigor.** Fechas, cifras y estados de la evidencia de este borrador son una primera propuesta. Cada uno se comprueba en la fuente al redactar la ficha, igual que en el Atlas de la Filosofía.

## 1. Alcance del piloto: dos fases

El piloto de filosofía fue un **corte horizontal**: una época, la Antigüedad, completa. Psicología hace los dos cortes, uno detrás de otro.

**Fase 1, corte vertical.** El canon a lo largo de toda la historia de la disciplina, unos 150 años: los autores del círculo 1 (en negrita en el apartado 5) y los experimentos marcados con ★ (apartado 6), con sus teorías y conceptos principales. Unos 80 nodos además de los estructurales (temáticas, contextos y escuelas).

Por qué primero el vertical:

- La historia de la psicología es corta; un solo periodo dejaría el mapa casi vacío.
- El estado de la evidencia, lo más propio de este atlas, solo se entiende viendo la historia entera: un experimento de 1971 se juzga con las críticas de 2018.
- La vista cronológica, los carriles por escuela y la lente de la evidencia se prueban desde el principio.

**Fase 2, corte horizontal.** Se completa un periodo entero, con los círculos 2 y 3: **revolución cognitiva y humanismo (1956–1980)**. Es el periodo más denso: concentra la mayoría de los experimentos célebres, buena parte de los debates de replicación y los puentes más claros con la sociología.

Tamaño orientativo al final de las dos fases: unos 140 nodos.

## 2. Periodos

Un archivo por periodo; cada uno es también un nodo `contexto`. Los límites son convenciones historiográficas y se dan como horquilla. Las temáticas y las escuelas, que atraviesan varios periodos, van en archivos propios.

| Archivo | Contenido | Horquilla | Prefijo de relaciones | De qué trata |
| --- | --- | --- | --- | --- |
| `tematicas.json` | Las 14 temáticas | | `tem-` | |
| `escuelas.json` | Escuelas y corrientes | | `esc-` | |
| `precursores.json` | Precursores | c. 1800 – 1879 | `pre-` | Raíces fisiológicas: psicofísica, localización cerebral, evolución, diferencias individuales. Las raíces filosóficas, más antiguas, se alcanzan por los puentes al Atlas de la Filosofía |
| `fundacion.json` | La fundación | 1879 – c. 1913 | `fun-` | Laboratorio de Wundt en Leipzig (1879), estructuralismo y funcionalismo, primeras leyes del aprendizaje y la memoria, nacimiento del psicoanálisis y de los tests |
| `grandes-escuelas.json` | Las grandes escuelas | c. 1913 – c. 1956 | `gre-` | Manifiesto conductista de Watson (1913), Gestalt, neoconductismo, expansión del psicoanálisis, Piaget y Vygotski |
| `revolucion-cognitiva.json` | Revolución cognitiva y humanismo | c. 1956 – c. 1980 | `cog-` | Simposio del MIT (1956), crítica de Chomsky a Skinner, humanismo, edad de oro de la psicología social, apego, sesgos y heurísticos |
| `contemporanea.json` | Psicología contemporánea | c. 1980 – hoy | `con-` | Neurociencia cognitiva, psicología positiva y evolucionista, crisis de replicación y ciencia abierta |

## 3. Temáticas

Catorce, como en filosofía, para mantener la simetría de la colección:

1. Métodos de investigación
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

La primera es «Métodos» y no «Historia y métodos» porque la historia ya es el atlas entero, mientras que los métodos (el experimento, el estudio de caso, la réplica, el metaanálisis) son un tema propio, y en este atlas uno central.

Las dos últimas se tratan **desde la historia de las ideas** (qué propuso cada corriente y con qué pruebas), no como orientación clínica. El lado clínico como tal sigue aparcado.

## 4. Escuelas y corrientes (carriles de la vista cronológica)

El carril de cada nodo lo decide el **primer** elemento de su lista `escuelas` (regla del esquema base).

| Escuela | Naturaleza | ¿Carril? | Notas |
| --- | --- | --- | --- |
| Estructuralismo | rótulo historiográfico | Sí | Nombre de Titchener para su programa; se aplica también, con matices, a Wundt |
| Funcionalismo | rótulo historiográfico | Sí | James, Dewey, Angell; más un clima que una escuela |
| Tradición psicodinámica | rótulo historiográfico | Sí | Paraguas de Freud, Jung, Adler, Anna Freud y Klein |
| · Psicoanálisis | real | No: va en el carril psicodinámico | Asociación Psicoanalítica Internacional desde 1910 |
| · Psicología analítica | real | No: va en el carril psicodinámico | Jung, tras su ruptura con Freud (1913–1914) |
| · Psicología individual | real | No: va en el carril psicodinámico | Adler, tras su ruptura con Freud (1911) |
| Conductismo | real | Sí | Watson acuñó el nombre (1913); luego el neoconductismo de Skinner, Tolman y Hull |
| Gestalt | real | Sí | Escuela de Berlín: Wertheimer, Köhler, Koffka |
| Psicología sociocultural | rótulo historiográfico | Sí | Vygotski y su escuela |
| Humanismo | real | Sí | «Tercera fuerza»: Maslow, Rogers |
| Cognitivismo | rótulo historiográfico | Sí | Miller, Neisser, Bruner, Simon |
| Neurociencia cognitiva | rótulo historiográfico | Sí | Desde finales de los años setenta |

Carril «otros» para quien no encaja en ninguna (Piaget, buena parte de la psicología social).

**Por qué un carril psicodinámico.** Ni Jung ni Adler caben con rigor bajo «psicoanálisis»: rompieron con Freud y fundaron escuelas propias. Pero darles carril propio llenaría la línea del tiempo de carriles casi vacíos. El paraguas «tradición psicodinámica», un rótulo historiográfico corriente, los reúne sin confundirlos: cada uno lleva primero el paraguas (que decide el carril) y después su escuela (`["escuela.tradicion_psicodinamica", "escuela.psicologia_analitica"]` en Jung), y la ruptura queda como relación entre fichas, que es lo que interesa al lector.

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

## 7. Estado de la evidencia: seis valores

Campo `estadoEvidencia` del nodo (teoría, hallazgo o tesis), distinto de la `certeza` de las relaciones. En el experimento, el campo recoge el estado de su hallazgo principal, como pide el ejemplo del núcleo. Se acompaña siempre de `notaEvidencia`: **desde cuándo** tiene ese estado y **por qué**, con la fuente.

**Pendiente del núcleo.** El esquema base admite cuatro valores: `consolidado`, `en_debate`, `no_replicado` y `superado`. Juan decidió usar seis, añadiendo `matizado` y `desacreditado`, sin los que los casos más instructivos del piloto (Milgram, Asch, el muñeco Bobo, Stanford) quedarían mal clasificados. Como es un campo común, se ha pedido al núcleo por el buzón (`2026-10-08-06-psicologia-filosofia-dos-valores-mas-en-estadoevidencia.md`); no se redefine solo en este atlas.

| Valor | Significado |
| --- | --- |
| `consolidado` | Replicado de forma independiente y robusta |
| `matizado` | El hallazgo central se sostiene, pero se han corregido su alcance, su tamaño o su interpretación |
| `en_debate` | Hay réplicas a favor y en contra, o críticas serias sin resolver |
| `no_replicado` | Réplicas rigurosas no han encontrado el efecto |
| `desacreditado` | Problemas graves de método o de integridad invalidan el estudio como prueba, aunque siga siendo históricamente importante |
| `superado` | Teoría abandonada por la disciplina y sustituida por otra (la frenología, la introspección como método único) |

Como las certezas y las fiabilidades, la app nunca muestra la etiqueta suelta, sino su significado.

**Tres familias para la vista.** Para que seis valores no pesen, la lente de la evidencia colorea por familias y deja el detalle para la ficha:

- **Se sostiene:** `consolidado`, `matizado`.
- **En duda:** `en_debate`.
- **No se sostiene:** `no_replicado`, `desacreditado`, `superado`.

**Guía de decisión.** Para que quien redacta elija siempre con el mismo criterio entre valores vecinos, se responden estas preguntas en orden y se para en la primera que decide:

1. ¿La disciplina ha abandonado esta explicación y la ha sustituido por otra mejor? → `superado`.
2. ¿El estudio original tiene fallos graves de método o de integridad que lo invalidan como prueba, al margen de lo que digan las réplicas (participantes guiados hacia el resultado, datos alterados, hechos mal descritos)? → `desacreditado`.
3. ¿Réplicas rigurosas (preregistradas, con muestras grandes o en varios laboratorios) han fallado de forma clara? → `no_replicado`.
4. ¿Hay resultados en los dos sentidos, o una crítica seria sin resolver? → `en_debate`.
5. Si las réplicas encuentran el efecto: ¿lo encuentran con el tamaño, el alcance y la interpretación del original? Sí → `consolidado`; con correcciones importantes → `matizado`.

Si un estudio nunca se ha replicado con rigor, se decide por el estado del debate y la `notaEvidencia` lo dice expresamente.

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

## 10. Decisiones de Juan

1. **Los dos cortes, en dos fases:** primero el vertical (el canon de toda la historia) y después el horizontal, con la revolución cognitiva y el humanismo completos (apartado 1).
2. **Las 14 temáticas,** con «Métodos de investigación» en lugar de «Historia y métodos» (apartado 3).
3. **Jung y Adler en un carril común, «tradición psicodinámica»,** junto a Freud, cada uno con su propia escuela como segundo elemento de la lista (apartado 4).
4. **Seis estados de la evidencia,** agrupados en tres familias para la vista y con una guía de decisión para los editores (apartado 7). Pendiente de que el núcleo admita los dos valores nuevos.
