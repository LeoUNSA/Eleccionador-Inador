# Estilos de Programacion - AccessResults

## Monolitico:
Todo el codigo esta escrito en un solo archivo y exportado como un solo modulo. Esta es una caracteristica de este estilo, donde toda la logica esta contenida dentro de una sola unidad.
## Ejemplo:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/77308482-a9c9-4504-b139-e8e9b7ec34d4)

Todo el componente Resultados esta definido en un solo archivo.

## Pipeline:
El uso de este estilo implica el pasar la salida de una funcion como entrada para otra funcion, creando un 'pipeline' con las llamadas a funciones.
## Ejemplo:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/b00a085e-9c72-49e4-9e60-3de01947ea2a)

Aqui, la salida de la funcion obtenerResultadosReales() esta siendo pasada como argumento a la funcion setResultados(), creando un pipeline.

## Kick Forward: 
Este estilo esta caracterizado por pasar una función de devolución de llamada (callback) a otra función para que se ejecute después de completarse una operación. En JavaScript, esto se realiza comúnmente utilizando Promesas y la sintaxis async/await; then/catch.
## Ejemplos:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/7d856923-d88d-4478-8ddb-57d12b3037fa)

Aqui, la funcion setResultados(data) es una funcion de llamada (callback) que es pasada a then() y es ejecutada tras obtener la respuesta de la funcion obtenerResultadosReales().

# Practicas de Codificacion Legible - AccessResults

## Comentarios y documentacion:
Dado que este es un trabajo grupal, es importante el agregar comentarios que orienten a los demas desarrolladores a la hora de interactuar con otros modulos.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/84c5ce4b-44af-4966-948d-811f1b4c4c08)

## Evitar comentarios obvios:
Ahora, si bien los comentarios se agradecen a la hora de entender el codigo, evidentemente tampoco esta bien sobrecargar el codigo de comentarios triviales, ya que, en partes el codigo es bastante autoexplicativo, lo que haria que los comentarios estorbasen mas que otra cosa. Es en estas secciones que se evita colocar comentarios.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/cb493a9e-43f1-41d7-9cf2-0f7bf43ce225)


## Identacion consistente:
Para una adecuada lectura del codigo, es importante que la identacion sea facil de identificar y que sea cosntante a lo largo de todo el archivo.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/d21450bc-1a95-49b3-9f7b-391922832da3)

## Agrupacion del codigo:
A la hora de trabajar, el tener el codigo organizado en bloques de acuerdo a ciertos criterios es bastante util, ya que no hace falta desplazarse mucho en el archivo para realizar las modificaciones necesarias. En este caso, se separo el codigo en 2 bloques de funcionalidad. Uno obtiene los valores y el otro realiza la representacion grafica.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/768ee451-52ab-4e48-8dd8-bfc3e5b00e3d)

## Evitar el Deep Nesting:
Una mala practica es generar Deep Nesting en el codigo, es decir, que se realizen varias instrucciones seguidas que hagan la identacion irse mas y mas hacia dentro, dificultando la lectura del codigo y su posterior modificacion (en las otras imagenes ya se evidencia que eso no es un problema presente).

## Limitar la longitud de las lineas:
El limitar la longitud de cada linea hace que sea mas facil de leer el codigo, se recomienda que no sea de mas de 80 lineas, en este caso la linea con mas caracteres (sin contar comentarios) tiene solo 72.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/a47d0143-c2aa-4172-a170-35118cb3d8e8)

## Usar nombres significativos para variables y funciones.
El usar nombres autoexplicativos facilita el entendimiento del codigo para los otros desarrolladores y para uno mismo, ya que al tener las funciones y variables un nombre relacionado al trabajo que hacen, se puede seguir la linea de pensamiento del desarrollador que implemento el codigo incialmente con mas facilidad.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/7783cfd5-a258-44ff-afb4-041758253709)

# Principios Solid - AccessResults
Debido a la naturaleza del lenguaje en el que se esta trabajando el codigo (siendo react un lenguaje de tipo funcional), la aplicacion de los principios SOLID que estan principalmente presentes en la programacion orientada a objetos, no se puede realizar de la misma manera que en  estos ultimos. Sin embargo, de cierto modo estan presentes usando cierta abstraccion conceptual. Por ejemplo el SRP y ISP por la distribucion del proyecto en modulos esta inherentemente presente, ya que cada modulo realiza una tarea en especifico y seran posteriormente integrados.

# Comentarios adicionales:
Tras instalar la extension SonarLint esta no detecto mayores inconvenientes en el codigo implementado.
Esta version aun esta en pronto desarrollo, con lo que se espera hacer mejoras a futuro ademas de tener que juntar los modulos con los otros participantes del grupo.
Se priorizo el flujo principal de casos, que es lo que  esta implementado hasta el momento.
