# WhatsMovie
Procesamiento del lenguaje natural

Programa que pretende autocompletar un chat con diálogos de películas.

## Equipo de trabajo:
- Daniel, [*DanyDolphin*](https://github.com/DanyDolphin)
- Karla, [*KarlaDSJ*](https://github.com/KarlaDSJ)

### Con ayuda de:
- Emilio, [*milmor*](https://github.com/milmor)
- Víctor, [*VMijangos*](https://github.com/VMijangos)

## Dataset:
- [*Marvel Cinematic Universe*](https://www.kaggle.com/phiitm/marvel-cinematic-universe-dialogue-dataset)
- [*Christopher Nolan*](https://www.kaggle.com/phiitm/marvel-cinematic-universe-dialogue-dataset)
- [*Pride & Prejudice*](https://www.kaggle.com/theeranartmeesathien/pride-prejudice-subtitles-and-text)

NOTA: Los modelos para RNN y Seq to Seq se encuentran en una carpeta de [*Drive*](https://drive.google.com/drive/folders/1suwOTuJFR9OhBVawD2raKh8CGw1hiTqV?usp=sharing), para correr los notebooks es necesio ponerlas a dentro de la carpeta process/


### Práctica 1
Preprocesar un corpus a partir de métodos basados en lenguajes formales y tokenizarlo en subpalabras.

### Práctica 2 
Generar un modelo del lenguaje neuronal junto con los embeddings de  ́este, que puedan ser utilizados en otras tareas

### Práctica 3 
Generación de texto. Para generar texto probamos 3 modelos:

- Red de Bengios
- Red RNN
- Red Seq to Seq

Cada modelo propuesto fue mejor que el anterior, al menos en apariencia, siendo el mejor el de la Red Seq to Seq ya que esta red guarda la información del dialogo anterior y al momento de entrenar lo forzamos un poco pasandolé a lo que queremos llegar, sin embargo aunque este modelo genera texto, que en estructura es bueno, si lo ponemos en contexto con el díalogo/query de entrada no tiene tanta relación, además un reto igual de grande que generar texto es encontrar la manera de evaluar que lo que está generando está bien, sin duda fue la parte en la que más batallamos, únicamente medimos la entropia y la perplejidad.
