<h1>Quiz #2</h1>
<ul>
  <li>Mónica Alfaro Parrales - 2020132572</li>
  <li>Sebastián Alpízar Morales - 2019187543</li>
  <li>Esteban Bosques Mondol - 2013046970</li>
  <li>Esteban Durán Vargas - 2020388144</li>
</ul> 

<h2>Acerca de la solución</h2>
Para este quiz se asignó la tarea de realizar un modelo MongoDB para el
sistema de <a href="https://datashine.org.uk/">https://datashine.org.uk/</a>. 
Para este modelo se utilizó un Json ejemplo para designar la organización de
los objetos de la base de datos. Hay tres colecciones principales que 
componen la base: datashine.json, cities.json y areas.json
La infomación principal se almacena en datashine.json. Este consiste en
un array de data subdividida por los filtros que se presentan en la aplicación.
Estos filtros permiten organizar los datos por sus subflitros. Al final de 
cada filtro se tiene una sección con el código del "path" que sigue este
filtro, esto nos ayuda a poder relacionar los filtros seleccionados con el
objeto de areas.json el cuál contiene los porcentajes correspondientes a cada filtro,
la información de los polígonos y sus características físicas, como 
zoom mínimo antes de convertirse en un macro área. Esto de los macro áreas 
y micro áreas consiste en una sub-división que realiza el sistema una vez que 
el zoom está muy lejos como para ver las áreas detalladamente, por lo que se 
"agrupan" en macro áreas que contienen la información de las micro áreas de 
manera general para una visualización más sencilla. Sin embargo, esta relación 
que se realiza entre datashine.json y areas.json es únicamente al final de la 
selección de filtros pues no es necesario tener la información de las áreas siempre.
Además, la colección de cities.json almacena la información de Zip Code de cada 
ciudad la cuál es utilizada por los filtros del sector de abajo de la página. 