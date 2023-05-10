1. Error: “ncaught TypeError: guessSubmit.addeventListener is not a function at index.html:89:21 (anónimo) @ index.html:89”
   Solución: Corregir el nombre del método “addeventListener” a “addEventListener” ya que no reconoce debido a que el método del evento no está escrito correctamente en dos partes del código “resetButton.addEventListener("click", resetGame)” y en “guessSubmit.addEventListener("click", checkGuess)”.

2. Error: “index.html:78 Uncaught TypeError: Cannot set properties of null (setting 'textContent') at HTMLInputElement.checkGuess (index.html:78:41)”.
   Solución: Modificar el querySelector de la clase lowOrHi a “document.querySelector(".lowOrHi")” ya anteriormente no hace referencia a una clase y como consecuencia no muestra ningún resultado en la etiqueta p con la clase lowOrHi.

3. Error: Solo se está generando un numero aleatorio entre 1-10 y uno de los requerimientos de la aplicación debe ser un numero entre el 1-100.
   Solución: En la función Math.random() debe multiplicar por 100.

4. Error: En la variable randomNumber se genera números con decimales es decir que no son enteros.
   Solución: redondear el número a entero con la función Math.round().

5. Error: El número de intentos solo está definido 5 veces y en los requerimientos indica que debe ser de 10 intentos.
   Solución: modificar la constante “ATTEMPS” y asignarle el valor de 10;

6. No se puede comprar dos variables de diferentes tipos con este operador “===”.
   Solución: En las condiciones se debe cambiar el operador “===” a “==” para no forzar que los tipos de variables tiene que ser igual.

7. Error: El color del background de los lastResult no corresponde a la respuesta.
   Solución: cambiarlo segundo la respuesta obtenido para que tenga sentido.

8. Error: Validar que el usuario debe ingresar un número entero.
   Solución: Crear una nueva condición “if (isNaN(userGuess) || userGuess % 1 !== 0)” y que retorne si se cumple para no sumar el guessCount.

9. Error: en la función restGame() no se genera correctamente el número random.
   Solución: arreglar la función de Math a “Math.round(Math.random() \* 100)”.
