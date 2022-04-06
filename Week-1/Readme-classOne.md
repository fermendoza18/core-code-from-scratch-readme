# core-code-from-scratch-readme

## Interpreted And Compiled Programming Languages

### Compiled Programming Languages

Estos son lenguajes de programación que pasan por un programa llamado compilador, este lo que hace es convertirnos el código fuente a código máquina para que nuestras computadoras puedan entender y correr el archivo que nos brindó el compilador, con esto podemos compartir el código máquina sin necesidad de enseñar nuestro código fuente, aunque estos lenguajes son menos flexibles que los interpretados, ya que no pueden ser ejecutados en todas las plataformas, solo a la que fue desarrollado.

### Interpreted Programming Languages

Estos lenguajes se caracterizan porque nuestro código fuente va a ser leído por un programa llamado interpreté línea por línea al momento de ejecutar nuestro archivo, que en este caso sería el propio código fuente, esto hace estos lenguajes un poco más lentos dado que tiene que procesar las instrucciones una por una y realizar esos procesos.

------------

## Is Java compiled or interpreted, or both?

Java es un intermedio de los dos tipos de lenguajes mencionados anteriormente, el código fuente pasa por un compilador que nos dará como resultado un archivo intermedio llamado bytecodes, este se caracteriza por ser multiplataforma, ya que solo necesita tener la jvm instalada en cualquier equipo para entrar a la segunda etapa del proceso, que sería que la jvm que traduzca el archivo de bytecodes a código máquina, es por eso que java utiliza los dos procesos mencionados.

------------

## Currency Converter Exercise

```
1. START
2. INIT usDollarsAmount, bitcoinResult, actualBitcoinPrice
3. actualBitcoinPrice <-- 0,000022
4. PRINT  'Insert the Amount that you want to convert'
5. usDollarsAmount <-- GET
6. bitcoinResult <-- usDollarsAmout * actualBitcoinPrice
7. PRINT 'Bitcoin: ', bitcoinResult
8. END
```
