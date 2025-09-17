# 🎓 Adopta_un_Junior_IA

📌 [Notebook en Google Colab](https://colab.research.google.com/drive/1W4I4se4GHpiCEmHsw7nafFAY4OI7gB_u?usp=sharing)

---

## ❓ ¿Por qué funcionan mis prompts?

Mis prompts funcionan porque:  
- 📐 Dan **instrucciones claras** al modelo.  
- 🧩 Especifican la **estructura JSON exacta** que debe seguir.  
- 🎯 Indican los **campos obligatorios**: título, género y motivo.  
- 📝 Incluyen un **ejemplo de salida** que guía al modelo para replicar el formato.  

Gracias a esto, el modelo responde de forma coherente y directamente utilizable.

---

## 🧑‍💻 Prompts

👉 Prompt 1:
```
Recomienda 3 películas en formato JSON.
Cada película debe tener:
- título
- género
- motivo de recomendación

Ejemplo de formato:
"""[
  {"título": "...", "género": "...", "motivo": "..."},
  {"título": "...", "género": "...", "motivo": "..."},
  {"título": "...", "género": "...", "motivo": "..."}
]"""
```

👉 Prompt 2:
```
Proporcione una lista de tres recomendaciones de películas en formato JSON.

Cada película debe incluir:

“Título”: el título de la película  
“Género”: el género de la película  
“Motivo”: el motivo por el que recomienda la película  

Asegúrese de que el JSON esté correctamente estructurado y siga el siguiente formato:

[
  {"Título": "Título de la película 1", "Género": "Género 1", "Motivo": "Motivo 1"},
  {"Título": "Título de la película 2", "Género": "Género 2", "Motivo": "Motivo 2"},
  {"Título": "Título de la película 3", "Género": "Género 3", "Motivo": "Motivo 3"}
]
```

---

## 🎬 Ejemplos de Salida

➡ **Ejemplo 1**
```json
[
  {
    "título": "Pulp Fiction",
    "género": "Acción",
    "motivo": "La mezcla perfecta de acción, drama y humor"
  },
  {
    "título": "La lista de Schindler",
    "género": "Drama",
    "motivo": "Un relato poderoso y emotivo sobre la humanidad"
  },
  {
    "título": "Inception",
    "género": "Ciencia ficción",
    "motivo": "Una experiencia visual y mental deslumbrante"
  }
]
```

➡ **Ejemplo 2**
```json
[
  {
    "Título": "Interstellar",
    "Género": "Ciencia Ficción",
    "Motivo": "Una obra maestra visual y conceptual que explora temas profundos como el tiempo y el futuro de la humanidad."
  },
  {
    "Título": "El Padrino",
    "Género": "Drama Criminal",
    "Motivo": "Un clásico atemporal que define el género de gánsteres, con actuaciones legendarias y una historia sobre poder y lealtad."
  },
  {
    "Título": "Amélie",
    "Género": "Comedia Romántica / Fantasía",
    "Motivo": "Una película encantadora y visualmente poética que te transporta a un París mágico."
  }
]
```
---

## ⚡ Cómo usar esta herramienta

1. 🔑 Necesitás la **API Key de gemini**.  
2. 🖥️ Ejecutá el código en **Google Colab** o en tu entorno local con Python.  
3. 📦 Si es en un entorno local con python instalá las dependencias necesarias:
   ```bash
   pip install transformers accelerate
   ```
4. 📤 Ejecuta todas las casillas de codigo y recibí el JSON con las recomendaciones de películas.  

✅ ¡Listo! Tendrás respuestas en formato estructurado para integrarlas en cualquier aplicación.  

---



