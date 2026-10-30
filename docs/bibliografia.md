# Bibliografía Oficial y Marco de Lecturas
**Hackathon EDU HU₿ · LABITCONF 2026**  
**Equipo:** Australianos (Mesa 5 · Hash: `0x0e652757`)  

Esta selección bibliográfica fue provista por la organización y mentores del hackathon como marco conceptual y técnico de referencia. Se divide en dos pilares fundamentales: **el contorno de lo humano / neurociencia del pensamiento** y **la ingeniería rigurosa de aplicaciones con Modelos de Lenguaje (LLMs)**.

---

## 📚 Índice de Libros Recomendados

| # | Libro | Autores | Editorial | Pilar |
| :-: | :--- | :--- | :--- | :--- |
| **1** | **Artificial: La nueva inteligencia y el contorno de lo humano** | Mariano Sigman & Santiago Bilinkis | Debate | Neurociencia, Filosofía y Cognición |
| **2** | **Prompt Engineering for LLMs** | John Berryman & Albert Ziegler | O'Reilly | Diseño de Prompts y Sistemas LLM |
| **3** | **Prompt Engineering for Generative AI** | James Phoenix & Mike Taylor | O'Reilly | Fiabilidad, Salidas Estructuradas y Testing |
| **4** | **LLM Engineer's Handbook** | Paul Iusztin & Maxime Labonne | Packt | De Concepto a Producción, RAG y Agentes |
| **5** | **The Practical LLM Builder Handbook** | Guía Paso a Paso | Independiente / Tech Guide | Construcción, Entrenamiento y Despliegue |

---

## 1. Pilar Humanista y Neurocognitivo

### *Artificial: La nueva inteligencia y el contorno de lo humano*
* **Autores:** Mariano Sigman (neurocientífico) y Santiago Bilinkis (emprendedor y tecnólogo).
* **Editorial:** Debate.
* **Ejes principales:**
  * **El lenguaje como herramienta de pensamiento:** El diálogo entre humanos y máquinas reconfigura la forma en que razonamos, aprendemos y tomamos decisiones.
  * **El riesgo de la atrofia del pensamiento propio:** Si delegamos en la máquina no solo el trabajo mecánico sino el juicio, caemos en el *sedentarismo cognitivo*.
  * **El contorno de lo humano:** Lo que la tecnología nunca podrá reemplazar: la empatía, el propósito moral, el cuestionamiento crítico de la realidad y la responsabilidad sobre las decisiones públicas.
* **Por qué importa en EDU HU₿:**
  * Fundamenta por qué los proyectos de educación e impacto social no deben ser cajas negras automáticas que "reemplacen" a las personas, sino herramientas que **aumenten la capacidad de juicio y agencia ciudadana**.

---

## 2. Pilar de Ingeniería Práctica de LLMs y Prompting

### *Prompt Engineering for LLMs: The Art and Science of Building Large Language Model-Based Applications*
* **Autores:** John Berryman & Albert Ziegler.
* **Editorial:** O'Reilly.
* **Ejes principales:**
  * Dejar de ver el prompting como "arte intuitivo" y tratarlo como **ingeniería de software determinista**.
  * Técnicas de descomposición de problemas (Chain-of-Thought, ReAct, desdoblamiento de tareas complejas en micro-prompts).
  * Manejo del contexto y diseño de interfaces entre lenguaje natural y APIs tradicionales.

---

### *Prompt Engineering for Generative AI: Future-Proof Inputs for Reliable AI Outputs*
* **Autores:** James Phoenix & Mike Taylor.
* **Editorial:** O'Reilly.
* **Ejes principales:**
  * **Fiabilidad y reducción de alucinaciones:** Técnicas para obligar al modelo a fundamentar sus respuestas en fuentes de datos verificadas (Grounding).
  * **Salidas estructuradas (JSON / Schema Enforcement):** Cómo diseñar prompts que devuelvan datos predecibles para ser consumidos por un frontend o base de datos.
  * **Evaluación sistemática de prompts:** Métricas para saber si un cambio de prompt mejora o degrada la calidad de respuesta.

---

### *LLM Engineer's Handbook: Master the art of engineering large language models from concept to production*
* **Autores:** Paul Iusztin & Maxime Labonne. Prólogos de referentes de Hugging Face y Google.
* **Editorial:** Packt.
* **Ejes principales:**
  * **Arquitectura RAG (Retrieval-Augmented Generation):** Cómo indexar documentos, bases de datos o APIs para que el LLM responda con datos frescos y propios del dominio.
  * **Tool Calling y Sistemas Agénticos:** Cómo conectar un LLM a herramientas externas (exactamente como conectamos OpenARG mediante el protocolo MCP).
  * **Monitoreo, latencia y costos:** Optimizar la velocidad de respuesta y el consumo de tokens en una demo en vivo.

---

### *The Practical LLM Builder Handbook: How to Build, Train, and Deploy Your Own Large Language Models*
* **Tipo:** Manual técnico de implementación integral.
* **Ejes principales:**
  * El ciclo de vida completo de un producto con IA: desde la ingesta de datos hasta el despliegue del MVP.
  * Integración de pipelines de datos y buenas prácticas de prototipado rápido para hackathons.
  * Buenas prácticas para no sobre-complejizar la arquitectura cuando se busca entregar una demo funcional en tiempo récord.

---

## 🎯 Síntesis Metodológica para el Jurado

Esta bibliografía conecta directamente con los dos criterios técnicos de la rúbrica de evaluación:

1. **Uso ético y reflexivo de la IA (20% - Innovación y Relevancia):**  
   Basado en Sigman y Bilinkis: la IA se utiliza para visibilizar lo oculto y empoderar a la comunidad con pensamiento crítico, no para sustituir la decisión humana.
2. **Robustez y calidad técnica del prototipo (20% - Prototipo / IA):**  
   Basado en la literatura de O'Reilly y Packt: la IA no responde "al azar" ni alucina; se fundamenta en **RAG / Tool Calling sobre datos públicos reales y auditables de OpenARG**, devolviendo esquemas estructurados y verificables.
