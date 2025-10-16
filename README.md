# Curso de Prompt Engineering

## Prompts efectivos

**Transforma tu Forma de Interactuar con la IA** 

La inteligencia artificial está cambiando la forma en que trabajamos, aprendemos y creamos. Sin embargo, muchas personas se quedan atrapadas en respuestas genéricas o poco útiles por no saber comunicarse correctamente con los modelos de lenguaje. ¿Te ha pasado? La clave está en el **prompt engineering**, una disciplina que permite obtener respuestas precisas, creativas y alineadas con lo que realmente necesitas.  

En este curso, aprenderás a estructurar tus prompts en cuatro componentes esenciales:  
- **Rol**: Asignar una identidad experta al modelo, como "especialista en marketing B2B", para alinear el tono y el criterio de las respuestas.  
- **Enfoque**: Definir acciones concretas con verbos específicos, como "crear una publicación en LinkedIn" o "sintetizar un informe".  
- **Límites**: Establecer reglas claras de formato, tono y extensión para evitar divagaciones y garantizar precisión.  
- **Memoria/Contexto**: Proporcionar información relevante, como el funcionamiento de un software SaaS, para enriquecer las respuestas y evitar generalidades.  

Además, explorarás cómo seleccionar el modelo adecuado según la tarea, descomponer problemas complejos en pasos manejables y equilibrar creatividad con precisión para minimizar errores o "alucinaciones" de la IA.  

**Primera Práctica: Comparando un Prompt Efectivo vs. Uno No Efectivo**  

Sigue estos pasos para experimentar la diferencia entre un prompt bien estructurado y uno vago:  

1. **Prompt No Efectivo**  
   Utiliza un prompt sin estructura:  
   ```  
   Habla de mi software contable en LinkedIn.  
   ```  
   Resultado:

    >Claro, aquí tienes un ejemplo de publicación para LinkedIn hablando de tu software contable, con un tono profesional y enfocado en destacar su valor:
    >
    >---
    >
    >💼 Transformar la contabilidad en una tarea simple, rápida y confiable ya no es un deseo: es una realidad.
    >
    >Presentamos nuestro software contable, diseñado para facilitar la gestión financiera de empresas que buscan eficiencia, control y crecimiento. Automatiza procesos clave, reduce errores y ofrece información en tiempo real para una toma de decisiones más inteligente.
    >
    >✅ Registro contable automatizado
    >✅ Reportes financieros claros y personalizables
    >✅ Integración bancaria
    >✅ Gestión de impuestos y cumplimiento fiscal
    >✅ Accesible desde cualquier lugar, en cualquier momento
    >
    >Más que un software, es una herramienta de transformación digital para profesionales contables y empresas que exigen resultados.
    >
    >Estamos listos para llevar tu contabilidad al siguiente nivel.
    >#SoftwareContable #TransformaciónDigital #FinanzasEmpresariales #Innovación #ContabilidadInteligente
    >
    >---
    >
    >¿Quieres que lo adapte a un tono más informal, técnico o con foco en algún beneficio específico? También puedo ayudarte a crear una imagen o gráfico que acompañe la publicación.



2. **Prompt Efectivo**  
   Usa esta estructura organizada:  
   ```
   Actúa como especialista en marketing en B2B.  
 
   Crea una publicación en LinkedIn acerca de mi producto.  

   La publicación no puede tener más de 150 caracteres y debe usar un lenguaje simple, concreto y coloquial.  

   Mi producto es un software as a service que automatiza el proceso contable de tu empresa.  
   ```  
   Resultado:

   >🚀 Ahorra tiempo y evita errores: nuestro software contable automatiza todo tu proceso financiero. ¡Contabilidad sin estrés! 💼✨

    Estructura del prompt:

    * [Rol]  
        Actúa como especialista en marketing en B2B.  
    
    * [Enfoque]  
        Crea una publicación en LinkedIn acerca de mi producto.  
    
    * [Límites]  
        La publicación no puede tener más de 150 caracteres y debe usar un lenguaje simple, concreto y coloquial.  
    
    * [Contexto]  
        Mi producto es un software as a service que automatiza el proceso contable de tu empresa.

3. **Compara los Resultados** 
   - **No efectivo**: Genérico, vago y sin impacto.  
   - **Efectivo**: Mensaje claro, persuasivo y dentro de los límites.  
    

