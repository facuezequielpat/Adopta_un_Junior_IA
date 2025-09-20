# 🎓 Adopta_un_Junior_IA

Mira mi proyecto desde aca: 📌 [Notebook en Google Colab](https://colab.research.google.com/drive/1W4I4se4GHpiCEmHsw7nafFAY4OI7gB_u?usp=sharing)

---

## ❓ ¿Por qué funcionan mis prompts?

Mis prompts funcionan porque:  
- 📐 Dan **instrucciones claras** al modelo.  
- 🧩 Especifican la **estructura JSON exacta** que debe seguir.  
- 🎯 Indican los **campos obligatorios**: título, género y motivo.
- ✅  Tiene una **mayor personalizacion** el usuario debe poner su Edad, Pelicula preferida, y Estado de animo actual (Inspirado por uno de mis compañeros)  
- 📝 Incluyen un **ejemplo de salida** que guía al modelo para replicar el formato.


Gracias a esto, el modelo responde de forma coherente y directamente utilizable.

---

## 🧑‍💻 Prompts

👉 Prompt 1:
```
Recomienda 3 películas en formato JSON.

Teniendo en cuenta la Edad:{Edad}
Teniendo en cuenta la Pelicula favorita:{Pelicula_preferida}
Teniendo en cuenta el Estado de animo actual:{Estado_de_animo_actual}

Cada película debe tener:
- título
- género
- motivo de recomendación

Ejemplo de formato:
[
  {"título": "...", "género": "...", "motivo": "..."},
  {"título": "...", "género": "...", "motivo": "..."},
  {"título": "...", "género": "...", "motivo": "..."}
]

No añadas explicaciones ni texto fuera del bloque JSON.
```

👉 Prompt 2:
```
Proporcione una lista de tres recomendaciones de películas en formato JSON.

Teniendo en cuenta la Edad:{Edad}
Teniendo en cuenta la Pelicula favorita:{Pelicula_preferida}
Teniendo en cuenta el Estado de animo actual:{Estado_de_animo_actual}

Cada película debe incluir:

“Título”: el título de la película
“Género”: el género de la película
“Motivo”: el motivo por el que recomienda la película
Asegúrese de que el JSON esté correctamente estructurado y siga el siguiente formato:
[
{“Título”: “Título de la película 1”, “Género”: “Género 1”, “motivo”: “Motivo para recomendar la película 1”},
{“Título”: “Título de la película 2”, “Género”: “Género 2”, “motivo”: “Motivo para recomendar la película 2”},
{“Título”: “Título de la película 3”, “Género”: “Género 3”, “motivo”: “Motivo para recomendar la película 3”}
]
```

---

## 🎬 Ejemplos de Salida

➡ **Ejemplo 1**
```
[
  {"título": "Inception", "género": "Acción, Ciencia Ficción", "motivo": "Dado tu estado de ánimo actual, 'Inception' podría ayudar a distraerte con su intrincada trama y efectos visuales impresionantes."},
  {"título": "La lista de Schindler", "género": "Drama, Histórico", "motivo": "Como te gusta la película 'IT', 'La lista de Schindler' ofrece una historia poderosa y conmovedora que podría resonar contigo."},
  {"título": "El Gran Hotel Harcourt", "género": "Comedia, Drama", "motivo": "Para un cambio de ritmo, 'El Gran Hotel Harcourt' ofrece una mezcla de humor y drama, ideal para calmar tu estado de ánimo."}
]
```

➡ **Ejemplo 2**
```json
[
  {
    "Título": "John Wick: Capítulo 4",
    "Género": "Acción, Thriller",
    "Motivo": "Para canalizar la energía del enojo, esta película ofrece una acción implacable y coreografías espectaculares. La venganza del protagonista puede ser catártica y la intensidad te mantendrá al borde del asiento, ideal para un estado de ánimo enojado."
  },
  {
    "Título": "Se7en (Seven: Pecados Capitales)",
    "Género": "Thriller, Crimen, Misterio",
    "Motivo": "Si te gusta la oscuridad y la intensidad de 'IT', este thriller psicológico te sumergirá en una atmósfera sombría y perturbadora. Su tensión constante y giros inesperados son perfectos para distraerte y mantener tu mente ocupada en una narrativa visceral."
  },
  {
    "Título": "Fight Club (El Club de la Lucha)",
    "Género": "Drama, Thriller, Sátira",
    "Motivo": "Una película provocadora y reflexiva que explora la frustración y la rabia en la sociedad moderna. Su estilo audaz y su mensaje subversivo pueden resonar con un estado de ánimo de enojo, ofreciendo una válvula de escape intelectual y emocional a tu edad."
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



