# Banco de Ideas Evaluadas
**Hackathon EDU HU₿ · LABITCONF 2026**  
**Equipo:** Australianos (Mesa 5 · Hash: `0x0e652757`)  

Este documento registra cada una de las ideas analizadas por el equipo, evaluadas rigurosamente según la rúbrica oficial del jurado (5 pilares de 20 puntos = 100 puntos), los filtros eliminatorios (OpenARG, Blockchain y Factibilidad) y propuestas concretas de mejora o pivote.

---

## Idea 1: Consorcio Transparente / Expensas on-chain con IA
* **Propuesta por:** Santi Garnier (UTN)
* **Fecha de análisis:** Viernes 30 de Octubre · 12:00 hs
* **Track sugerido:** Impacto y Comunidad / Inclusión Financiera

### Resumen de la Idea
Una aplicación web para consorcios de edificios donde:
1. La administración sube facturas y tickets en foto/PDF.
2. Una IA lee, extrae datos y categoriza automáticamente los gastos (sueldos, mantenimiento, limpieza, etc.).
3. Cada gasto se ancla de forma inmutable en blockchain para auditoría pública o de los vecinos.
4. El fondo de reserva del consorcio se resguarda en stablecoins (dólar digital) para evitar su licuación inflacionaria.
5. Un chatbot con IA responde a los vecinos consultas sobre motivos y evolución de los gastos en lenguaje natural.

---

### 📊 Evaluación con la Rúbrica Oficial (Puntaje: 71 / 100)

| Criterio Oficial | Puntaje | Justificación |
| :--- | :---: | :--- |
| **1. Impacto y relevancia del problema** | **15 / 20** | **Muy cotidiano y empático:** En Argentina, más de 6 millones de personas viven en propiedad horizontal y reniegan con las expensas, falta de rendición y fondos licuados. Sin embargo, no aborda una situación de vulnerabilidad social crítica (es un dolor de clase media/alta urbana). |
| **2. Modelo de negocio** | **16 / 20** | **Claro:** Modelo SaaS B2B a administraciones de consorcio (pago mensual por unidad funcional) o % sobre el rendimiento DeFi/rendimiento del fondo de reserva. |
| **3. Pitch y comunicación (60s)** | **18 / 20** | **Excelente:** En 10 segundos cualquiera en la sala entiende el problema ("¿quién no sufrió con la liquidación de expensas de su edificio?"). Genera empatía instantánea. |
| **4. Calidad del prototipo y tecnología** | **12 / 20** | **Riesgo:** El flujo de OCR con IA es viable, pero la custodia de fondos cripto para un consorcio tiene trabas legales severas en Argentina (Ley de Propiedad Horizontal exige cuenta bancaria oficial en pesos a nombre del consorcio). |
| **5. Innovación y creatividad** | **10 / 20** | **Baja diferenciación:** "Expensas en blockchain" o "Consorcio DAO" es una idea clásica que ya se presentó en decenas de hackathons (2021-2024), y en el mercado ya existen soluciones consolidadas de gestión como *ConsorcioAbierto*, *Edilizia* u *OctoCampus*. |

---

### 🚦 Análisis de Filtros Eliminatorios

* ❌ **Filtro OpenARG (PELIGRO - OBLIGATORIO POR BASES):**  
  * *Estado:* **NO CUMPLE EN SU FORMA PURA.**  
  * *Razón:* Las expensas de un edificio privado son **datos privados de vecinos particulares**. OpenARG indexa **datos públicos del Estado argentino** (+33.000 datasets oficiales). Si la app solo procesa tickets privados de un consorcio de Caballito, **el jurado la descalifica por no estar justificada con OpenARG**.
* ⚠️ **Filtro Blockchain ("¿Por qué no alcanza con una base de datos?"):**  
  * Si el administrador malintencionado sube una factura trucha o inflada, la blockchain solo guardará un ticket trucho de forma inmutable (*"Garbage In, Garbage Out"* o el problema del oráculo). Blockchain no resuelve por sí sola la verificación física del arreglo del ascensor.
