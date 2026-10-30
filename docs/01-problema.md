# Bloque 1: El Problema
**Hackathon EDU HU₿ · LABITCONF 2026**  
**Equipo:** Australianos (Mesa 5 · Hash: `0x0e652757`)  
**Ejes:** Educación · Pobreza · Gasto Público  
**Estado:** Bloque 1 Minado (Vie 11:00 a 12:30)

---

## 1. Lluvia de 5 Problemas Concretos en Argentina

Analizamos problemas cotidianos reales donde se cruzan la educación, la vulnerabilidad socioeconómica y el uso de los fondos públicos:

1. **Opacidad y degradación en la comida que reciben los chicos en escuelas públicas:**  
   En las escuelas públicas de contextos vulnerables, la comida escolar (vianda o comedor) es muchas veces la única nutrición diaria asegurada de los alumnos. Sin embargo, los alimentos llegan con bajo valor nutricional, porciones reducidas o en mal estado, y las familias y directores no tienen capacidad de auditar ni validar lo que el Estado paga a los concesionarios antes de la liquidación de los contratos.

2. **Deserción en la secundaria por necesidad urgente de generar ingresos informales:**  
   En hogares bajo la línea de pobreza, los adolescentes abandonan la escuela al terminar la primaria o durante los primeros años de la secundaria porque el costo de oportunidad de asistir a clases es superior a salir a changuear, sumado a que las becas estatales sufren demoras burocráticas, desfasaje frente a la inflación y trabas de cobro.

3. **Asimetría extrema en la infraestructura y vacantes entre zonas ricas y vulnerables ("Desiertos Educativos"):**  
   En las zonas de mayor pobreza urbana (sur de la Ciudad de Buenos Aires y 2do/3er cordón del Conurbano Bonaerense), miles de familias no consiguen vacantes en salas de 3, 4 y 5 años ni en escuelas técnicas, mientras que en zonas de mayores ingresos sobran vacantes o las partidas de mantenimiento se asignan de forma centralizada sin priorizar la urgencia real del territorio.

4. **Burocracia y trabas para que las cooperadoras y comunidades escolares financien mejoras directas:**  
   Las cooperadoras escolares y directivos carecen de autonomía financiera y sufren trabas bancarias e impositivas severas para administrar fondos propios, recibir donaciones directas o ejecutar reparaciones edilicias urgentes (techos, gas, estufas, conectividad), dependiendo de partidas centralizadas que tardan meses en llegar.

5. **Inconsistencia entre lo presupuestado y lo efectivamente ejecutado en equipamiento y conectividad escolar:**  
   Se anuncian y aprueban programas presupuestarios millonarios para equipamiento informático, internet y material pedagógico en escuelas de barrios populares, pero la ejecución real sufre subejecución crónica o desvíos burocráticos, dejando a las escuelas periféricas sin conectividad básica.

---

## 2. El Problema Elegido

Aplicando la pregunta filtro: **¿Esto le pasa a alguien de verdad, hoy?**  
Sí, le pasa todos los días a millones de niños y niñas en las escuelas públicas más vulnerables del país, a sus directores y a sus familias.

### Formulación en una sola frase (sin nombrar tecnología)
> **"Los estudiantes en situación de pobreza en las escuelas públicas reciben una alimentación escolar deficiente e irregular porque las comunidades escolares no tienen forma de auditar ni certificar el cumplimiento de los contratos de compra que el Estado paga a las empresas proveedoras."**

*(Cumple la regla: no dice "falta una app", ni "falta una blockchain", ni nombra software; describe un dolor real y estructural).*

---

## 3. Respaldo Obligatorio con Datos Oficiales de OpenARG

Validamos la existencia y magnitud de este problema consultando el catálogo oficial indexado en **OpenARG**:

