# Estilos de Programacion

## Monolitico:
Todo el codigo esta escrito en un solo archivo y exportado como un solo modulo. Esta es una caracteristica de este estilo, donde toda la logica esta contenida dentro de una sola unidad.
## Ejemplo:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/95ac53b2-7860-478b-bef9-ff1e6959b35c)

Todo el componente Resultados esta definido en un solo archivo.

## Pipeline:
El uso de este estilo implica el pasar la salida de una funcion como entrada para otra funcion, creando un 'pipeline' con las llamadas a funciones.
## Ejemplo:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/f523f3f1-5d5a-491c-ba55-75f07121d247)

Aqui, la salida de la funcion obtenerResultadosReales() esta siendo pasada como argumento a la funcion setResultados(), creando un pipeline.

## Kick Forward: 
Este estilo esta caracterizado por pasar una función de devolución de llamada (callback) a otra función para que se ejecute después de completarse una operación. En JavaScript, esto se realiza comúnmente utilizando Promesas y la sintaxis async/await; then/catch.
## Ejemplos:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/a1ffc9f3-7235-44bd-8357-4e54aed21b44)
![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/28b91ac1-85b3-4ab0-a138-dcc734d26a2b)

Aqui, la funcion setResultados(data) es una funcion de llamada (callback) que es pasada a then() y es ejecutada tras obtener la respuesta de la funcion obtenerResultadosReales().

# Practicas de Codificacion Legible

## Comentarios y documentacion:
Dado que este es un trabajo grupal, es importante el agregar comentarios que orienten a los demas desarrolladores a la hora de interactuar con otros modulos.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/a5f6911d-9499-40c4-80a3-3659558843ea)

## Evitar comentarios obvios:
Ahora, si bien los comentarios se agradecen a la hora de entender el codigo, evidentemente tampoco esta bien sobrecargar el codigo de comentarios triviales, ya que, en partes el codigo es bastante autoexplicativo, lo que haria que los comentarios estorbasen mas que otra cosa. Es en estas secciones que se evita colocar comentarios.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/10942acb-8734-4c71-b33f-94980457e62d)

## Identacion consistente:
Para una adecuada lectura del codigo, es importante que la identacion sea facil de identificar y que sea cosntante a lo largo de todo el archivo.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/9b337040-cfd6-4fe5-ac35-bf3e622b7c7c)

## Agrupacion del codigo:
A la hora de trabajar, el tener el codigo organizado en bloques de acuerdo a ciertos criterios es bastante util, ya que no hace falta desplazarse mucho en el archivo para realizar las modificaciones necesarias. En este caso, se separo el codigo en 2 bloques de funcionalidad. Uno obtiene los valores y el otro realiza la representacion grafica.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/0895ba58-43bb-4acd-bd2a-8e8e73a4a0d6)

## Evitar el Deep Nesting:
Una mala practica es generar Deep Nesting en el codigo, es decir, que se realizen varias instrucciones seguidas que hagan la identacion irse mas y mas hacia dentro, dificultando la lectura del codigo y su posterior modificacion (en las otras imagenes ya se evidencia que eso no es un problema presente).

## Limitar la longitud de las lineas:
El limitar la longitud de cada linea hace que sea mas facil de leer el codigo, se recomienda que no sea de mas de 80 lineas, en este caso la linea con mas caracteres (sin contar comentarios) tiene solo 72.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/9d040608-d867-419d-81a8-2af341cb9341)

## Usar nombres significativos para variables y funciones.
El usar nombres autoexplicativos facilita el entendimiento del codigo para los otros desarrolladores y para uno mismo, ya que al tener las funciones y variables un nombre relacionado al trabajo que hacen, se puede seguir la linea de pensamiento del desarrollador que implemento el codigo incialmente con mas facilidad.

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/f9ae7d5d-2e10-424b-88ab-0b2d48b6ec9d)

# Comentarios adicionales:
Tras instalar la extension SonarLint esta no detecto mayores inconvenientes en el codigo implementado.
Esta version aun esta en pronto desarrollo, con lo que se espera hacer mejoras a futuro ademas de tener que juntar los modulos con los otros participantes del grupo.
Se priorizo el flujo principal de casos, que es lo que  esta implementado hasta el momento.
## Resultado ahsta el momento - Visualizacion de Resultados:

![image](https://github.com/LeoUNSA/Eleccionador-Inador/assets/104027221/79c21dae-a9b5-41ea-9d70-3b80068b76d7)
