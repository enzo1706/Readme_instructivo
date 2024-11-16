# **Detector y Mutador de ADN**

Este programa analiza secuencias de ADN representadas en una matriz de 6x6 para detectar mutaciones y permite modificarlas (mutarlas) o sanarlas. Se centra en las bases nitrogenadas del ADN: **Adenina (A)**, **Timina (T)**, **Citosina (C)** y **Guanina (G)**.

---

## **Descripción**

Una secuencia de ADN se considera mutante si contiene al menos 4 bases nitrogenadas iguales seguidas en alguna de las siguientes direcciones:
- **Horizontal**
- **Vertical**
- **Diagonal**

El programa incluye clases que permiten:
- **Detectar mutantes** en una matriz de ADN.
- **Crear mutantes** de manera horizontal, vertical o diagonal.
- **Sanar ADN**, generando nuevas secuencias sin mutaciones.

### **Ejemplo de Matriz de ADN**
Una matriz de ADN se representa como una lista de strings:
```python
matriz = ["AGATCA", "GATTCA", "CAACAT", "GAGCTA", "ATTGCG", "CTGTTC"]

## **1. Ejecutar el Programa**
El programa interactúa con el usuario desde un archivo ejecutable.py. Ejemplo:
python ejecutable.py

## **2. Flujo del Programa**
Solicita al usuario una matriz de ADN.
Pregunta si desea:
Detectar mutaciones.
Crear mutantes (mutar).
Sanar el ADN.
Según la opción seleccionada:
Se utiliza la clase Detector para verificar mutaciones.
Se instancian las clases Radiación o Virus para mutar el ADN.
Se utiliza la clase Sanador para crear un nuevo ADN sin mutaciones.
Muestra la matriz final y un mensaje con el resultado.

## **Ejemplo de Entrada y Salida**
Entrada
Ingrese la matriz de ADN:
AGATCA
GATTCA
CAACAT
GAGCTA
ATTGCG
CTGTTC
¿Qué desea hacer? (1: Detectar mutantes, 2: Mutar, 3: Sanar)

Salida
Si se detecta una mutación:
¡Mutante horizontal detectado en la fila 3 columna 3! Base: C

Si se realiza una mutación:
Mutación horizontal realizada en fila 0 desde columna 0.
TTTTCA
GATTCA
CAACAT
GAGCTA
ATTGCG
CTGTTC

Si se sana el ADN:
Matriz curada.
ACGTCA
GATTGA
CAACAT
GAGCTA
ATTGCG
CTGTAC