* ⚠️ **Traba Legal / Regulatoria en Argentina:**  
  * El Código Civil y Comercial (art. 2046) y el Registro Público de Administradores (RPA de CABA Ley 941) obligan a bancarizar las expensas en bancos tradicionales en pesos a nombre del consorcio (CUIT del edificio). Un consorcio no puede legalmente poner su fondo de reserva en USDT sin violar la normativa vigente.

---

### 😈 Las Preguntas Asesinas del Jurado (Abogado del Diablo)

1. **El jurado técnico de OpenARG:** *«La consigna exigía que la solución esté obligatoriamente justificada con datos de OpenARG y aplique a políticas/problemas públicos. ¿Dónde están los datos públicos en un consorcio privado?»*
2. **El jurado VC (Fede Gir / Picante):** *«Ya existen ConsorcioAbierto y 10 plataformas más de expensas claras. ¿Por qué un administrador con incentivos para ocultar cosas adoptaría voluntariamente una blockchain que lo exponga?»*
3. **El jurado legal/cripto:** *«¿Cómo resuelve el consorcio la personería jurídica para custodiar stablecoins legalmente sin que el administrador se quede con las llaves privadas?»*

---

### 🚀 Propuestas de Mejora / Pivotes para llevarla a 90+ Puntos

Para no descartar la esencia de la idea de Santi y convertirla en una candidata ganadora de EDU HU₿, proponemos **dos pivotes estratégicos**:

#### Opción A: "El Consorcio Escolar" (La Cooperadora Transparente) — *RECOMENDADA*
* **El Giro:** En vez de un edificio de departamentos, aplicarlo a las **Cooperadoras Escolares de Escuelas Públicas**.
* **El Problema:** Cada escuela pública funciona exactamente como un consorcio: directivos y cooperadoras reciben dinero del Estado, cuotas voluntarias y donaciones, pagan arreglos de gas, estufas, pintura y compra de insumos, pero conviven con desconfianza de los padres, facturas en papel borroso y fondos que se licúan.
* **Conexión OpenARG:** Se conecta con el **Padrón Oficial de Establecimientos Educativos** y los **precios de referencia de compras públicas de CABA (BAC)**. La IA lee el ticket del plomero o de la librería y lo compara en tiempo real con los precios de referencia oficiales del Estado: *"Esta cooperadora pagó la pintura 40% más barata que el precio testigo oficial"*.
* **Por qué gana:** Cumple 100% con el eje de **Educación**, resuelve el requisito de **OpenARG** y mantiene la simpleza del pitch de Santi.

#### Opción B: "Auditor de Expensas con Datos Públicos" (PropTech Cívico)
* **El Giro:** Mantener los edificios privados, pero convertir la app en un **Auditor Inteligente de Expensas alimentado por OpenARG**.
* **La Solución:** El vecino sube la liquidación de su expensa. La IA extrae los ítems y los compara contra los datasets oficiales de OpenARG:
  * Índices de inflación específicos del INDEC (rubro mantenimiento de vivienda y servicios).
  * Cuadros tarifarios oficiales de Aysa, Edenor y Metrogas de portales públicos.
  * Paritarias oficiales de encargados de edificios (SUTERH).
* **El Valor:** La app le dice al vecino: *"Tu administración aumentó el rubro limpieza un 80% este mes, cuando la paritaria oficial y la inflación del rubro en CABA fue del 12%. Te están cobrando de más."*
* **Por qué gana:** Cumple con OpenARG, protege al vecino frente a administradores abusivos y no requiere meterse en el lío regulatorio de crear wallets para consorcios.

---

