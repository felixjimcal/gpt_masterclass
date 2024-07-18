# gpt_masterclass
Notes from the course: https://www.udemy.com/course/chatgpt-complete-masterclass

Interesting links:
- https://flowgpt.com/
- https://github.com/f/awesome-chatgpt-prompts
- https://www.kaggle.com/datasets/aungpyaeap/supermarket-sales
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
---------------------------------------------------------------------------------------------------
**Bulking Generations**
- Check folder with same name
---------------------------------------------------------------------------------------------------
**GPT-4/GPT-3.5**: Modelos de lenguaje grandes detrás de ChatGPT, capaces de generar texto humano.

**Modelo de lenguaje grande**: Inteligencia artificial entrenada con vastos datos para reconocer patrones y generar texto.

**Red neuronal**: Sistema de capas interconectadas de nodos (neuronas) que procesan y transmiten información.

**Modelo transformador**: Tipo avanzado de red neuronal que procesa secuencias de texto simultáneamente.

**Atención**: Mecanismo que permite al modelo enfocarse en partes relevantes del texto al generar respuestas.

**Encoder-Decoder**: Arquitectura donde el encoder convierte el input en vectores y el decoder genera la salida a partir de esos vectores.

---------------------------------------------------------------------------------------------------
**Estructura multi-capa**: Composición del modelo de lenguaje grande con múltiples capas en el encoder y decoder para procesar y generar texto.

**Transformers**: Modelos neuronales avanzados que han revolucionado el procesamiento del lenguaje natural.

**Mecanismo de atención**: Permite al modelo enfocarse en partes relevantes del texto para generar respuestas contextualmente adecuadas.

**Pesos**: Valores asignados a cada palabra del input que representan su importancia en el contexto, determinados por consultas, claves y valores.

**Capa de atención multi-cabezal**: Asigna pesos a las palabras y combina múltiples cabezas para producir el output final.

**Encoder**: Procesa el input en el modelo transformador.

**Decoder**: Genera el output, utilizando una capa de atención extra que toma el output del encoder como input.

**Tokenización**: Proceso crucial para dividir el texto en unidades manejables para su procesamiento y comprensión.

---------------------------------------------------------------------------------------------------
**Tokenización**: Proceso de dividir texto en unidades más pequeñas, llamadas tokens, que el modelo puede procesar.

**Codificación Byte-Pair**: Técnica utilizada para dividir el texto en partes más frecuentes, incluso caracteres individuales.

**Token**: Unidad de texto procesada por el modelo, promedio de cuatro caracteres en inglés.

**Probabilidades**: ChatGPT predice el siguiente token basado en probabilidades derivadas del contexto previo.

**Playground**: Herramienta de OpenAI para experimentar con la generación de texto y ver probabilidades de tokens.

**Granularidad de tokens**: Equilibrio delicado para decidir el tamaño de los tokens durante el entrenamiento del modelo.

---------------------------------------------------------------------------------------------------
**Pre-entrenamiento**: Exposición del modelo a vastos datos textuales para aprender a predecir la siguiente palabra en una oración.

**Fine tuning**: Entrenamiento adicional con un conjunto de datos más específico, guiado por revisores humanos para ajustar las respuestas del modelo.

**Datos de entrenamiento**: Incluyen artículos, libros, sitios web, papers científicos y código, usados para enseñar patrones al modelo.

**Sesgos**: El modelo puede aprender sesgos presentes en los datos de entrenamiento.

**Comprensión de patrones**: El modelo genera respuestas basadas en patrones aprendidos, no en una comprensión humana del texto.

**Feedback humano**: Retroalimentación de revisores humanos que ayuda a ajustar y mejorar el comportamiento del modelo.

---------------------------------------------------------------------------------------------------
**Signal Prompting**: Técnica para influir en las respuestas del modelo usando palabras o frases asociativas.

**Ejemplo histórico**: "Lista de 10 figuras históricas" con la palabra "Europa" añadida para limitar a figuras europeas.

**Asociaciones abstractas**: Palabras como "caer" o "rojo" pueden generar respuestas inesperadas o novedosas basadas en asociaciones del modelo.

**Fechas**: Añadir "1900" para obtener figuras históricas relacionadas con ese año.

**Listas señaladas**: Usar indicaciones como "A" o formatos de numeración específicos para guiar la estructura de la respuesta.

---------------------------------------------------------------------------------------------------
**Signal Prompting**: Técnica para influir respuestas de ChatGPT añadiendo palabras específicas.

**Lista de figuras históricas**: Solicitar una lista y agregar palabras para enfocar la respuesta.
Ejemplo: "Europa" para obtener solo figuras europeas.

**Asociaciones**: Añadir palabras abstractas para generar asociaciones inesperadas.
Ejemplo: "Caída" para obtener respuestas relacionadas con ese concepto.

