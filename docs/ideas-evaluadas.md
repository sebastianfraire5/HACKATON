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
