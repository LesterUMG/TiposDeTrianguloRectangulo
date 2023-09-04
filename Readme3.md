# TAREA 1 DE ALGORITMOS
# Lester López
## El siguiente programa muestra 4 tipos de triangulo rectangulo.
>Algoritmo en Pseudocodigo
 ```
 Algoritmo TiposDeTrianguloRectangulo
	Definir puntos Como Entero
	definir opc Como Entero
	Escribir "Ingrese el numero de puntos que desee que tenga el triangulo"
	Leer puntos
	
	Escribir "¿Cual de las 4 formas del Triangulo Rectangulo desea ver?"
	
	Escribir "Triangulo Rectangulo: 1"
	Escribir "   +-----------+"
	Escribir "     *          "
	Escribir "     * *        "
	Escribir "     * * *      "
	Escribir "     * * * *    "
	Escribir "     * * * * *  "
	Escribir "   +-----------+"
	
	Escribir "Triangulo Rectangulo: 2"
	Escribir "   +-----------+"
	Escribir "     * * * * *  "
	Escribir "     * * * *    "
	Escribir "     * * *      "
	Escribir "     * *        "
	Escribir "     *          "
	Escribir "   +-----------+"
	
	Escribir "Triangulo Rectangulo: 3"
	Escribir "   +-----------+"
	Escribir "     * * * * *  "
	Escribir "       * * * *  "
	Escribir "         * * *  "
	Escribir "           * *  "
	Escribir "             *  "
	Escribir "   +-----------+"
	
	Escribir "Triangulo Rectangulo: 4"
	Escribir "  +-----------+"
	Escribir "            *  " 
	Escribir "          * *  "
	Escribir "        * * *  "
	Escribir "      * * * *  "
	Escribir "    * * * * *  "
	Escribir "  +-----------+"
	
	leer opc
	
	Segun opc Hacer
		1:
			Para i<-1 Hasta puntos Con Paso 1 Hacer
				Para j<-1 Hasta i Con Paso 1 Hacer
					Escribir  "* ", " "  Sin Saltar
				Fin Para
				Escribir " " 
			Fin Para
		2:
			Para i<-0 Hasta puntos-1 Con Paso 1 Hacer
				Para j<-0 Hasta puntos-(i+1) Con Paso 1 Hacer
					Escribir "* "," " Sin Saltar
				Fin Para
				Escribir " "
			Fin Para
		3:
			Para i<- puntos Hasta -1 Con Paso -1 Hacer
				Para j<-0 Hasta (puntos-i-1) Con Paso 1 Hacer
					Escribir  "  " Sin Saltar
				Fin Para
				Para j<-1 Hasta i Con Paso 1 Hacer
					Escribir " *" Sin Saltar
				Fin Para
				Escribir " " 
			Fin Para
		4: 
			Para i<-0 Hasta puntos Con Paso 1 Hacer
				Para j<-0 Hasta (puntos-i-1) Con Paso 1 Hacer
					Escribir  "  " Sin Saltar
				Fin Para
				Para j<-1 Hasta i Con Paso 1 Hacer
					Escribir " *" Sin Saltar
				Fin Para
				Escribir " " 
			Fin Para
	Fin Segun
FinAlgoritmo
  ```
