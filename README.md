# PFC-2
# LangChain: Usando Modelos de Lenguaje con Hugging Face y OpenAI

## Descripción

 **LangChain**, una poderosa biblioteca para trabajar con **Modelos de Lenguaje Grandes (LLMs)** como **Hugging Face** y **OpenAI**. LangChain permite crear aplicaciones e integrar flujos de trabajo complejos, tales como chatbots, generación de preguntas y respuestas, resúmenes automáticos y mucho más.

En este ejemplo, mostramos cómo conectar **LangChain** con **Hugging Face** y **OpenAI** para hacer tareas de procesamiento de lenguaje natural.

## Requisitos

Para empezar, necesitas instalar los siguientes paquetes:

```bash
pip install -qU langchain
pip install -qU huggingface_hub
pip install -qU openai



## Configuración

### **Hugging Face**

Para utilizar los modelos de Hugging Face, necesitarás configurar tu token de API.

1. Crea una cuenta en [Hugging Face](https://huggingface.co/).
2. Entra en tu perfil, selecciona **Settings** > **Access Tokens** > **New Token**.
3. Copia el token generado y pégalo en tu código como se muestra a continuación:

```python
import os
os.environ['HUGGINGFACEHUB_API_TOKEN'] = 'HF_API_KEY'  # Reemplaza con tu token
