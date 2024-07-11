# Victor AI Assistant

Victor es un chatbot  diseñado para proporcionar asistencia basada en los datos recolectados por los relojes 
inteligentes de Samsung. Este proyecto utiliza inteligencia artificial y aprendizaje automático para interpretar 
y responder a consultas relacionadas con la salud y el bienestar, basándose en la información recolectada por 
los dispositivos.


![image](https://github.com/repositoriosHackaton/Turing/assets/76980571/6c33f5ed-295a-4c51-961c-83af38780c22)

## Tabla de contenidos

1. Estructura de las carpetas.
2. Fases del desarrollo.
3. Arquitecturas utilizadas
4. [Proceso](#Proceso)
7. [Agradecimientos](#Agradecimientos)



# Estructura de las carpetas

  ### **venv/:** 
  Este directorio contiene el entorno virtual de Python. Es utilizado para aislar las dependencias del
  proyecto y asegurarse de que no haya conflictos con otras versiones de paquetes instalados globalmente en el sistema.

  ### **Data/:** 
  En este directorio se almacenan los datos necesarios para el funcionamiento del chatbot.

  ### **Icons/:** 
  Este directorio contiene los iconos utilizados en la interfaz gráfica de usuario (GUI) del chatbot.

  ### **API_key.env:** 
  Este archivo de entorno contiene la clave API de OPEN AI. Este archivo debe ser configurado correctamente
  antes de ejecutar el chatbot.

  ### **GUI.py:** 
  Este archivo fuente de Python contiene el código para la interfaz gráfica de usuario del chatbot. Maneja las
  interacciones del usuario y presenta la información de manera visualmente accesible.

  ### **victorAI.py:** 
  Este archivo fuente de Python contiene la lógica principal del chatbot, incluyendo la integración con la API
  de OPEN AI, el procesamiento de datos y las respuestas del asistente virtual basado en inteligencia artificial.

# Fases del desarrollo.
  1. Se busco [data](https://www.kaggle.com/datasets/djamchid92/samsung-health) real de un samsung watch para poder usarla en el modelo.
  2. Se limpiaron los dataset para crear la base de conocimiento.
  3. Se dividio la data en dos parates. Entrenamiento (Fine tunning) y prueba (RAG).
  4. Se realizo el fine tunning del modelo.
  5. Se implemento RAG en el modelo

# Arquitecturas utilizadas
## Rag
El proyecto utiliza una arquitectura llamada **RAG** (Retrieval Augmented Generation). Rag es un enfoque en inteligencia artificial que 
combina la recuperación de información y la generación de texto. Utiliza un modelo de recuperación para buscar documentos relevantes de 
una base de datos en respuesta a una consulta, y luego un modelo generativo para crear una respuesta coherente basada en esos documentos 
recuperados. Esto permite proporcionar respuestas más precisas y contextualmente apropiadas en aplicaciones como chatbots y asistentes 
virtuales.


![image](https://github.com/HarolReyes0/Turing/assets/76980571/9c468ac2-9fa0-49db-aa01-3848974ceea6)

## Fine Tunning
Fine-tuning es el proceso de ajustar un modelo de inteligencia artificial preentrenado en un conjunto de datos específico para una tarea 
particular. Consiste en tomar un modelo que ya ha sido entrenado en una gran cantidad de datos genéricos y entrenarlo adicionalmente con 
un conjunto de datos más pequeño y específico para adaptar el modelo a una tarea específica, mejorando su rendimiento en esa tarea particular.

![image](https://github.com/HarolReyes0/Turing/assets/76980571/21125987-b793-4444-b235-af2297d35c1f)
