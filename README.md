# Atlas de la Psicología

Mapa interactivo de la historia de la psicología. Autores, escuelas, conceptos, teorías y experimentos se presentan como una red navegable que el estudiante explora y va «despejando» a su ritmo, como en un juego de exploración.

**Autor:** Juan Domínguez Gallego

Forma parte de la colección **Atlas**, junto al [Atlas de la Filosofía](https://github.com/caducidad/ATLAS_FILOSOFIA). Lo común a toda la colección (esquema, validador, motor de la app y reglas de los puentes entre atlas) vive en [ATLAS_NUCLEO](https://github.com/caducidad/ATLAS_NUCLEO).

> Estado: en desarrollo. Datos estructurales (14 temáticas, 12 escuelas y 5 periodos) y la primera tanda del piloto, **la fundación (1879 – c. 1913)**: 11 autores, 7 obras, 9 conceptos, 9 tesis con su estado de la evidencia, 3 experimentos y 2 grandes preguntas, con 52 relaciones. Todo pasa el validador del núcleo sin errores.

## Qué tendrá de propio

- **Los experimentos como protagonistas.** Cada experimento clásico es una ficha propia: quién lo hizo, cómo, qué encontró y qué se sabe hoy de él.
- **El estado de la evidencia, a la vista.** Cada teoría y cada hallazgo indican si están consolidados, matizados, en debate, sin replicar o desacreditados, y desde cuándo. La crisis de replicación forma parte del mapa.
- **«Predice el resultado».** Antes de ver un experimento, el lector apuesta qué ocurrió.
- **La ética de la investigación,** señalada en los estudios que hoy serían inadmisibles.
- **Puentes** con el Atlas de la Filosofía y, más adelante, con los de Sociología y Antropología.

## Estructura del repositorio

```
atlas.json                  Configuración del atlas y extensiones del esquema base
datos/
  tematicas.json            Las 14 temáticas
  escuelas.json             Escuelas y corrientes (carriles de la línea del tiempo)
  precursores.json          c. 1800 – 1879
  fundacion.json            1879 – c. 1913
  grandes-escuelas.json     c. 1913 – c. 1956
  revolucion-cognitiva.json c. 1956 – c. 1980
  contemporanea.json        c. 1980 – hoy
docs/
  piloto.md                 Contenido del piloto y decisiones tomadas
  informes/
    fundacion.md            Informe previo de la primera tanda (1879 – c. 1913)
    grandes-escuelas.md     Informe previo de la segunda tanda (c. 1913 – c. 1956)
```

## Validar los datos

Con el repositorio [ATLAS_NUCLEO](https://github.com/caducidad/ATLAS_NUCLEO) descargado al lado:

```
python3 ../ATLAS_NUCLEO/herramientas/validar.py .
```

## Licencias

- **Textos y datos** (carpetas `datos/` y `docs/`): [CC BY-SA 4.0](LICENSE-DATOS.md).
- **Código**: [licencia MIT](LICENSE).

## Cómo citar

> Domínguez Gallego, Juan. *Atlas de la Psicología*. 2026. https://github.com/caducidad/ATLAS_PSICOLOGIA
