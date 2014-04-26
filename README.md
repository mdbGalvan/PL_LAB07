#Simple example of how to use Jison in the browser.

## Resumen

>Se reescribe el *Analizador Sintáctico de [PL0 Grammar](http://en.wikipedia.org/wiki/Recursive_descent_parser)* realizado en la realizado en esa práctica [práctica 5](http://pl-lab05.herokuapp.com/) usando en esta ocasión *Jison*. También podría observarse la [práctica 6](http://pl-lab06.herokuapp.com/) realizada con *PGE.js*.

>Además, se tuvo que:

>1. La salida debe ser el AST del programa de entrada
>2. Modifique block y statement para que los procedure reciban argumentos y las llamadas a procedimiento puedan pasar argumentos.
>3. Añada if ... then ... else ....
>4. Actualice la documentación de la gramática para que refleje la gramática ampliada
>5. Limite el número de programas que se pueden salvar a un número prefijado, por ejemplo 10. Si se intenta salvar uno se suprime uno al azar y se guarda el nuevo.
>6. Las pruebas deben comprobar que los AST generados reflejan la semántica del lenguaje así como alguna situación de error
>7. Sólo usuarios autenticados pueden salvar sus programas en la base de datos.
>8. Extienda la autenticación OAuth para que además de Google pueda hacerse con Twitter ó GitHub ó Facebook ó ... Sólo debe implementar una.
>9. Método de Entrega:
>>* Use un repositorio privado en BitBucket o bien solicite al administrador del Centro de Cálculo un repositorio privado en GitHub.
>>* Comparta dicho repositorio con sus colaboradores y con el profesor.
>>* Suba la práctica al workshop/taller antes de la fecha límite.
>>* Cuando el taller pase a la fase de evaluación haga público su repositorio.


>>![alt text](http://pl-lab07.herokuapp.com/images/PL0.png "PL/0")

## Motivación

>La aplicación fue propuesta para ser desarrolla en la asignatura **Procesadores de Lenguajes**, del tercer año del **Grado en Ingeniería Informática**. Se corresponde con la 7ª práctica de la asignatura.

##  Funcionamiento

>Puede probar en [Heroku](http://pl-lab07.herokuapp.com/), el funcionamiento del *Analizador Sintáctico del Lenguaje PL/0 usando Jison*.

>Pueden cargarse ejemplos previamente *salvados* de la gramática PL/0 cliqueando sobre ellos, también es posible subir un fichero propio o incluso introducir el código en el textarea. Una vez, cargada puedes pulsar el botón de parse para analizar el código. Luego, se muestra el resultado de lo analizado.

>También, cabe la opción de guardar el código introducido (por fichero o a mano). Para ello, se deberá introducir un nombre en el recuadro que se encuentra debajo de: `Save the code as` y clickear.

>En esta práctica también se ha añadido la opción de que sólo pueden salvar datos aquellas personas autentificadas por facebook o google.

>*Nota*: Las palabras reservadas de la gramática (if, call, ...) las acepta tanto en mayúscula como en minúscula. Aunque si se usa en mayúscula el codemirror no las reconoce, por lo que, queda mejor al ponerlas en mayúscula.

## Desarrollo

>Los lenguajes y herramientas (frameworks, librerías, etc.) utilizados para el desarrollo del presente proyecto fueron:

>* [Ruby gems](http://rubygems.org/)
* [Sinatra](http://www.sinatrarb.com/configuration.html)
* [Heroku](https://dashboard.heroku.com/apps)
* HTML/CSS/Javascript
* [JQuery](http://jquery.com/)
* [PEG.js](http://pegjs.majda.cz/)
* [DataMapper](http://datamapper.org/docs/)
* [Sass](http://sass-lang.com/) 
* [MathJax](http://docs.mathjax.org/en/latest/start.html)
* [SQLite](https://sqlite.org/)
* [PostgreSQL](http://www.postgresql.org/)
* [Jison](http://zaach.github.io/jison/)

## Tests

>Entorno de pruebas basado en [Mocha](http://visionmedia.github.io/mocha/) y [Chai](http://chaijs.com/guide/installation/). 

>Pueden ejecutarse las pruebas [aquí](http://pl-lab07.herokuapp.com/tests).


## Colaboradores

| Autores | E-mail |
| ---------- | ---------- |
| María D. Batista Galván   | magomenlopark@gmail.com  |


## Licencia

>Léase el archivo LICENSE.txt.