### ⚖️ Veredicto
**REQUIERE PIVOTE.**  
La idea tiene excelente empatía y simplicidad comunicacional, pero tal como está formulada **quedaría descalificada por falta de OpenARG** y frenada por la regulación de consorcios. Aplicándola al **Pivote A (Cooperadoras Escolares)** o al **Pivote B (Auditor con Datos INDEC/OpenARG)**, pasa automáticamente a ser una propuesta de **90+ puntos**.

---

## Idea 2: Inclusión Financiera desde la Causa Raíz (Comprensión Lectora y Lógica Anti-Trampas)
* **Propuesta por:** Gabo / Australianos
* **Fecha de análisis:** Viernes 30 de Octubre · 12:15 hs
* **Track:** Nueva Educación (Track 2) / Inclusión Financiera (Track 1)
* **Inspiración:** Pruebas PISA / Aprender (Latam vs. Asia) + Bilinkis (*Sedentarismo Cognitivo*) + Kai-Fu Lee (*Habilidades Humanas de Razonamiento*)

### La Paradoja de Partida (El Problema Real)
> **"En Argentina y América Latina se impulsa la 'inclusión financiera' regalando billeteras virtuales a chicos desde los 13 años, mientras las pruebas PISA y Aprender demuestran que 1 de cada 2 estudiantes no comprende un texto básico ni resuelve operaciones matemáticas simples. Sin comprensión lectora ni lógica, la inclusión financiera no genera riqueza: genera ludopatía adolescente (apuestas online clandestinas), endeudamiento usurario y estafas piramidales."**

---

### Resumen de la Solución Propuesta: "Lógica Real / DecodeFin"
Una plataforma pedagógica interactiva impulsada por IA y anclada en datos reales donde los adolescentes aprenden inclusión financiera **ejercitando la comprensión de textos reales y el razonamiento lógico**:

1. **Módulo 'Cazador de Letra Chica' (Comprensión Lectora con IA):**  
   La IA alimenta al alumno con textos reales del mundo financiero (términos y condiciones de créditos rápidos, contratos de billeteras, publicidades de influencers, promociones engañosas) y lo desafía a desarmar las trampas ocultas: *"¿Dónde te cobran la tasa oculta?", "¿Qué pasa si te atrasás 1 día?", "¿Por qué esta rentabilidad es matemáticamente imposible?"*.
2. **Módulo 'Simulador Anti-Timba' (Lógica y Probabilidades - Método Singapur):**  
   Inspirado en los modelos asiáticos de aprendizaje visual-concreto: el alumno simula apuestas y préstamos viendo el valor esperado negativo y la aceleración exponencial del interés compuesto. Destruye la ilusión de la plata fácil con matemática empírica.
3. **Incentivos 'Learn-to-Earn' en Bitcoin / Lightning (Inclusión Financiera Real):**  
   A medida que el estudiante demuestra comprensión lectora y pensamiento crítico superando desafíos reales, no recibe puntos ficticios: recibe micropagos reales en satoshis (vía Lightning Network) en una billetera no custodial, aprendiendo de primera mano la diferencia entre dinero duro/ahorro soberano y deuda inflacionaria.
4. **Mapa de Vulnerabilidad Educativa (Conexión OpenARG):**  
   Tablero analítico alimentado con los **Resultados Aprender de OpenARG** (datos por partido/municipio de Lengua y Matemática) que permite a escuelas y gobiernos mapear los distritos con mayor brecha de comprensión lectora, identificando las zonas más indefensas ante estafas financieras y apuestas online.

---

### 📊 Evaluación con la Rúbrica Oficial (Puntaje: 91 / 100)

