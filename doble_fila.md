##Lunes 14 de septiembre 2015

###Doble Fila

####Valores Iniciales
```
Ai = -1
Ad = -1
```
####Altas

#####Izquierda
```
Si Ai == -1 Entonces #Esta vacio
	Ai = 0
    Ad = 0
	Leer valor
	vector[0] = valor
de otra manera si (Ad=Ai-1) Ó (Ad=limite Y Ai=0) Entonces
	Mostrar Fila Llena
Sino
    Ai = (Ai==0)?limite:Ai-1
    Leer valor
    vector[Ai] = valor
Fin Si
```
#####Derecha
```
Si Ai == -1 Entonces #Esta vacio
	Ai = 0
    Ad = 0
	Leer valor
	vector[0] = valor
de otra manera si (Ad=Ai-1) Ó (Ad=limite Y Ai=0) Entonces
	Mostrar Fila Llena
Sino
    Ad = (Ad==limite)?0:Ad+1
    Leer valor
    vector[Ad] = valor
Fin Si
```
####Bajas
#####Izquierda
```
Si Ai == -1 Entonces
	Mostrar Fila Vacia
De otra manera si Ad == Ai Entonces
	Ai = -1
    Ad = -1
sino
	Ai = (Ai==limite)?0:Ai+1
Fin Si
```
#####Derecha
```
Si Ai == -1 Entonces
	Mostrar Fila Vacia
De otra manera si Ad == Ai Entonces
	Ai = -1
    Ad = -1
sino
	Ad = (Ad==0)?limite:Ad-1
Fin Si
```
####Consultas
#####Izquierda
```
Si Ai == -1 Entonces
	Mostrar Fila Vacia
sino
	Mostrar vector[ai]
Fin Si
```
#####Derecha
```
Si Ai == -1 Entonces
	Mostrar Fila Vacia
sino
	Mostrar vector[ad]
Fin Si
```
####Reporte/Recorrido
#####Izquierdo
```
Desde i=Ai Hasta i=Ad i++
	Si i = (limite+1)
    	i=0
    Fin Si
	Mostrar i, vector[i]
Fin Desde
```
#####Derecha
```
Desde i=Ad Hasta i=Ai i--
	Si i = -1
    	i=0
    Fin Si
	Mostrar i, vector[i]
Fin Desde
```
####Depuración
```
Desde i=0 Hasta i=limite i++
	Mostrar i, vector[i]
Fin Desde
Mostrar Ai, Ad
```
