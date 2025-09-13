# Generación de Contenido de Marketing con IA para ESU Analytics

## 📌 Resumen
Este proyecto presenta el desarrollo de una solución basada en **Inteligencia Artificial generativa** para la creación de contenido de marketing digital orientado a **PyMEs**. La propuesta busca apoyar la estrategia de comunicación de **ESU Analytics**, consultora especializada en profesionalizar la gestión de datos en los sectores manufacturero y comercial.  

El trabajo integra modelos de **texto–texto** y **texto–imagen**, aplicando técnicas de *Fast Prompting* (zero-shot y one-shot) para generar publicaciones en LinkedIn acompañadas de imágenes conceptuales. El sistema desarrollado garantiza **eficiencia en costos** (control de tokens), **trazabilidad de resultados** (exportación de inputs, outputs y métricas) y una **metodología reproducible** adaptable a diferentes temáticas comerciales.  

---

## 📖 Introducción

### Nombre del proyecto
**Generación de Contenido de Marketing con IA para ESU Analytics**

### Presentación del problema
Las PyMEs suelen tener dificultades para comunicar, de forma clara y atractiva, la importancia de la gestión de datos aplicada a su negocio. Esto limita su capacidad de mostrar valor frente a clientes y socios estratégicos, afectando su competitividad. Resolver esta problemática resulta clave para mejorar la visibilidad digital y el posicionamiento de ESU Analytics como consultora especializada.  

### Desarrollo de la propuesta de solución
La solución consiste en un flujo automatizado de generación de contenido:  
- **Posts de LinkedIn** creados mediante `gpt-4o-mini`, usando briefs personalizables y técnicas de *Fast Prompting*.  
- **Imágenes conceptuales** generadas con `gpt-image-1`, en estilos consistentes (realista o Pixar/clay 3D), evitando la necesidad de diseño manual.  
- **Exportación automática** de cada ejecución en formatos `.json` y `.md`, incluyendo trazabilidad completa de inputs, outputs y métricas.  

### Justificación de la viabilidad
El proyecto es viable técnica y económicamente porque:  
- Utiliza **modelos livianos y accesibles** (`gpt-4o-mini`), con límites de tokens para reducir costos.  
- Se implementa en **Python y Jupyter Notebook**, con librerías estándar (`dotenv`, `tiktoken`, etc.).  
- Se ajusta al tiempo disponible y muestra resultados aplicables en un caso profesional real (marketing digital de ESU Analytics).  

---

## 🎯 Objetivos
- Generar contenido de LinkedIn profesional y atractivo para PyMEs.  
- Aplicar técnicas de *Fast Prompting* (zero-shot y one-shot).  
- Integrar modelos de **texto–texto** y **texto–imagen** en un único flujo.  
- Exportar y registrar cada ejecución para garantizar trazabilidad.  
- Demostrar la viabilidad de la IA generativa en un caso real de consultoría.  

---

## 🛠️ Metodología
1. **Definición de briefs** con parámetros clave (tema, objetivo, audiencia, insight, evidencia, CTA, restricciones).  
2. **Construcción de prompts dinámicos** en formato JSON, listos para la API.  
3. **Generación de publicaciones** con `gpt-4o-mini`, usando configuraciones con límite de tokens.  
4. **Exportación automática** de resultados en `.json` (trazabilidad) y `.md` (texto final).  
5. **Generación de imágenes conceptuales** con `gpt-image-1`, en estilos controlados y sin texto.  
6. **Evaluación de resultados** en base a claridad, coherencia y costos de uso.  

---

## 🧰 Herramientas y tecnologías
- **OpenAI API**  
  - `gpt-4o-mini` (texto–texto).  
  - `gpt-image-1` (texto–imagen).  
- **Técnicas de prompting**  
  - *Zero-shot prompting*.  
  - *One-shot prompting*.  
- **Python / Jupyter Notebook**  
- Librerías: `dotenv`, `tiktoken`, `json`, `os`, `re`.  

---

## 💻 Implementación
El notebook incluye:  
- Definición de briefs personalizables.  
- Funciones para construir prompts, generar publicaciones y medir tokens.  
- Exportación automática de resultados en `Exportado/`.  
- Generación de imágenes conceptuales con prompts diseñados para consistencia visual.  

Ejemplo de prompt de imagen:  
- Ilustración 3D estilo Pixar / clay render, colores vibrantes y corporativos (azules, naranjas, verdes). 
- Escenario: oficina moderna, escritorio con laptop y un gran tablero de pared lleno de gráficos abstractos (barras, tortas, flechas de tendencia). 
- Restricciones: sin personas, sin texto, sin números, sin logotipos.

---

## 📊 Resultados
- Se generaron publicaciones de LinkedIn alineadas con diferentes briefs (ventas, estrategia comercial, automatización, finanzas).  
- Cada post fue exportado con su trazabilidad completa.  
- Se produjeron imágenes acompañantes en estilos realista y Pixar/clay 3D.  
- Los costos de uso de la API fueron controlados gracias a la gestión de tokens.  
- Los resultados mostraron consistencia en el estilo y relevancia para la audiencia objetivo.  

---

## ✅ Conclusiones
El proyecto alcanzó los objetivos planteados:  
- Se resolvió el problema de generar contenido claro y atractivo para PyMEs con IA.  
- Se aplicaron técnicas de *Fast Prompting* que mejoraron claridad y eficiencia.  
- Se integraron modelos de texto–texto y texto–imagen de forma efectiva.  
- Se logró trazabilidad y control de costos en todo el flujo.  

Los resultados evidencian que es posible establecer un sistema **escalable, económico y orientado a resultados**, que potencia la visibilidad digital y la captación de clientes de ESU Analytics.  

### **Próximos pasos sugeridos:**  
- Ampliar el set de briefs a otras áreas de gestión PyME.  
- Realizar pruebas A/B con variaciones de estilo.  
- Medir métricas reales en redes sociales para validar impacto.  

---

## 📚 Referencias
- Documentación oficial de OpenAI: https://platform.openai.com/docs
- Librería tiktoken: https://github.com/openai/tiktoken