### Dato A: Magnitud de la población afectada (INDEC / EPH)
* **Dataset:** *INDEC - Informe de Pobreza — 31 aglomerados urbanos — Cuadro 1* (vía OpenARG: `raw.cache_indec_pobreza_informe_cuadro_1`).
* **Dato oficial:** 
  * En el 1er semestre de 2024 la pobreza en personas alcanzó el **52,9%**, y la indigencia trepó al **13,6%**.
  * En niños y adolescentes (0 a 14 años), la pobreza supera el **66%** en los centros urbanos.
  * **Impacto real:** Para más de la mitad de los chicos escolarizados en aglomerados urbanos de Argentina, la ración del comedor o vianda escolar no es un complemento: **es el aporte calórico y proteico central de su jornada**.

### Dato B: Volumen de compras y contratos públicos en juego (CABA / BAC)
* **Dataset:** *Buenos Aires Compras - Contracts* (vía OpenARG: `raw.bac__buenos_aires_compras_contracts__45b499b0__v2`).
* **Dato oficial:** 
  * El sistema registra más de **500.000 contratos** de compras y suministros públicos en estándar internacional OCDS.
  * El rubro de suministro de alimentos, raciones y viandas representa partidas presupuestarias de miles de millones de pesos licitadas a un grupo reducido de concesionarias.
  * **Falla del sistema:** El circuito de compra pública es 100% administrativo y burocrático (expediente, orden de compra y factura firmada entre funcionarios y contratistas). **La comunidad escolar (docentes, cooperadoras y familias) no forma parte del circuito de validación.** El Estado paga a 30-90 días contra remito administrativo, aunque la comida haya llegado incompleta, fría o con fruta podrida.

### Dato C: Cobertura territorial (Padrón Nacional de Escuelas)
* **Dataset:** *Padrón Oficial de Establecimientos Educativos* (vía OpenARG: `cache_datos_gob_ar_padr_n_oficial_de_establecimient_r0ccb304b55`).
* **Dato oficial:** Registra más de **61.800 establecimientos educativos** en Argentina, de los cuales miles cuentan con servicio de comedor o copa de leche bajo esquemas de gestión descentralizada opaca.

---

## 4. Los 5 Porqués (Causa Raíz)

1. **¿Por qué los chicos en escuelas vulnerables comen mal o reciben viandas insuficientes?**  
   Porque los concesionarios envían porciones reducidas, sustituyen ingredientes nutritivos por carbohidratos baratos o entregan mercadería en mal estado.
2. **¿Por qué los concesionarios pueden hacer eso sin consecuencias inmediatas?**  
   Porque los controles estatales de bromatología y auditoría física son esporádicos, tardíos y cubren menos del 5% de las escuelas al año.
3. **¿Por qué las quejas de los directores y familias no frenan el cobro de esas empresas?**  
   Porque el circuito de pago de contrataciones públicas está desacoplado de la conformidad de recepción de la comunidad escolar: el expediente se aprueba en el ministerio con firmas burocráticas mientras los reclamos quedan cajoneados en actas en papel.
4. **¿Por qué la comunidad escolar no tiene poder de veto o penalidad sobre el contrato?**  
   Porque la información de los pliegos (qué menú exacto se licitó, cuánto pesa cada ración, cuánto cobró el proveedor por ración) está dispersa, en formatos técnicos inaccesibles y sin mecanismos vinculantes de reporte directo.
5. **¿Por qué pasa esto en el fondo? (Causa Raíz):**  
   **Existe una asimetría de información y una desconexión total entre quien paga (el funcionario en el ministerio), quien cobra (el proveedor) y quien consume el servicio (el estudiante en el aula). Quien sufre el mal servicio no tiene ningún mecanismo verificable para auditar el cumplimiento del gasto público.**

---

## 5. Criterio de "Bloque Minado"

- [x] **Entra en una frase clara.**
- [x] **No menciona tecnología** (ni blockchain, ni app, ni tokens).
- [x] **Respaldado obligatoriamente con datos duros de OpenARG** (INDEC + BAC + Padrón de Escuelas).
- [x] **Relevante para LABITCONF:** Plantea un problema de **asimetría de información, rendición de cuentas e intermediación burocrática del dinero público**, preparando el terreno para una solución que requiera consenso ciudadano, trazabilidad inmutable o incentivos descentralizados (bloque 3).
