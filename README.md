# Funciones-Matematicas-Oracle
#### Realizan operaciones con expresiones numericas y siempre retornan un resultado con tipo de dato numerico, a estas funciones se le pasa un parametro de entrada numerico para que retornen dicho valores.

>funcion abs retorna el valor absoluto de un numero que le pasemos en una ejecucion , tambien funciona con operaicones matematicas
```sql
select abs(-50) from dual;
```
|ABS(-50)|
|:-------:|
|50|

___

>funcion ceil: redondea un numero entero hacia arriba
```sql
select ceil(15.50) from dual;
```
|CEIL(15.50)|
|:-------:|
|16|
___

> funcion floor- redondea el valor hacia a abajo de una cantidad que le especifiquemos en uan ejecucion

```sql
select floor ( 15.50) from dual;
```
|FLOOR(15.50)|
|:-------:|
|15|

___

> funcion mod: devuelve el residuo de una division entre dos numeros enteros
```sql
select mod(10,3) from dual;
```
|MOD(10,3)|
|:-------:|
|1|

___ 

> funcion power: realiza la operacion de potenciacion matematica
```sql
select power(2,3) from dual;
``` 
|POWER(2,3)|
|:-------:|
|8|

___

>funcion round : ejecuta el redondeo de una cantidad en decimales en tantos lugares que se le indiquemos en un segundo parametro en una ejecucion

```SQL
select round(123.456,2) from dual;
```
|ROUND(123.456,2)|
|:-------:|
|123.46|

```SQL
select round(123.456,3) from dual;
```
|ROUND(123.456,3)|
|:-------:|
|123.456|

```SQL
select round(123.456,1) from dual;
```
|ROUND(123.456,1)|
|:-------:|
|123.5|

___

>funcion sign : retorna la naturaleza de un numero entero que le pasemos al sistema
```SQL
select sign (-100) from dual;
```
|SIGN(-100)|
|:-------:|
|-1|

#####si colocamos 100 nos devolvera 1 esto significa q es positivo
___

>funcion trunc: corta las cifras decimales de una cantidad;
```sql
select trunc(1234.1234,3) from dual;
```
|TRUNC(1234.1234,3)|
|:-------:|
|1234.123|

___

>funcion sqrt : raiz cuadrada a una cantidad que le pasemos a una ejcucion del sistema
```sql
select sqrt(27) from dual;
```
|SQRT(27)|
|:-------:|
|5.196152422706632|

##### para evitar que salga muchos decimales podemos usar la funcion round combinado con srt a esto se le llama **funciones anidadda**
```sql
select round(sqrt(27)) from dual;
```
|SQRT(27)|
|:-------:|
|5|
