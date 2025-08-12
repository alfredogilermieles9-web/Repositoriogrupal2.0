# Repositoriogrupal2.0
# Proyecto: Matriz Transpuesta en C++

Este proyecto contiene un programa en C++ que permite ingresar una matriz 3x3 desde el teclado, muestra la matriz original y luego imprime su matriz transpuesta.

## Descripción

- El programa solicita al usuario que ingrese 9 números para completar una matriz 3x3.
- Muestra la matriz tal como fue ingresada.
- Luego calcula y muestra la matriz transpuesta, intercambiando filas por columnas.

## Código principal

```cpp
#include <iostream>
using namespace std;

int main() {
    int numeros[3][3];

    // 1. Leer la matriz 3x3 desde el teclado
    for (int a = 0; a < 3; a++) {
        for (int b = 0; b < 3; b++) {
            cout << "Digite un numero (" << a << ") (" << b << "): ";
            cin >> numeros[a][b];
        }
    }

    // 2. Mostrar la matriz original
    cout << "\nLa matriz que ingresaste:\n";
    for (int a = 0; a < 3; a++) {
        for (int b = 0; b < 3; b++) {
            cout << numeros[a][b] << "\t";
        }
        cout << "\n";
    }

    // 3. Mostrar la matriz transpuesta
    cout << "\nTu matriz ya transpuesta:\n";
    for (int a = 0; a < 3; a++) {
        for (int b = 0; b < 3; b++) {
            cout << numeros[b][a] << "\t";
        }
        cout << "\n";
    }

    return 0;
}
