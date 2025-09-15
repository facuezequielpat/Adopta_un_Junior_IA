# Adopta_un_Junior_IA

# Por que funcionan mis prompts?

## Prompts



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




Proporcione una lista de tres recomendaciones de películas en formato JSON.

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

## Salidas

[
  {
    "título": "Pulp Fiction",
    "género": "Accion",
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

[
  {
    "Título": "Interstellar",
    "Género": "Ciencia Ficción",
    "Motivo": "Una obra maestra visual y conceptual que explora temas profundos como el tiempo, la paternidad y el futuro de la humanidad, con una banda sonora inolvidable."
  },

  {
    "Título": "El Padrino",
    "Género": "Drama Criminal",
    "Motivo": "Un clásico atemporal que define el género de gánsteres, con actuaciones legendarias, una dirección impecable y una historia compleja sobre la familia, el poder y la lealtad."
  },
  
  {
    "Título": "Amélie",
    "Género": "Comedia Romántica / Fantasía",
    "Motivo": "Una película encantadora y visualmente poética que te transporta a un París mágico, llena de personajes excéntricos y un optimismo contagioso que te dejará con una sonrisa."
  }
]

## Porque?


Este prompt funciona porque da **instrucciones claras** al modelo, indicando tanto la **estructura del JSON** como los **campos requeridos**.  
Además, incluye un **ejemplo de salida** que el modelo replica con coherencia.