---
---
>Algoritmo en C++
 ```C++
 #include<iostream>
using namespace std;
// Programa que muestra 4 tipos de triangulo de rectangulo

int main() {
	float i;
	float j;
	int opc;
	int puntos;
	cout << "Ingrese el numero de puntos que desee que tenga el triangulo" << endl;
	cin >> puntos;
	cout << "¿Cual de las 4 formas del Triangulo Rectangulo desea ver?" << endl;
	cout << "Triangulo Rectangulo: 1" << endl;
	cout << "   +-----------+" << endl;
	cout << "     *          " << endl;
	cout << "     * *        " << endl;
	cout << "     * * *      " << endl;
	cout << "     * * * *    " << endl;
	cout << "     * * * * *  " << endl;
	cout << "   +-----------+" << endl;
	cout << "Triangulo Rectangulo: 2" << endl;
	cout << "   +-----------+" << endl;
	cout << "     * * * * *  " << endl;
	cout << "     * * * *    " << endl;
	cout << "     * * *      " << endl;
	cout << "     * *        " << endl;
	cout << "     *          " << endl;
	cout << "   +-----------+" << endl;
	cout << "Triangulo Rectangulo: 3" << endl;
	cout << "   +-----------+" << endl;
	cout << "     * * * * *  " << endl;
	cout << "       * * * *  " << endl;
	cout << "         * * *  " << endl;
	cout << "           * *  " << endl;
	cout << "             *  " << endl;
	cout << "   +-----------+" << endl;
	cout << "Triangulo Rectangulo: 4" << endl;
	cout << "  +-----------+" << endl;
	cout << "            *  " << endl;
	cout << "          * *  " << endl;
	cout << "        * * *  " << endl;
	cout << "      * * * *  " << endl;
	cout << "    * * * * *  " << endl;
	cout << "  +-----------+" << endl;
	cin >> opc;
	switch (opc) {
	case 1:
		for (i=1; i<=puntos; ++i) {
			for (j=1; j<=i; ++j) {
				cout << "* " << " ";
			}
			cout << " " << endl;
		}
		break;
	case 2:
		for (i=0; i<=puntos-1; ++i) {
			for (j=0; j<=puntos-(i+1); ++j) {
				cout << "* " << " ";
			}
			cout << " " << endl;
		}
		break;
	case 3:
		for (i=puntos; i>=-1; --i) {
			for (j=0; j<=(puntos-i-1); ++j) {
				cout << "  ";
			}
			for (j=1; j<=i; ++j) {
				cout << " *";
			}
			cout << " " << endl;
		}
		break;
	case 4:
		for (i=0; i<=puntos; ++i) {
			for (j=0; j<=(puntos-i-1); ++j) {
				cout << "  ";
			}
			for (j=1; j<=i; ++j) {
				cout << " *";
			}
			cout << " " << endl;
		}
		break;
	}
	return 0;
}
  ```
---
---
>Algoritmo en Phyton
```Python
#Programa que muestra 4 tipos de triangulo rectangulo
if __name__ == '__main__':
	puntos = int()
	opc = int()
	print("Ingrese el numero de puntos que desee que tenga el triangulo")
	puntos = int(input())
	print("¿Cual de las 4 formas del Triangulo Rectangulo desea ver?")
	print("Triangulo Rectangulo: 1")
	print("   +-----------+")
	print("     *          ")
	print("     * *        ")
	print("     * * *      ")
	print("     * * * *    ")
	print("     * * * * *  ")
	print("   +-----------+")
	print("Triangulo Rectangulo: 2")
	print("   +-----------+")
	print("     * * * * *  ")
	print("     * * * *    ")
	print("     * * *      ")
	print("     * *        ")
	print("     *          ")
	print("   +-----------+")
	print("Triangulo Rectangulo: 3")
	print("   +-----------+")
	print("     * * * * *  ")
	print("       * * * *  ")
	print("         * * *  ")
	print("           * *  ")
	print("             *  ")
	print("   +-----------+")
	print("Triangulo Rectangulo: 4")
	print("  +-----------+")
	print("            *  ")
	print("          * *  ")
	print("        * * *  ")
	print("      * * * *  ")
	print("    * * * * *  ")
	print("  +-----------+")
	opc = int(input())
	if opc==1:
		for i in range(1,puntos+1):
			for j in range(1,i+1):
				print("* "," ", end="")
			print(" ")
	elif opc==2:
		for i in range(puntos):
			for j in range(puntos-(i+1)+1):
				print("* "," ", end="")
			print(" ")
	elif opc==3:
		for i in range(puntos,-2,-1):
			for j in range((puntos-i-1)+1):
				print("  ", end="")
			for j in range(1,i+1):
				print(" *", end="")
			print(" ")
	elif opc==4:
		for i in range(puntos+1):
			for j in range((puntos-i-1)+1):
				print("  ", end="")
			for j in range(1,i+1):
				print(" *", end="")
			print(" ")

```
  ---
  ---