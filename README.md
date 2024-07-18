# gpt_masterclass
Notes from the course: https://www.udemy.com/course/chatgpt-complete-masterclass

Interesting links:
- https://flowgpt.com/
- https://github.com/f/awesome-chatgpt-prompts
---------------------------------------------------------------------------------------------------
El CETO (Contexto, Especificidad, Tono y Objetivo) en ingeniería de prompts es una guía para crear instrucciones efectivas y claras para modelos de lenguaje como ChatGPT. 

1. **Contexto**: Proporciona información relevante para situar al modelo.
2. **Especificidad**: Detalla claramente lo que se espera del modelo.
3. **Tono**: Define el estilo o el enfoque deseado en la respuesta.
4. **Objetivo**: Establece el propósito final del prompt o la tarea específica que se desea lograr.

Estos elementos ayudan a obtener respuestas más precisas y útiles del modelo.
---------------------------------------------------------------------------------------------------
Claro, aquí tienes un ejemplo utilizando el método CETO para un prompt:

**Contexto**: Eres un asistente de inteligencia artificial especializado en historia del arte.
**Especificidad**: Quiero un resumen sobre el estilo y las obras más importantes de Vincent van Gogh.
**Tono**: Utiliza un lenguaje sencillo y accesible.
**Objetivo**: Proveer información clara y concisa para un estudiante de secundaria.

**Prompt resultante**:
```
Eres un asistente de inteligencia artificial especializado en historia del arte. Quiero un resumen sobre el estilo y las obras más importantes de Vincent van Gogh. Utiliza un lenguaje sencillo y accesible. Provee información clara y concisa para un estudiante de secundaria.
```

**Respuesta esperada**:
Vincent van Gogh fue un pintor postimpresionista conocido por su uso audaz del color y su estilo emotivo. Algunas de sus obras más importantes incluyen "La noche estrellada", "Los girasoles" y "El dormitorio en Arlés". Su técnica se caracteriza por pinceladas gruesas y texturizadas, y a menudo pintaba escenas de la vida cotidiana y paisajes.
---------------------------------------------------------------------------------------------------
En el contexto de la ingeniería de prompts y el aprendizaje automático, los términos Zero-Shot, One-Shot y Few-Shot se refieren a diferentes enfoques para hacer que un modelo realice tareas basadas en la cantidad de ejemplos proporcionados durante el entrenamiento o el uso.

1. **Zero-Shot**:
   - **Definición**: El modelo realiza una tarea sin haber visto ningún ejemplo específico de esa tarea durante el entrenamiento.
   - **Ejemplo**:
     **Prompt**: "Traducir la siguiente frase al francés: 'Good morning'."
     **Respuesta esperada**: "Bonjour."

2. **One-Shot**:
   - **Definición**: El modelo recibe un solo ejemplo antes de realizar la tarea.
   - **Ejemplo**:
     **Prompt**: "Ejemplo: 'Hello' se traduce al francés como 'Bonjour'. Ahora traduce la siguiente frase: 'Good night'."
     **Respuesta esperada**: "Bonne nuit."

3. **Few-Shot**:
   - **Definición**: El modelo recibe unos pocos ejemplos antes de realizar la tarea.
   - **Ejemplo**:
     **Prompt**: "Ejemplos: 'Hello' se traduce al francés como 'Bonjour'. 'Goodbye' se traduce al francés como 'Au revoir'. Ahora traduce la siguiente frase: 'Good night'."
     **Respuesta esperada**: "Bonne nuit."

Estos enfoques permiten evaluar y utilizar la capacidad del modelo para generalizar y aplicar conocimientos previos a nuevas tareas con diferentes niveles de guía y ejemplos.
---------------------------------------------------------------------------------------------------
Sequential Prompting = Steps by steps
---------------------------------------------------------------------------------------------------
**Ask-to-Respond Prompting** es una técnica en la ingeniería de prompts donde el modelo formula preguntas relevantes sobre el tema antes de proporcionar una respuesta completa. Esto ayuda a clarificar el contexto y asegurar que la respuesta sea más precisa y relevante.

**Ejemplo de Ask-to-Respond Prompting**:

**Tarea**: Escribir una breve biografía de Leonardo da Vinci.

**Paso 1**: Solicitar preguntas al modelo.
**Prompt**: "Voy a escribir una breve biografía de Leonardo da Vinci. ¿Qué preguntas debo responder para cubrir los aspectos más importantes de su vida y obra?"

