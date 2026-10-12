# Práctica: Método de Gauss-Jordan

**Asignatura:** Métodos Numéricos (Unidad 3)[cite: 1]  
**Alumno:** Marco Antonio Pavia Flores[cite: 1]  
**Docente:** Víctor Hugo Vásquez Herrera[cite: 1]  
**Institución:** Instituto Tecnológico Superior de Xalapa (ITSX)[cite: 1]

---

## Descripción de la Estructura Modular
El proyecto está desarrollado en Java bajo una arquitectura modular y el principio de reutilización de código[cite: 1]:
* **`src/defmatrizz.java`**: Contiene la definición y el almacenamiento de la matriz aumentada $[A \vert{} b]$ del sistema de ecuaciones[cite: 1].
* **`src/Gauss.java`**: Contiene el método de Eliminación Gaussiana simple (`eliminacionGaussiana`), encargado de realizar la fase de triangulación superior[cite: 1].
* **`src/GaussJordan.java`**: Reutiliza la triangulación superior anterior, implementa la normalización de pivotes a la unidad y ejecuta el barrido superior para transformar la matriz en una matriz identidad, obteniendo el vector de soluciones de manera directa[cite: 1].
* **`src/Lanzador_GaussJordan.java`**: Clase principal (`main`) que coordina la ejecución de los módulos y despliega los resultados[cite: 1].

---

##  Pasos para Compilar y Ejecutar en Java

1. Asegúrate de tener instalado **Java JDK** en tu computadora.
2. Abre tu terminal o línea de comandos en la carpeta raíz del proyecto (donde se encuentra el paquete `Ecuaciones_lineales`).
3. Compila todos los archivos fuente con el siguiente comando:
   ```bash
   javac Ecuaciones_lineales/*.java