Reflexiona: ¿Cuál comunica mejor el valor del producto? Con esta práctica, verás cómo la estructura transforma completamente los resultados. ¡Sigue explorando!


---

## Análisis de Documentos: 
**De Preguntas Vagas a Resultados Accionables**  

Ahora exploraremos cómo aplicar los principios del prompt engineering para analizar documentos y extraer insights valiosos. La clave está en transformar consultas genéricas en instrucciones específicas que la IA pueda procesar de manera eficiente.

### De lo General a lo Específico

El verdadero poder de los LLMs se revela cuando trabajamos con documentos largos. Veamos un caso práctico basado en un reporte real de McKinsey sobre inteligencia artificial:

**Descarga el documento 👉️ [Aqui](./src/docs/the-state-of-ai-how-organizations-are-rewiring-to-capture-value_final.pdf) 👈️**

**Ejemplo de Progresión en el Prompting:**

1. **Primer Prompt (Genérico):**
   
   sube el documento a ChatGPT [the-state-of-ai-how-organizations-are-rewiring-to-capture-value_final.pdf]

   ```
   ¿de qué trata este reporte?
   ```
   *Resultado: Un resumen general del contenido, útil pero limitado.*

2. **Segundo Prompt (Con Contexto Personal):**
   ```
   Ok, esto fue útil pero quiero que me des los 3 puntos más valiosos para mi.
   
   Te cuento de mi, Jacobo Cosme y soy el Chief Product Officer de Conversa, la escuela de computación e inglés más grande de México. Nosotros nos enfocamos en enseñar programación, inteligencia artificial, diseño, marketing, negocios, inglés y todas las habilidades de tecnología que necesitan los profesionales de hoy en día.
   ```
   *Resultado: La IA ahora puede priorizar información relevante para tu contexto específico.*

3. **Tercer Prompt (Formato y Límites):**
   ```
   Me suena lo del plan, pero quiero que me lo des en bullet points, concretos, concisos y accionables. No me expliques todo el contexto, dime el insight y la recomendación directa. Si tengo preguntas, te las haré. No superes mas de 500 caracteres.
   ```
   *Resultado: Respuestas enfocadas, listas para implementar.*

4. **Cuarto Prompt (Microaclaración):**
   ```
   explicame a que te refieres con esto. Recuerda ser conciso
   ```
   *Resultado: Aclaración puntual sobre términos complejos sin divagaciones.*

5. **Quinto Prompt (Validación con Fuente):**
   ```
   en que página del reporte esta lo de etica de AI?
   ```
   *Resultado: Referencia específica para verificar la información.*

### El Arte de la Iteración: Prompt Shadowing

Este proceso de refinamiento progresivo se conoce como **prompt shadowing**: trabajar con la IA hasta perfeccionar formato, tono y enfoque. La magia ocurre cuando convertimos esta iteración en un prompt maestro reutilizable.

**Prompt Ganador Final:**
```
Soy Jacobo Cosme, Chief Product Officer de Conversa. Analiza este reporte y dame los 3 insights más relevantes para mi rol en educación tecnológica. Formato: bullets concretos, accionables, máximo 500 caracteres. Incluye referencias a páginas sobre ética y gobernanza de IA.
```

### Práctica: Comparando Enfoques

**Ejercicio de Análisis Documental:**

1. **Prompt No Estructurado:**
   ```
   Lee este PDF y dime qué hay importante.
   ```
   *Resultado: Resumen genérico, sin contexto personal, sin formato específico.*

2. **Prompt Estructurado (Usando la Fórmula Maestra):**
   ```
   [Rol] Eres un consultor especializado en educación tecnológica
   [Enfoque] Analiza este reporte y extrae los 3 puntos más relevantes
   [Límites] Máximo 500 caracteres, formato bullet points, lenguaje accionable
   [Contexto] Soy CPO de una escuela de tecnología en México, enfocado en programas de IA
   ```
   *Resultado: Insights personalizados, recomendaciones ejecutivas, referencias específicas.*

**Compara los resultados:**
- ¿Cuál te da información que puedes usar inmediatamente en tu trabajo?
- ¿Cuál proporciona verificación de fuentes?
- ¿Cuál se adapta a tu contexto específico?

