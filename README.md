# README-T-cnico-Gestor-de-Tareas-con-Tkinter-Persistencia-y-Strategy-Pattern
Aplicación de escritorio para gestionar tareas personales y académicas. Incluye interfaz gráfica, persistencia flexible y priorización inteligente mediante Strategy Pattern.
Descripción

Este proyecto implementa un gestor de tareas con interfaz gráfica hecha en Tkinter, almacenamiento mediante JSON, CSV o SQLite y un sistema de priorización inteligente basado en Strategy Pattern.

Permite:

✔ Crear
✔ Editar
✔ Eliminar
✔ Filtrar
✔ Ordenar
✔ Priorizar tareas según distintas estrategias

El diseño sigue principios de ingeniería de software:

Modularidad

Encapsulamiento

Separación de responsabilidades

Patrones de diseño (Strategy, MVC/MVVM adaptado, DAO)

gestor_tareas/
│
├── src/
├── tests/
├── docs/

🛠️ Instalación
1️⃣ Clonar repositorio
git clone <URL_DEL_REPO>
cd gestor_tareas

2️⃣ Crear entorno virtual (opcional)
python -m venv venv
source venv/bin/activate    # Linux/Mac
venv\Scripts\activate       # Windows

3️⃣ Instalar dependencias
pip install -r requirements.txt

▶️ Ejecución
python src/main.py

🎨 Interfaz (Tkinter)

La aplicación incluye:

Ventana principal con lista de tareas

Formulario de creación/edición

Botones y menús para filtrar/ordenar

Selector de estrategia de priorización

Scrollbars y layouts responsivos

(Agrega capturas si deseas — puedo generarte maquetas de UI)

🧠 Módulo de Priorización Inteligente (Strategy Pattern)
Estrategias incluidas:
Estrategia	Descripción
DateStrategy	Prioriza según fecha límite (más urgente = mayor prioridad)
CategoryStrategy	Prioriza según jerarquía de categorías
ManualStrategy	El usuario asigna la prioridad
Diagrama del patrón Strategy
PrioritizationStrategy (interface)
│
├── DateStrategy
├── CategoryStrategy
└── ManualStrategy

📌 Diseño del Sistema
Patrones utilizados

Strategy → Priorización intercambiable

DAO/Data Access Layer → Manejo de persistencia

MVC/MVVM → Separación GUI / lógica / datos

Factory (opcional) → Selección del tipo de almacenamiento

Diagrama de Clases (UML)

(Ideal para incluir como imagen)
Archivo: docs/diagrama_clases_uml.png

🧪 Pruebas Unitarias

Ejecutar pruebas:

pytest tests/


Incluye pruebas de:

Validación de tareas

Estrategias de priorización

Gestión de tareas

Persistencia JSON / CSV / SQLite

📄 Casos de Uso

Resumen:

Crear tarea

Editar tarea

Eliminar tarea

Filtrar tareas

Ordenar por distintos criterios

Cambiar estrategia de priorización
Documentos completos:
/docs/casos_de_uso.pdf

🤝 Contribuir

Crear una rama nueva:

git checkout -b feature/nueva-funcionalidad


Hacer cambios y confirmar:

git commit -m "Descripción clara de cambios"


Subir rama:

git push origin feature/nueva-funcionalidad


Crear Pull Request

📜 Licencia

Uso académico permitido.
Puedes modificar y distribuir con fines educ
