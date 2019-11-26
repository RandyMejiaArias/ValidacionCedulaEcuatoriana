# ValidacionCedulaEcuatoriana
Método para validar que un número de cédula ingresado sea válido, se envía como parámetro un String de 10 caracteres.
Devuelve como resultado un booleano.

El algoritmo cumple las siguientes condiciones:
- El décimo dígito es un dígito verificador y es el resultante de un cálculo.
- Las 2 primeras posiciones corresponden a la provincia donde fue expedida, por lo cual los dos primeros números no será mayor a 24 ni menor a 1.
- El tercer dígito es un número menor a 6 (0,1,2,3,4,5)
- Se trabaja con los 9 dígitos de la cédula.
- Cada dígito de posición impar se lo multiplica por dos, si este resultado es mayor que nueve se resta nueve.
- Cada dígito de posición par se lo multiplica por uno
- Se suman todos los resultados
- Este resultado se resta de la decena inmediata superior.
- El resultado anterior debe ser el décimo dígito.
- Si la suma resulta 10, el décimo dígito es cero.
