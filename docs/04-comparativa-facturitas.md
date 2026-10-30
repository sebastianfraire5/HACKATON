# Análisis Competitivo: Clara / SIRCREB Hunter vs. Facturitas.app
**Hackathon EDU HU₿ · LABITCONF 2026**  
**Equipo:** Australianos (Mesa 5 · Hash: `0x0e652757`)  
**Fecha:** Viernes 30 de Octubre · 16:40 hs  

---

## 🔎 Qué es realmente Facturitas (`facturitas.app`)

Investigamos a fondo la plataforma **Facturitas**:
* Es un bot y webapp argentina enfocada en **simplificar la emisión de facturas electrónicas de monotributistas locales** ante ARCA (ex-AFIP).
* Su propuesta de valor es emitir comprobantes (principalmente **Factura C** y notas de crédito en pesos) mediante mensajes de WhatsApp, audios o planillas de Excel para comercios, repartidores (como Rapiboy) y profesionales locales.
* Requiere que el usuario ingrese a ARCA con Clave Fiscal, delegue el servicio de WebServices de Facturación a `Facturitas S.R.L.` y cree un Punto de Venta específico.

---

## ⚔️ Matriz Comparativa: Las 6 Diferencias Fundamentales

| Dimensión | Facturitas (`facturitas.app`) | Clara / SIRCREB Hunter (Nuestro Producto) |
| :--- | :--- | :--- |
| **1. Enfoque Principal** | **Herramienta de Emisión (Teclado rápido):** Solo sirve para "empujar" facturas hacia ARCA. | **Agente Auditor y Defensor Fiscal:** Audita lo que pasa en tu cuenta bancaria y defiende tus derechos. |
| **2. Visión Bancaria (SIRCREB y Retenciones)** | ❌ **CIEGO TOTAL:** No lee extractos bancarios ni Mercado Pago. No tiene idea de si te retuvieron plata ni cuánto. | 🟢 **NATIVO:** Lee extractos bancarios (PDF/CSV) con OCR/IA y aísla cada retención indebida de Ingresos Brutos. |
| **3. Exportación de Servicios y Cripto** | ❌ **No cubre exportación:** Diseñado para cobros locales en pesos (Factura C). No maneja valuación de cobros en USDT/cripto (RG 5616/2024). | 🟢 **ESPECIALIZADO:** Conoce las zonas grises de cobro exterior, Factura E y el tipo de cambio oficial BNA vs. exchange local. |
| **4. Defensa Legal y Reclamos** | ❌ **No genera reclamos:** Si el banco te retiene $50.000 de más, Facturitas no te avisa ni te ayuda a reclamar. | 🟢 **AUTÓNOMO:** Cita el **Art. 179 inc. 21 del Código Fiscal de CABA** (exención total) y redacta la nota oficial de exclusión para AGIP/COMARB. |
| **5. Privacidad y Seguridad (Clave Fiscal)** | ⚠️ **Intrusivo:** Exige delegar permisos de WebService y administración de Clave Fiscal a un tercero. | 🟢 **Privacy-First:** El usuario solo arrastra su extracto en su navegador; no entrega claves fiscales ni tokens a nadie. |
| **6. Anclaje Blockchain (Fecha Cierta)** | ❌ **Cero Blockchain:** Es una base de datos centralizada tradicional con conexión a AFIP. | 🟢 **Fecha Cierta Inmutable:** Sella la huella SHA-256 de los reclamos y entregables en Bitcoin con **OpenTimestamps**. |

---

## 💡 Lo que Facturitas EVIDENTEMENTE NO Puede Solucionar

1. **No sabe qué pasa con la plata después de facturar:**  
   Un freelancer puede usar Facturitas para hacer su Factura E o C. Pero cuando el dinero entra al banco Galicia o Mercado Pago y **el sistema SIRCREB le debita compulsivamente el 3%**, Facturitas no tiene ojos en el banco. Para Facturitas, ese débito simplemente no existe.
2. **No frena las retenciones indebidas:**  
   No puede armar una nota de exclusión de padrón ni pedir la repetición de saldos a favor porque no es un motor de reclamos tributarios, sino un emisor de tickets.
3. **No asesora sobre normas provinciales (Ingresos Brutos):**  
   Facturitas solo habla con los servidores nacionales de ARCA (ex-AFIP). **No se conecta con los fiscos provinciales (AGIP, ARBA, COMARB)**, que es donde se produce el 80% de los abusos tributarios contra freelancers.
4. **No tiene modelo a éxito:**  
   Facturitas te cobra un abono mensual fijo solo por darte un atajo para emitir facturas (algo que en la web oficial de ARCA es gratuito). Nuestro producto cobra **comisión sobre plata real que recuperamos para el usuario**.

---

## 🚀 Cómo Podemos Mejorar Nuestro Producto con este Aprendizaje

A partir de analizar Facturitas, incorporamos **3 ventajas tácticas** que dejan a nuestro agente en otra liga:

### 1. "De la Facturación a la Cobranza Protegida" (El Loop Completo)
* Facturitas termina su trabajo cuando emite la factura.
* **Clara cierra el círculo completo:**  
  1) Te ayuda a emitir la Factura E con la cotización correcta (RG 5616).  
  2) Monitorea la acreditación bancaria: si el banco te retuvo un centavo por SIRCREB, **Clara dispara inmediatamente el contraataque legal**.

### 2. Canales Conversacionales Livianos (WhatsApp / Telegram sin delegar Clave)
* Facturitas demostró que a los usuarios les gusta usar WhatsApp.
* **Nuestra mejora:** El usuario le manda el extracto bancario en PDF por WhatsApp o chat web a Clara, y Clara le devuelve el informe de retenciones y la nota de reclamo lista, **sin necesidad de que el usuario delegue su Clave Fiscal en ARCA**.

### 3. Facturitas como Potencial Partner (No competidor)
* En el pitch podemos decir con total soltura:
  > *"Facturitas o cualquier sistema de facturación es complementario: ellos te ayudan a emitir la factura; nosotros somos el Escudo Fiscal que audita tu cuenta bancaria para que los fiscos provinciales no te confisquen el 5% de lo que facturaste."*

---

## 🎤 La Respuesta Letal para el Jurado en 30 Segundos

Si el jurado pregunta: *«¿Y cuál es la diferencia con Facturitas?»*:

> *"Facturitas es un bot de WhatsApp para emitir Factura C en ARCA para comercios y repartidores locales. Es un teclado rápido, pero es completamente ciego a lo que pasa en tu cuenta bancaria.  
> 
> Facturitas no lee extractos, no sabe qué es SIRCREB, no detecta retenciones indebidas y no conoce la exención de exportación de servicios en CABA (Art. 179 inc. 21).  
> 
> Facturitas te ayuda a **emitir comprobantes**; nosotros somos el **perro de caza que audita tu banco, frena las retenciones indebidas del 5% y te recupera la plata retenida** sellando los reclamos en Bitcoin."*