| Criterio Oficial | Puntaje | Justificación |
| :--- | :---: | :--- |
| **1. Impacto y relevancia del problema** | **20 / 20** | **Crítico y en agenda nacional:** La crisis de comprensión lectora (PISA/Aprender) combinada con la epidemia de apuestas online en adolescentes y el sobreendeudamiento es el problema socioeducativo #1 de Argentina hoy. |
| **2. Modelo de negocio** | **17 / 20** | **Muy viable y diversificado:**  <br>• B2B a Fintechs y Bancos (obligados por regulaciones de BCRA y CNV a destinar presupuesto a RSE y educación financiera real).<br>• B2G / Escuelas: Licenciamiento a colegios privados y programas ministeriales de alfabetización. |
| **3. Pitch y comunicación (60s)** | **19 / 20** | **Demoledor:** La frase *"Darle una billetera virtual a un chico que no sabe leer un contrato es darle una trampa, no una oportunidad"* captura al jurado en los primeros 5 segundos. |
| **4. Calidad del prototipo y tecnología** | **17 / 20** | **Totalmente construible en 24h:** Una web interactiva con un tutor de IA (Prompt Engineering avanzado con Grounding) que toma fragmentos reales de contratos, desafía al usuario y le otorga un comprobante o micro-satoshi por resolver la trampa. |
| **5. Innovación y creatividad** | **18 / 20** | **Altamente diferencial:** No es "otro cursito aburrido de qué es un bono o cómo abrir una cuenta". Ataca la causa raíz cognitiva (lógica + lengua) comparando el modelo latinoamericano con el método asiático. |

---

### 🚦 Análisis de Filtros Eliminatorios

* ✅ **Filtro OpenARG:**  
  * *Dataset Oficial Verificado:* `raw.cache_buenos_aires_resultados_aprender_r93dec25c45` (3.264 filas con los resultados de Aprender en Lengua y Matemática para cada partido de la Provincia de Buenos Aires: porcentaje avanzado, básico y por debajo del básico).
  * *Uso en la app:* El mapa y los niveles de dificultad del juego se calibran según la realidad educativa de cada distrito.
* ✅ **Filtro Blockchain Oficial ("¿Por qué no alcanza con una base de datos?"):**  
  * Supera la pregunta 3 del jurado: *"¿Hay plata o valor moviéndose entre personas sin intermediario?"* -> **SÍ.** El protocolo premia el esfuerzo cognitivo con micro-recompensas en satoshis reales (Lightning) y emite credenciales de alfabetización financiera inmutables (Soulbound / Badges descentralizados), enseñando autocustodia real en vez de dependencia bancaria tradicional.
* ✅ **Filtro Sedentarismo Cognitivo (Bilinkis / Sigman):**  
  * Es la encarnación exacta del libro *Artificial*: la IA no le da la respuesta al chico; **le hace preguntas incómodas y lo entrena para pensar críticamente**, combatiendo activamente el sedentarismo cognitivo.

---

### 😈 Las Preguntas Asesinas del Jurado (Abogado del Diablo)

1. **El jurado pedagógico:** *«¿Cómo garantizan que un chico de 14 años en un barrio vulnerable se siente a 'analizar contratos' en vez de seguir jugando a la ruleta online?»*  
   *Respuesta del equipo:* *«A través de gamificación agresiva: el simulador muestra la ruleta de apuestas reales desarmando el algoritmo en tiempo real para mostrar cómo la casa siempre gana, y premia con satoshis reales al que descubre el truco, utilizando la misma dopamina pero en sentido inverso: el placer de no dejarse estafar.»*
2. **El jurado técnico:** *«¿La IA no puede alucinar explicaciones financieras complejas?»*  
   *Respuesta del equipo:* *«Aplicamos Prompt Engineering con Schema Enforcement (O'Reilly): la IA trabaja sobre fragmentos cerrados de contratos reales y solo clasifica trampas pre-validadas contra reglas fijas de tasa de interés e inflación del INDEC.»*

---

### ⚖️ Veredicto
**APROBADA CON CALIFICACIÓN SOBRESALIENTE (91/100).**  
Es una idea de altísimo impacto, profunda, alineada con el track de **Nueva Educación / Inclusión Financiera**, y con un gancho de pitch que resuena profundamente en cualquier jurado.