### Conclusión Práctica

El prompt engineering con documentos transforma la sobrecarga de información en ventaja competitiva. Al dominar esta técnica, puedes:
- Reducir horas de lectura a minutos de análisis
- Obtener perspectivas personalizadas para tu rol
- Tomar decisiones basadas en datos verificables
- Crear un sistema reutilizable para cualquier documento

---

## Embedding

**Descifrando el Lenguaje de los LLMs**

Hasta ahora hemos dominado la estructuración de prompts y el análisis de documentos. Pero para convertirnos en verdaderos expertos en prompt engineering, necesitamos entender **cómo** los modelos de lenguaje procesan y comprenden nuestras palabras. Aquí es donde entran en juego los embeddings, el corazón semántico de los LLMs.

### El Mundo Vectorial: Donde las Palabras Viven como Números

Imagina que cada palabra tiene un "ADN matemático" único. Eso es exactamente un embedding:

**¿Qué son los Embeddings?**
- Representación vectorial de palabras en espacios multidimensionales
- Secuencias numéricas que capturan el significado semántico
- Sistema que permite medir similitudes y diferencias contextuales

**Ejemplo Práctico:**
```
"perro" → [0.2, -0.5, 0.8, 0.3, ...]
"gato" → [0.25, -0.45, 0.78, 0.28, ...]
```
La cercanía entre estos vectores explica por qué los LLMs entienden que perros y gatos comparten características (animales, domésticos, mamíferos).

### Operaciones Semánticas: La Magia Matemática del Lenguaje

Lo más fascinante es que podemos realizar operaciones con estos vectores como si fueran números:

**Ejemplo Clásico:**
```
rey − hombre + mujer = reina
```

Esta operación vectorial demuestra cómo los LLMs capturan relaciones semánticas complejas. No es magia, es matemática pura.

### Visualizando el Espacio Semántico

Para entender mejor este concepto, explora esta herramienta interactiva:

