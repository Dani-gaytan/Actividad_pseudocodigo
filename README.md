# A continuación se muestran los algoritmos realizados primero en pseudocódigo, ahora en lenguaje de Python 

## Algoritmo para calcular el área de un triángulo

```
print("El siguiente algoritmo calculará el área de un triángulo")
base = float(input("Ingrese la base del triángulo: "))
altura = float(input("Ingrese la altura del triángulo: "))
area = (base * altura) / 2
print("El área del triángulo es:", area)
```

## Algoritmo para calcular el volumen de una esfera
```
import math

def calcular_volumen_esfera(radio):
    volumen = (4/3) * math.pi * radio**3
    return volumen

print("El siguiente algoritmo calculará el volumen de una esfera")
radio = float(input("Ingrese el radio de la esfera: "))
redondeo = round(calcular_volumen_esfera(radio),2)
print("El volumen de la esfera es:", (redondeo), "unidades cúbicas")
```

## Algoritmo para calcular ordenar un número de mayor a menor
```
print("Este algoritmo ordenará 5 números ingresados de mayor a menor :)")
conjunto = [float(input("Capture su primer número: ")), 
float(input("Capture su segundo número: ")), 
float(input("Capture su tercer número: ")), 
float(input("Capture su cuarto número: ")), float(input("Capture su último número: "))]
conjunto.sort(reverse=True)
print("Los números en orden descendente son:", conjunto)
```

## Algoritmo para saber cuantos días faltan para navidad o día de muertos
```
from datetime import datetime

fecha_actual =datetime.now()
print("La fecha actual es: ", fecha_actual)

navidad = datetime(fecha_actual.year, 12, 25 )

if fecha_actual.date() == navidad.date():
  print("¡Feliz Navidad! 🎄")
else:
  if fecha_actual < navidad:
      dias_faltantes = (navidad - fecha_actual).days
      print("Faltan", dias_faltantes, "días para Navidad :(")
  else:
      dias_faltantes = (fecha_actual - navidad).days
      print("Ya pasaron", dias_faltantes, "días desde la Navidad")

muertos = datetime(fecha_actual.year, 11, 2 )

if fecha_actual.date() == muertos.date():
  print("¡hora de poner la ofrenda! :O")
else:
  if fecha_actual < muertos:
      dias_faltantes = (muertos - fecha_actual).days
      print("Faltan", dias_faltantes, "días para Día de muertos :(")
  else:
      dias_faltantes = (fecha_actual - navidad).days
      print("Ya pasaron", dias_faltantes, "días desde el dia de Muertos ")
```

## Algoritmo para mostrar tú nombre
```
nombre = input("¿Cuál es tu nombre?")
print("El nombre: ", (nombre), "es bellisimo \(^o^)/")
```

## Algoritmo para calcular el incremento salarial

```
print ("Este algoritmo calculará su respectivo incremento salarial, acorde con su salario mensual")
salario= float(input("Capture su salario mensual:" ))
if salario > 15000:
  salario *= 1.20
  print("Su salario con el respectivo incremento es:", salario, "Un aumento del 20%")
else: 
  salario *= 1.15
  print("Su salario con el respectivo incremento es:", salario, "Un aumento del 15%")
```
