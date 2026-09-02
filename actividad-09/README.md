# Actividad 9 — Suma regresiva iterativa y recursiva

## Propósito
Implementar una suma regresiva de dos maneras: iterativa y recursiva, y validar ambas mediante pruebas automáticas.

## Problema
El programa debe leer desde teclado un entero no negativo `n` y calcular la suma `n + (n-1) + ... + 1`.

Ejemplo: para `n = 5`, el resultado es `15`.

## Contrato técnico
Debes implementar exactamente estas funciones declaradas en `include/suma_regresiva.hpp`:

```cpp
long long sumaIterativa(unsigned int n);
long long sumaRecursiva(unsigned int n);
```

Reglas:
- `sumaIterativa` debe usar un ciclo y no recursividad.
- `sumaRecursiva` debe llamarse a sí misma y tener un caso base explícito.
- Para `n = 0`, ambas funciones deben regresar `0`.
- `main.cpp` debe leer `n` desde teclado, ejecutar ambas funciones y mostrar ambos resultados.

## Archivos permitidos
Puedes modificar únicamente:
- `src/suma_regresiva.cpp`
- `src/main.cpp`
- `EXPLICACION.md`

No modifiques `include/`, `tests/`, `CMakeLists.txt` ni `.github/workflows/`.

## Ejecución local
```bash
cmake -S actividad-09 -B actividad-09/build
cmake --build actividad-09/build
ctest --test-dir actividad-09/build --output-on-failure
```

## Flujo de entrega
Implementa, prueba localmente, haz commit y push a `main`, revisa GitHub Actions, corrige si es necesario, registra el SHA final en `EXPLICACION.md` y marca Entregada en Classroom solo cuando tu versión final esté lista.

Un resultado verde en GitHub Actions es retroalimentación provisional; la calificación oficial permanece en Classroom.

## Evaluación — 100 puntos
- Implementación iterativa correcta: 25 pts.
- Implementación recursiva correcta y caso base: 25 pts.
- Lectura por teclado y ejecución de ambas versiones: 20 pts.
- Resultados correctos y pruebas automáticas: 20 pts.
- Claridad y `EXPLICACION.md`: 10 pts.