🔗 **[Embedding Projector - TensorFlow](https://projector.tensorflow.org/)**

Al usar esta visualización, ten en cuenta:
- Solo muestra 3 dimensiones (los LLMs usan cientos o miles)
- Las distancias visuales pueden cambiar al rotar la vista
- Las palabras cercanas comparten contexto semántico

**Prueba esto en el Embedding Projector:**
1. Busca "queen" (reina)
2. Observa palabras cercanas: "king", "princess", "Elizabeth"
3. Compara con búsquedas de "technology", "education", "programming"

### Por Qué los Embeddings Superan al Teclado Predictivo

- **Teclado predictivo**: Sugiere palabras basadas en frecuencia, sin comprensión
- **LLM con embeddings**: Dirige la atención a zonas semánticas relevantes

**Ejemplo:**
```
"El cielo es..." 
```
Un LLM enfoca su atención en la región semántica del clima y completa coherentemente, mientras un teclado predictivo solo sugiere palabras comunes.

### Aplicación Práctica en Prompt Engineering

**Estrategias Basadas en Embeddings:**

1. **Selección Intencional de Palabras**
   ```
   ❌ "Habla de aprendizaje"
   ✅ "Explica machine learning para principiantes"
   ```

2. **Uso de Lenguaje Nativo**
   - Español nativo capta mejor matices culturales
   - Traducciones automáticas pierden embedding richness

3. **Contextualización Explícita**
   ```
   [Contexto] En educación tecnológica en Latinoamérica...
   ```

4. **Analogías Semánticas**
   ```
   "Explícalo como si fuera [concepto familiar]"
   ```

### Práctica: Experimentando con el Espacio Vectorial

**Ejercicio de Embeddings:**

1. **Explora el Embedding Projector**
   - Ingresa al [enlace proporcionado](https://projector.tensorflow.org/)
   - Busca palabras clave de tu industria
   - Observa patrones y relaciones

2. **Crea Analogías Vectoriales**
   Intenta estas operaciones semánticas:
   ```
   México - América Latina + Europa = ?
   Programación - código + diseño = ?
   ```

3. **Compara Resultados con Diferentes Términos**
   - Prompt A: "Explica inteligencia artificial"
   - Prompt B: "Explica machine learning y deep learning"
   - ¿Notas diferencias en profundidad y enfoque?

### Conclusión: Dominando el Lenguaje de los LLMs

Los embeddings no son solo un concepto técnico, son la clave para comunicarnos efectivamente con los modelos de lenguaje. Al entender que cada palabra activa regiones específicas en el espacio vectorial, podemos:

- Diseñar prompts más precisos y efectivos
- Anticipar cómo el modelo interpretará nuestras instrucciones
- Crear analogías y relaciones que el modelo entenderá naturalmente

**Reflexión Final:**
¿Has notado cómo cambiar una sola palabra en tu prompt puede transformar completamente la respuesta? Ahora sabes por qué: estás navegando por diferentes regiones del espacio vectorial de embeddings.

¿Qué analogías semánticas has descubierto en tu uso de LLMs? Comparte tus hallazgos y juntos exploremos las fascinantes dimensiones del lenguaje artificial.


---

# Roles 
**El Poder Transformador de los Roles en tus Prompts**

Llegamos a uno de los conceptos más poderosos en prompt engineering: la asignación estratégica de roles. Como descubrimos con los embeddings, cada palabra dirige la atención del modelo hacia regiones específicas del espacio vectorial. Al definir un rol, estamos realizando la navegación más efectiva posible hacia el conocimiento especializado que necesitamos.

### Tu Brújula en el Espacio Vectorial

**¿Por qué un rol cambia todo?**
Cuando asignas un rol al LLM, estás esencialmente dándole una "descripción de puesto" que:
- Orienta el tono y vocabulario
- Activa patrones de lenguaje especializado
- Enfoca la respuesta en el área de conocimiento relevante
- Reduce la ambigüedad desde el primer momento

### Demostración Práctica: El Ejemplo del Clima

**Prompt Genérico:**
```
¿qué es el clima?
```
*Respuesta típica:* Definición técnica estándar - "condiciones atmosféricas como temperatura, precipitación, humedad..."

**Prompt con Rol Estratégico:**
```
Actúa como climatólogo experto y explícame qué es el clima. Yo soy un niño de primaria.
```
*Respuesta transformada:* 
"¡Hola amiguito! 🌞 El clima es como la 'personalidad' de un lugar cada día. ¿Ves cuando a veces hace sol ☀️, otras llueve 🌧️, o hace viento 💨? ¡Eso es el clima! Es como si la Tierra tuviera diferentes estados de ánimo..."

### La Anatomía de un Prompt con Rol Efectivo

**Estructura Comprobada:**
```
[Rol] Actúa como [especialista específico]
[Enfoque] [Tarea concreta con verbo de acción]
[Contexto] [Información relevante + audiencia]
[Límites] [Formato, extensión, tono]
```

**Ejemplo Desglosado:**
```
[Rol] Actúa como ingeniero de software senior especializado en Python
[Enfoque] Explica el concepto de decoradores
[Contexto] Soy un desarrollador junior con 6 meses de experiencia
[Límites] Máximo 300 palabras, usa analogías prácticas, evita tecnicismos innecesarios
```

### Validación de Roles: Antes de Disparar

Una práctica subestimada pero crucial es validar cómo el modelo interpreta un rol:

**Prompt de Validación:**
```
Para ti, ¿qué es un community manager? Describe sus responsabilidades clave.
```

Esto te permite:
- Verificar la comprensión del modelo sobre ese rol
- Ajustar o cambiar el rol antes de la tarea principal
- Evitar malentendidos costosos

### Práctica: Transformando Prompts con Roles

**Ejercicio de Transformación:**

1. **Prompt Débil Original:**
   ```
   Necesito ideas para redes sociales
   ```

2. **Prompt con Rol Estratégico:**
   ```
   [Rol] Actúa como director creativo de una agencia de marketing viral
   [Enfoque] Genera 5 ideas para posts de Instagram
   [Contexto] Tengo una startup de educación en tecnología para jóvenes
   [Límites] Ideas específicas para Gen Z, tono casual pero profesional, incluye hooks atractivos
   ```

**Compara los resultados:**
- ¿Cuál produce ideas más innovadoras y específicas?
- ¿Cuál entiende mejor el contexto del negocio?
- ¿Cuál requiere menos iteraciones?

### Casos de Uso por Industria

**Para Educadores:**
```
[Rol] Eres un pedagogo especializado en aprendizaje acelerado
[Enfoque] Diseña un plan de 30 minutos para enseñar [concepto]
[Contexto] Estudiantes universitarios con atención limitada
```

**Para Emprendedores:**
```
[Rol] Actúa como consultor de startups en etapa temprana
[Enfoque] Analiza este modelo de negocio y señala 3 riesgos principales
[Contexto] Producto SaaS con 100 usuarios mensuales
```

**Para Desarrolladores:**
```
[Rol] Eres arquitecto de software con 15 años de experiencia
[Enfoque] Revisa esta estructura de base de datos
[Contexto] Aplicación de e-commerce escalando a 10,000 usuarios
```

### Conclusión: Dominio a Través de Roles

El uso estratégico de roles no es un truco más; es la evolución natural de entender cómo funcionan los LLMs. Al asignar roles específicos:

- **Triplicas** la relevancia de las respuestas
- **Reduces** las iteraciones necesarias
- **Aumentas** la calidad del output
- **Personalizas** la experiencia para tu contexto único

**Tu Desafío Práctico:**
Toma una tarea que hayas solicitado recientemente a un LLM y reescríbela usando la estructura de roles. Compara los resultados.

¿Qué rol descubriste que transformó completamente tus resultados? ¿Cómo aplicaste este concepto en tu industria?

---

**Curso de Prompt Engineering: Comparando Modelos de IA para Resultados Óptimos**

Hemos dominado la estructura de prompts, el análisis de documentos, los embeddings y el uso estratégico de roles. Ahora llega el momento crucial: **¿qué modelo elegir para cada tarea?** La respuesta no es única, y aprender a comparar sistemáticamente te dará una ventaja competitiva significativa.

### El Arte de la Comparación Justa: Método Científico para IA

**Por qué comparar correctamente importa:**
- Los modelos evolucionan semanalmente
- Cada uno tiene fortalezas específicas
- El "mejor" depende completamente de tu caso de uso

**Metodología de comparación confiable:**
1. **Prepara el entorno:** Abre ChatGPT, Claude, Gemini y Copilot en pestañas paralelas
2. **Mismo prompt, mismo momento:** Ejecuta pruebas el mismo día para evitar variaciones por actualizaciones
3. **Criterios predefinidos:** Define qué buscarás antes de ver los resultados
4. **Prompt unificado:** Usa exactamente la misma instrucción en todos

### Ejemplo Práctico: Mejorando la Productividad del Equipo

**Prompt Genérico (para comparación base):**


>¿cómo mejorar la productividad del equipo?


**Prompt Estructurado (para comparación avanzada):**

>Eres consultor especializado en eficiencia organizacional
>
>Propon 5 estrategias para mejorar productividad
>
>Equipo de 15 personas en startup tecnológica, trabajo híbrido
>
>Estrategias accionables, máximo 300 palabras, formato bullet points

- [Rol] Eres consultor especializado en eficiencia organizacional

- [Enfoque] Propon 5 estrategias para mejorar productividad

- [Contexto] Equipo de 15 personas en startup tecnológica, trabajo híbrido

- [Límites] Estrategias accionables, máximo 300 palabras, formato bullet points

### Análisis de Resultados por Criterios

**Criterios de Evaluación Esenciales:**

1. **Claridad:** ¿Las ideas son concretas y entendibles?
2. **Accionabilidad:** ¿Ofrece pasos aplicables inmediatamente?
3. **Contextualización:** ¿Se adapta al escenario específico?
4. **Profundidad vs Brevedad:** ¿Logra el equilibrio adecuado?
5. **Formato:** ¿Presentación limpia y fácil de digerir?

**Ejemplo de Hallazgos Típicos:**
- **ChatGPT:** 6 ítems detallados, tono conversacional
- **Claude:** Estructura jerárquica clara, enfoque en procesos
- **Gemini:** 4 puntos concisos, integración con herramientas Google
- **Copilot:** Enfoque Microsoft-centric, referencia a Teams/Office

### Entendiendo el Ecosistema de Modelos

**No es lo mismo la herramienta que el modelo:**

- **ChatGPT (OpenAI):** Modelos GPT-4, GPT-5
  - *Modos:* Bajo pensamiento → Pensamiento → Pro
  - *Ideal para:* Creatividad, redacción, análisis general

- **Claude (Anthropic):** Opus vs Sonnet
  - *Opus:* Máximo razonamiento para problemas complejos
  - *Sonnet:* Eficiente para tareas diarias
  - *Ideal para:* Análisis ético, documentos largos

- **Gemini (Google):** 2.5 Pro vs 2.5 Flash
  - *Pro:* Razonamiento avanzado, matemáticas, código
  - *Flash:* Velocidad para consultas directas
  - *Ideal para:* Integración Google Workspace, búsqueda

- **Microsoft Copilot:** GPT-4/GPT-5 + Prometheus
  - *Prometheus:* Orquesta LLM con datos Microsoft
  - *Ideal para:* Entornos empresariales Microsoft

### Modelos Rápidos vs. Modelos de Razonamiento

**Cuándo usar cada tipo:**

**Modelos Rápidos (Gemini Flash, ChatGPT rápido):**

>"Resume este documento en 3 puntos clave"
>"Traduce este párrafo al inglés"

- Respuesta inmediata
- Consultas directas
- Procesamiento por lotes

**Modelos de Razonamiento (Claude Opus, GPT-5 Pro):**

>"Analiza estas 3 estrategias de marketing y recomienda la óptima con justificación"
>
>"Diseña un plan de transformación digital en 5 fases"

- Pensamiento paso a paso
- Problemas complejos
- Toma de decisiones

### Práctica: Tu Propia Comparación Sistemática

**Ejercicio Guiado:**

1. **Identifica tu tarea real:**
   
   >"Crear un plan de contenido para redes sociales del próximo trimestre"
  

2. **Diseña tu prompt estructurado:**
   
   >Eres director de marketing digital
   >Crea un plan de contenido para 3 meses
   >Empresa B2B SaaS, audiencia: directores técnicos
   >4 publicaciones por mes, incluir temas y formatos
   


   - [Rol] Eres director de marketing digital
   - [Enfoque] Crea un plan de contenido para 3 meses
   - [Contexto] Empresa B2B SaaS, audiencia: directores técnicos
   - [Límites] 4 publicaciones por mes, incluir temas y formatos

3. **Ejecuta en las 4 plataformas** el mismo día

4. **Evalúa con esta matriz:**
   
   | Criterio        | ChatGPT | Claude | Gemini | Copilot |
   |-----------------|---------|--------|--------|---------|
   | Claridad        |    ⭐⭐⭐   |   ⭐⭐⭐⭐  |   ⭐⭐⭐   |   ⭐⭐    |
   | Accionabilidad  |    ⭐⭐⭐⭐  |   ⭐⭐⭐⭐  |   ⭐⭐⭐   |   ⭐⭐⭐   |
   | Originalidad    |    ⭐⭐⭐   |   ⭐⭐⭐⭐  |   ⭐⭐    |   ⭐⭐⭐   |
   | Integración     |    ⭐⭐    |   ⭐⭐    |   ⭐⭐⭐⭐  |   ⭐⭐⭐⭐  |
   

3. **Conclusión accionable:**
   "Para planificación de contenido, Claude ofrece mayor profundidad estratégica, mientras Gemini integra mejor con mi stack de Google"

### Integración en Tu Flujo de Trabajo

**Consideraciones prácticas:**
- **Si usas Google Workspace:** Gemini ofrece integración nativa
- **Entorno Microsoft:** Copilot accede a tus emails y documentos
- **Proyectos creativos:** ChatGPT suele liderar en originalidad
- **Análisis ético/complejo:** Claude Opus destaca

### Conclusión: Tu Kit de Herramientas Inteligente

Dominar la comparación de modelos te convierte en un usuario estratégico de IA. En lugar de tener un favorito, desarrollas un criterio para:

- **Seleccionar** el modelo óptimo para cada tipo de tarea
- **Ahorrar** tiempo y obtener mejores resultados
- **Adaptarte** rápidamente a nuevas versiones y herramientas

**Tu Desafío Final:**
Esta semana, realiza una comparación formal con una tarea real de tu trabajo.
- ¿Qué tarea elegiste?
- ¿Qué modelo ganó y por qué?
- ¿Qué sorpresa descubriste en el proceso?

La verdadera maestría en prompt engineering no está en conocer un solo modelo, sino en saber orquestar todo el ecosistema para tu beneficio.

