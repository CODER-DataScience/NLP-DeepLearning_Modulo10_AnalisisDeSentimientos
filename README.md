# Módulo 10 – Tipos de Análisis de Sentimientos

Este proyecto implementa dos enfoques clave de NLP aplicados a reseñas multilingües:

- **Análisis de sentimiento general**: valoración global de un texto (positivo/negativo/neutro o en estrellas).
- **Análisis basado en aspectos (ABSA)**: identificación de atributos específicos (ej. cámara, batería, precio) y asignación de sentimiento individual.

---

## Objetivos del módulo
- Diferenciar entre análisis general y ABSA.
- Implementar un pipeline multilingüe con reseñas en español e inglés.
- Visualizar resultados por aspecto para detectar fortalezas y debilidades.
- Documentar cada paso con Markdown para garantizar reproducibilidad y auditabilidad.

---

## Contenido del repositorio
- `README.md` → documentación principal del módulo.
- `Entrega_Modulo10.ipynb` → notebook con implementación paso a paso.
- `data/` → dataset de reseñas multilingües (opcional).
- `images/` → gráficos exportados del notebook (ej. sentimiento por aspecto).
- `docs/` → resumen teórico del módulo en Markdown (opcional).

---

## Ejercicio práctico

1. **Instalación de librerías**  
   `transformers`, `torch`, `pandas`, `matplotlib`, `seaborn`, `spacy`.

2. **Dataset multilingüe**  
   Reseñas en español e inglés con múltiples aspectos.

3. **Análisis general**  
   Modelo multilingüe: `nlptown/bert-base-multilingual-uncased-sentiment`.

4. **Definición de aspectos de negocio**  
   Cámara, batería, envío, soporte, precio, calidad, rendimiento.

5. **Modelo por aspecto**  
   `distilbert-base-uncased-finetuned-sst-2-english`.

6. **Extracción de sentimiento por aspecto**  
   Tabla con texto, aspecto, sentimiento y confianza.

7. **Visualización**  
   Gráfico de barras mostrando distribución de sentimientos por aspecto.

8. **Comparación de enfoques**  
   Ejemplo práctico mostrando diferencia entre análisis general y ABSA.

---

## Conclusiones

- **Fortalezas**: cámara, calidad, rendimiento.  
- **Debilidades**: batería, logística de entrega.  
- **Variables sensibles**: precio y soporte al cliente (opiniones mixtas).  

### Insight general:  
El análisis general ofrece una visión panorámica, mientras que ABSA permite un **zoom detallado** en cada componente, revelando oportunidades de mejora y diferenciación estratégica.

---

## Aplicaciones reales
- **Comercio electrónico**: identificar qué características generan satisfacción o insatisfacción.  
- **Empresas globales**: integrar feedback en múltiples idiomas para obtener insights comparables.  
- **Marketing internacional**: evaluar aspectos específicos en diferentes culturas y mercados.  

---

## Ejecución

1. Clonar el repositorio:
   ```bash
   git clone https://github.com/CODER-DataScience/NLP-DeepLearning_Modulo10_AnalisisDeSentimientos.git
