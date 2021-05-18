# Experiencias con RadVax

RadVax es una vacuna de código abierto, disponible gratuitamente para que cualquiera pueda fabricarla.  Actualmente la vacuna es experimental, y cada usuario que la toma ha elegido hacerlo sabiendo que fue diseñada y predicha como segura, pero que no se han realizado estudios formales (aunque el grupo RaDVaC está buscando socios para realizar ensayos clínicos).

El conjunto de datos sirve para dos propósitos:
1. Permite ver lo que ha ocurrido con los usuarios en el pasado
2. Te permite presentar tu propia experiencia, para que los futuros usuarios potenciales puedan evaluar

El conjunto de datos está disponible en este repositorio en el archivo [radvax_exp.tsv](/radvax_exp.tsv) , y cualquiera es libre de verlo o descargarlo.  El archivo de datos es un archivo "separado por tabulaciones", que puede ser leído por cualquier lector de texto. Para leerlo con un programa de hoja de cálculo (como MS Excel), es posible que tenga que especificar "tab" como separador.  

Si desea enviar su propia experiencia con el uso de RadVax, puede hacerlo a través de uno de los dos métodos siguientes

1. Rellene las preguntas que se formulan a continuación y envíenos las respuestas por correo electrónico.
2. Descargue el archivo de experiencias pasadas, añada su propia entrada en la parte inferior, y luego envíe una Solicitud de Extracción (este método es preferible, si usted es capaz de hacerlo).

Como en todos los proyectos de ciencia ciudadana, confiamos en que nos informe de sus resultados con honestidad.  Haremos algunos controles de calidad muy básicos (por ejemplo, si envías información sobre un registro anterior utilizando una dirección de correo electrónico diferente, querremos saber por qué), pero en última instancia contamos contigo.

Recuerda que esta información está a disposición de cualquiera, así que no envíes nada con lo que no te sientas cómodo compartiendo públicamente.  Si necesitas ayuda con el envío, puedes enviarnos un correo electrónico.


# Preguntas
Para reducir las molestias, hemos dividido las preguntas en tres grupos.  El primer grupo es el más importante (básicamente, ¿hubo efectos secundarios?).  El segundo grupo de preguntas son rasgos sobre ti, que podrían permitir a la gente aprender si hay variaciones sistemáticas en la respuesta (por ejemplo, tal vez las mujeres son más propensas a tener dolores de cabeza después de tomar RadVax, o los mestizos son más propensos a experimentar una nariz congestionada).  El tercer grupo de preguntas es potencialmente interesante, pero no crítico.  Por favor, rellénelas si le resulta conveniente, pero no se sienta mal si no puede hacerlo.

## Sobre los efectos secundarios
- Identificador único (vea más abajo las instrucciones para hacer su propio identificador único)
- En la semana posterior a la toma de RadVax, ¿notó síntomas físicos?
- Incluyendo esta dosis, ¿cuántas dosis de RadVax ha tomado?

## Sobre usted
- edad en el momento de la primera dosis de RadVax
- sexo
- etnia

## Otras preguntas
- Fecha de la dosis de RadVax (aprox.)  AAAA/MM/DD
- Generación de RadVax, si se conoce
- ¿Otros comentarios?


## Utilizar una identificación única
Para poder compartir sus datos sin revelar su información personal, debe enviar su experiencia junto con un identificador único.  Puede utilizar cualquier método para generarlo, pero el siguiente es fácil y seguro.  Básicamente, sólo tienes que pasar tu nombre por una "función hash", y utilizar el resultado.  Si estás interesado, puedes aprender más [aquí](https://www.kalzumeus.com/essays/dropping-hashes/)

### Generar tu nombre con hash usando DuckDuckGo
- Ve al sitio web [DuckDuckGo.com](https://duckduckgo.com/)
- introduce SHA, seguido de tu nombre: `SHA "Firstname Lastname"`.  Por ejemplo, Jane Doe introduciría su nombre de la siguiente manera:

![Página de inicio de DuckDuckGo, con 'SHA "Jane Doe"' en el cuadro de búsqueda](/figs/DDG__homepage.png)

- Copia el resultado; ese código es tu identificador único (y nadie puede invertirlo para saber tu nombre).  El identificador único de Jane es `cac7bbb6b67b44ea0ab997d34a88e4ea9b4d3d62`.

![DuckDuckGo devuelve la página, mostrando el identificador único de Jane](/figs/DDG__Jane_Doe.png)

- Eso es todo.

- Si alguna vez necesitas obtener tu identificador de nuevo, sólo tienes que repetir los pasos anteriores.  Asegúrate de escribir tu nombre exactamente igual, incluyendo las mayúsculas.  La diferencia de una sola letra cambiará drásticamente la salida de la función hash.  Por ejemplo, si Jane se olvida de escribir su nombre en mayúsculas, y escribe `SHA "jane Doe"`, la salida se convierte en:

![DuckDuckGo devuelve la página, mostrando una salida diferente cuando el nombre no está en mayúsculas](/figs/DDG__jane_Doe.png)

