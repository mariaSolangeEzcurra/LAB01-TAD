1. Descripción del Proyecto

El presente proyecto consiste en el desarrollo de un sistema de recomendación de cursos universitarios, orientado a estudiantes de la Escuela Profesional de Ingeniería de Sistemas (EPIS). El sistema utiliza ChromaDB como base de datos vectorial para implementar un mecanismo de búsqueda semántica, permitiendo recomendar cursos en función de los intereses y perfil del usuario.
El enfoque aplicado combina técnicas de representación vectorial de texto (embeddings) con filtrado estructurado mediante metadatos, logrando así una búsqueda híbrida más precisa y contextualizada.

2. Tecnologías Utilizadas

* Lenguaje de programación: Python 3.x
* Base de datos vectorial: ChromaDB
* Modelo de embeddings: Sentence Transformers

3. Estructura del Sistema
El sistema cuenta con una base de datos persistente que almacena una colección denominada “cursos_epis”, la cual contiene 20 cursos ficticios del área de Ingeniería de Sistemas. Cada curso incluye la siguiente información:

* Nombre del curso
* Descripción 
* Número de créditos
* Semestre académico (1-9)
* Área (básica, especialidad, electivo)
* Prerrequisitos

4. Funcionalidades Implementadas

 4.1 Recomendación de cursos: Permite sugerir cursos en función de los intereses del estudiante y su semestre actual, aplicando filtrado por semestre y similitud semántica.
 4.2 Búsqueda de cursos similares: Dado el nombre de un curso, el sistema identifica otros cursos con contenido temáticamente similar utilizando embeddings.
 4.3 Búsqueda por perfil: Permite encontrar cursos adecuados a partir de un conjunto de habilidades o intereses del usuario, filtrando adicionalmente por área académica.
 4.4 Interfaz de usuario: Se implementó una interfaz de línea de comandos (CLI) que permite al usuario interactuar con el sistema mediante un menú de opciones.

5. Ejecución del Sistema
  Para ejecutar el sistema, se deben seguir los siguientes pasos:
1. Instalar las dependencias necesarias:
```
pip install chromadb sentence-transformers
```
2. Ejecutar el archivo principal:
```
python main.py
```
3. Interactuar con el menú en consola:
```
===== SISTEMA DE RECOMENDACIÓN =====
1. Recomendar cursos
2. Cursos similares
3. Buscar por perfil
4. Salir
```