**Respuesta esperada**:
1. "¿Cuándo y dónde nació Leonardo da Vinci?"
2. "¿Cuáles fueron sus principales áreas de interés y contribuciones?"
3. "¿Cuáles son algunas de sus obras más famosas?"
4. "¿Cómo influyó en el Renacimiento?"
5. "¿Cuándo y dónde murió?"

**Paso 2**: Responder a las preguntas generadas.
**Pregunta 1**: "¿Cuándo y dónde nació Leonardo da Vinci?"
**Respuesta esperada**: "Leonardo da Vinci nació el 15 de abril de 1452 en Vinci, Italia."

**Pregunta 2**: "¿Cuáles fueron sus principales áreas de interés y contribuciones?"
**Respuesta esperada**: "Leonardo da Vinci fue un pintor, científico, ingeniero, anatomista, escultor y arquitecto. Contribuyó significativamente a diversas áreas del conocimiento."

**Pregunta 3**: "¿Cuáles son algunas de sus obras más famosas?"
**Respuesta esperada**: "Algunas de sus obras más famosas incluyen 'La Mona Lisa', 'La Última Cena' y 'El Hombre de Vitruvio'."

**Pregunta 4**: "¿Cómo influyó en el Renacimiento?"
**Respuesta esperada**: "Leonardo da Vinci fue una figura clave del Renacimiento, conocido por su enfoque multidisciplinario que combinaba arte y ciencia, lo cual inspiró a generaciones posteriores."

**Pregunta 5**: "¿Cuándo y dónde murió?"
**Respuesta esperada**: "Leonardo da Vinci murió el 2 de mayo de 1519 en Amboise, Francia."

**Paso 3**: Redactar la biografía utilizando las respuestas.
**Prompt**: "Usando las respuestas anteriores, escribe una breve biografía de Leonardo da Vinci."
**Respuesta esperada**: "Leonardo da Vinci nació el 15 de abril de 1452 en Vinci, Italia. Fue un pintor, científico, ingeniero, anatomista, escultor y arquitecto, conocido por sus contribuciones significativas a diversas áreas del conocimiento. Algunas de sus obras más famosas incluyen 'La Mona Lisa', 'La Última Cena' y 'El Hombre de Vitruvio'. Fue una figura clave del Renacimiento, conocido por su enfoque multidisciplinario que combinaba arte y ciencia, inspirando a generaciones posteriores. Leonardo da Vinci murió el 2 de mayo de 1519 en Amboise, Francia."

Este método permite al modelo ayudar a estructurar la información relevante antes de componer la respuesta final.
---------------------------------------------------------------------------------------------------
**ASk for images**
- Como representarías la tenacidad?
![image](https://github.com/user-attachments/assets/da39c12e-d9f4-49fe-befa-d4d4f6bfc902)
- ¿Y la lectura? no libros, sinó el poder de adquirir conocimiento y felicidad con la lectura
![image](https://github.com/user-attachments/assets/14112a3a-6ca1-4b09-898d-3532431101a9)
- Ahora juntalos, tenacidad y lectura
![image](https://github.com/user-attachments/assets/09261493-7436-47c8-bf1e-3edb1e7edf44)
- ¿Conoces la teoría de Carl Jung de los símbolos?
- Sí, Carl Jung desarrolló la teoría de los símbolos como parte de su psicología analítica. Según Jung, los símbolos son representaciones inconscientes de arquetipos, que son patrones universales y recurrentes que surgen en el inconsciente colectivo. Los símbolos ayudan a expresar contenidos psíquicos profundos y a conectar la mente consciente con el inconsciente.
- ¿Qué símbolo representaría la lectura y cuál la tenacidad y cual podría represaentar a ambos ?

**Símbolos según Carl Jung:**

- **Lectura:** El "libro abierto" es un símbolo común de la lectura, representando conocimiento, aprendizaje y sabiduría.

- **Tenacidad:** El "roble" simboliza fuerza y perseverancia debido a su robustez y capacidad para soportar adversidades.

- **Ambos (lectura y tenacidad):** La "antorcha" podría representar ambos, simbolizando la luz del conocimiento y la perseverancia en la búsqueda de la verdad, ya que ilumina el camino en la oscuridad.
- representa la antorcha, en un tatuaje en blanco y negro
- ![image](https://github.com/user-attachments/assets/64b286f7-6c41-41a1-a502-f755ce6ff782)
- Hazla más terrorifica
- ![image](https://github.com/user-attachments/assets/2940ce84-ad28-48fc-a2d9-b26955ea0332)
- DALL·E 2024-07-18 11.26.42 - Tattoo design in black and white of a torch with a more terrifying appearance. The flame is dark and jagged, with ghostly faces and twisted shapes eme.webp
- 
---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------
