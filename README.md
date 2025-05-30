# Asistente de conceptos financieros y finanzas personales con IA Generativa
## 🤖 Inteligencia Artificial Aplicada para la Economía
## 👨‍🏫 Autor
Valentina Latorre R. 2012912974
Estudiante del curso Inteligencia Artificial Aplicada a la Economía

## 📚 Descripción del Proyecto
Es una aplicación educativa desarrollada con inteligencia artificial generativa, orientada a mejorar la alfabetización financiera de jóvenes y ciudadanos. El sistema responde preguntas en lenguaje natural y simula compras a crédito con recomendaciones personalizadas.

Este proyecto aplica conceptos clave de IA generativa como Transformers, RAG, Prompt Engineering y modelos encoder-decoder. Fue desarrollado como parte de una evaluación práctica del curso IA Aplicada a la Economía y está diseñado para ejecutarse en Google Colab con código comentado y totalmente funcional.

## 🧠 ¿Qué valor aporta este proyecto a la economía?
Ofrece explicaciones claras de términos económicos y financieros.
Promueve decisiones responsables de ahorro, inversión y crédito.
Ayuda a evitar el sobreendeudamiento desde el conocimiento.

En una economía con altos niveles de informalidad e iliquidez, herramientas como esta empoderan a los ciudadanos para tomar mejores decisiones financieras.

## ⚙️ ¿Cómo funciona?
El proyecto está construido sobre una arquitectura RAG (Retrieval-Augmented Generation) y consta de tres componentes principales:

### Recuperación de conocimiento
Se carga una base de datos CSV con temas y contenidos financieros.
Se vectorizan con all-MiniLM-L6-v2 y se indexan con FAISS.

### Generación de respuesta
Se busca el fragmento más similar a la pregunta.
Se construye un prompt contextual.
El modelo FLAN-T5-base genera una respuesta breve y clara.

### Simulador financiero
Calcula cuotas mensuales, interés total y riesgos de sobreendeudamiento.
Genera recomendaciones basadas en el ingreso del usuario.

## ✨ ¿Por qué IA Generativa?
A diferencia de la IA predictiva, la IA generativa puede adaptarse a cualquier tipo de pregunta formulada libremente y ofrecer explicaciones personalizadas, no solo etiquetas o categorías.
Se eligió FLAN-T5 por ser un modelo encoder-decoder multitécnica entrenado para seguir instrucciones. Es rápido, gratuito y altamente efectivo para tareas educativas y de conversación.

## 🧪 Prompt Engineering
### 🎯 Prompt estructurado utilizado:
```
text
Copiar
Editar
Información financiera:

{contexto recuperado}

Pregunta: {pregunta del usuario}

Respuesta en español:
```

### 📌 Técnicas utilizadas:
- Instrucción directa y clara al modelo.
- Separación entre contexto, pregunta e instrucción de idioma.
- Parámetros de generación ajustados:
temperature=0.7
top_p=0.9
max_new_tokens=100

Estas técnicas aseguran que la respuesta sea relevante, breve y en español, y evitan alucinaciones o repeticiones.

### 📊 Contenido del Repositorio
El repositorio incluye:

- 📘 EconoTutorIA_Notebook.ipynb: código documentado paso a paso

- 📁 base_conocimiento_finanzas.csv: corpus de conceptos financieros

- 📄 README.md: descripción completa del proyecto


### 📅 Estructura del Proyecto
bash
Copiar
Editar
📁 EconoTutorIA/
├── EconoTutorIA_Notebook.ipynb       # Código funcional y comentado
├── base_conocimiento_finanzas.csv    # Base de conocimiento sobre educación financiera
├── README.md                         # Este documento

### 🛠️ Requisitos Técnicos
- Python 3

- Google Colab o Jupyter Notebook

- Librerías:

`transformers`

`sentence-transformers`

`faiss-cpu`

`gradio`

`pandas, torch`

Todos los scripts funcionan sin GPU ni API externa (100% gratuito).

### 💡 Metodología aplicada
- Recuperación semántica con FAISS y embeddings

- Generación de respuestas con FLAN-T5 (Transformer)

- Ingeniería de prompts efectiva

- Simulación numérica con criterios económicos reales

### 🔎 Conceptos aplicados
- RAG (Retrieval-Augmented Generation)

- Prompt Engineering

- Modelos fundacionales y transformers

- Embeddings y búsqueda semántica

- Hiperparámetros de inferencia (temperature, top_p, max_tokens)

- Arquitectura encoder-decoder

- IA generativa vs IA predictiva



