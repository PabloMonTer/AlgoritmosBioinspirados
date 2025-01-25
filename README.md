# Algoritmos Bioinspirados

Este proyecto aborda la resolución del Problema del Viajante de Comercio (TSP) utilizando enfoques bioinspirados, específicamente el Algoritmo de Colonia de Hormigas (ACO) y el Algoritmo Genético (GA). El objetivo del problema es encontrar la ruta más corta que un viajante debe seguir para visitar un conjunto de ciudades, visitando cada una exactamente una vez y regresando al punto de inicio.

## Metodología
El proyecto se desarrolló utilizando dos métodos bioinspirados conocidos por su capacidad para encontrar soluciones aproximadas en problemas de optimización complejos:

### 1. Algoritmo de Colonia de Hormigas (ACO)
El Algoritmo de Colonia de Hormigas (ACO) es un algoritmo de optimización basado en el comportamiento colectivo de las hormigas en la naturaleza. En el ACO, se simula la búsqueda de rutas de un grupo de hormigas en un entorno donde cada hormiga va depositando feromonas en su camino. Las hormigas más exitosas (que recorren rutas más cortas) dejan una mayor cantidad de feromonas, lo que guía a otras hormigas a seguir rutas similares.

Pasos principales del algoritmo:
- Inicialización de las hormigas en posiciones aleatorias.
- Las hormigas se desplazan por los nodos, eligiendo los próximos nodos basándose en una combinación de la cantidad de feromonas y la distancia.
- Se actualiza la cantidad de feromonas en las rutas recorridas, favoreciendo aquellas rutas que han mostrado ser mejores.
Repetición del proceso para varias iteraciones hasta que se converge a una solución óptima o subóptima.

### 2. Algoritmo Genético (GA)
El Algoritmo Genético (GA) es un algoritmo de optimización basado en los principios de la selección natural y evolución. En este enfoque, se simula la evolución de una población de soluciones mediante procesos como la selección, cruce (crossover) y mutación, con el objetivo de encontrar la mejor solución posible.

Pasos principales del algoritmo:
- Inicialización: Se genera una población inicial de soluciones.
- Selección: Se seleccionan las soluciones más prometedoras (con base en el menor costo de viaje) para formar una nueva población.
- Cruzamiento (Crossover): Se combinan dos soluciones (padres) para crear una nueva solución (hijo).
- Mutación: Se realizan pequeñas modificaciones en una solución (por ejemplo, intercambiando el orden de dos ciudades en la ruta).
Este proceso se repite a lo largo de varias generaciones hasta que se alcanza una solución lo suficientemente buena.

### 3. Comparación de los Modelos
Ambos modelos fueron evaluados utilizando el conjunto de datos de las ciudades de TSP, y se compararon en cuanto a:

Calidad de la Solución: Medida en términos de la longitud total de la ruta encontrada.
Tiempo de Ejecución: Para evaluar la eficiencia de cada algoritmo en cuanto a la rapidez con que encuentran una solución.
Convergencia: Cuán rápido ambos algoritmos llegaron a soluciones cercanas a las óptimas.