**Palabras específicas**: Usar palabras como "rojo" para obtener conexiones específicas.
Ejemplo: Mao Zedong, asociado al comunismo chino.

**Fechas**: Añadir años para obtener figuras relacionadas con esa época.
Ejemplo: "1900" para obtener figuras nacidas, premiadas o vividas en esa época.

**Numeración**: Usar formatos de numeración específicos para estructurar respuestas.
Ejemplo: Iniciar lista con "A" para comenzar directamente con la letra especificada.

---------------------------------------------------------------------------------------------------
**Reverse-engineering prompt**: Técnica para generar un prompt que produzca un output similar a uno que nos gusta.

**Act as reverse prompt engineer**: Prompt usado para analizar y generar instrucciones para obtener un output similar.

**Ejemplo divertido**: "I will give you answers and you will generate the questions about these answers."

**Proceso**: Proveer respuestas (como "carbon dioxide" y "cats"), obtener preguntas relacionadas.

**Uso práctico**: Analizar un output deseado, generar un prompt específico para replicar el estilo.

**Probabilidad**: Resultados varían, se pueden ajustar y regenerar prompts para mejorar precisión.

**Prompt**: "Act as reverse prompt engineer. I will give you an example output. You will analyze this output and give me instructions that I can give someone to write a very similar style output."

---------------------------------------------------------------------------------------------------
**GPT-3.5**: Modelo con dificultades en problemas lógicos complejos.

**Chain of thought prompt**: Técnica para mejorar la precisión añadiendo razonamiento paso a paso.

**Ejemplo**: Contar palabras en un texto, añadir "provide step-by-step reasoning" para obtener la respuesta correcta.

**Precisión**: Aumenta al seguir el proceso de pensamiento del modelo.

**Aplicación**: Útil para problemas lógicos y preparación para entrevistas.

---------------------------------------------------------------------------------------------------
**Open AI Playground**: Alternativa a la interfaz de ChatGPT con más capacidades.

**Parámetros específicos**: Permite ajustar parámetros del modelo.

**Acceso**: Desde openai.com, bajo la sección de desarrolladores.

**Precios**: Pago por input y output, sin suscripción. GPT-3.5 Turbo: 0.15 centavos por 1000 tokens.

**Tokens**: Bloques básicos de texto, aproximadamente 3/4 de una palabra.

**Funcionalidades**: Cambiar modos, usar diferentes modelos, y modificar parámetros.

**Ejemplo**: Asignar roles, como "profesor de primaria", para ajustar respuestas.

**Prompt**: "You are an elementary school teacher."

---------------------------------------------------------------------------------------------------
**Open AI Playground**: Alternativa con más capacidades y parámetros ajustables para ChatGPT.

**Parámetros**: Permiten ajustar el modelo para aplicaciones específicas.

**Modelos**: GPT-3.5 Turbo, estándar y eficiente en costos.

**Precio**: Por input y output, basado en tokens.

**Tokens**: Bloques de texto, aproximadamente 3/4 de una palabra.

**Temperature**: Controla la aleatoriedad, valores bajos dan respuestas más genéricas y determinísticas; valores altos dan respuestas más creativas y aleatorias.

**Contexto**: Modelos avanzados permiten mayor límite de tokens para contexto más amplio.

**Prompt**: "You are a teacher."

**Ejemplo**: "Tell me something about cats" con alta temperatura muestra respuestas más creativas pero potencialmente sin sentido.

En la próxima lección, se discutirán parámetros como longitud máxima y secuencias de parada.

---------------------------------------------------------------------------------------------------
**Top P**: Controla la diversidad mediante muestreo nuclear; valores bajos reducen el número de palabras consideradas.

**Muestreo nuclear**: Método matemático que considera opciones basadas en su probabilidad.

**Efecto**: Valores bajos enfocan las respuestas al considerar solo las palabras más probables; valores altos permiten más creatividad y aleatoriedad.

**Temperature**: Ajusta la probabilidad de elección de palabras menos probables; valores altos aumentan la aleatoriedad y creatividad.

**Frecuencia y presencia**: Parámetros adicionales que se discutirán en la próxima lección para ajustar la generación de respuestas.

---------------------------------------------------------------------------------------------------
**Frequency penalty**: Penaliza nuevos tokens según su frecuencia existente en el texto, reduciendo repeticiones.

**Presence penalty**: Penaliza tokens si ya han aparecido, disminuyendo la probabilidad de repetir temas.

**Uso**: Importante para ajustar parámetros en aplicaciones, mejorando la originalidad y diversidad del texto generado.

**Guardar presets**: Permite guardar configuraciones de parámetros para uso futuro.

En la próxima lección, se explorarán los presets y ejemplos disponibles.

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------

---------------------------------------------------------------------------------------------------





