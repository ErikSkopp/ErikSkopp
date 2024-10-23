+++
author = "eskopp"
title = "Pointer"
date = "2024-10-23"
description = "Pointer Description"
tags = [
    "C",
    "C++",
    "pointer",
    "programmierung"
]
thumbnail = "images/dollar.png"

+++

```c++

#include <iostream>
using namespace std;

int main() {
    int n;
    cout << "Gib die Anzahl der Elemente ein: ";
    cin >> n;

    // Dynamisches Array mit Pointer erstellen
    int* array = new int[n];

    // Array-Werte über den Pointer eingeben
    for (int i = 0; i < n; i++) {
        cout << "Gib Element " << i+1 << " ein: ";
        cin >> array[i];
    }

    // Array-Werte über den Pointer ausgeben
    cout << "Die eingegebenen Werte sind: ";
    for (int i = 0; i < n; i++) {
        cout << array[i] << " ";
    }
    cout << endl;

    // Dynamisch reservierten Speicher freigeben
    delete[] array;

    return 0;
}
```
