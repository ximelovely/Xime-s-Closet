# ✦ Xime's Closet — Adaptive Neural Stylist ✦
> Un optimizador de outfits inteligente que fusiona la moda con redes neuronales.

Este proyecto es una aplicación web interactiva diseñada para gestionar un armario personal y generar combinaciones de ropa inteligentes basadas en el contexto diario (clima, ocasión y "vibe"). Utiliza un motor de lógica "neural" simulado para calcular la compatibilidad de estilos y colores.

---

## ✨ Características Principales
- **Gestión de Armario:** Interfaz intuitiva para añadir prendas con atributos de tipo, color y estilo.
- **Neural Engine:** Algoritmo que genera una puntuación de compatibilidad (score) basada en matrices de armonía de color y estilo.
- **Context Awareness:** Ajusta las sugerencias según el clima (desde caluroso hasta frío/lluvioso) y la ocasión.
- **Visualización de Red:** Animación de barras que representa la activación de los "embeddings" de la prenda durante el cálculo.
- **Historial de Estilo:** Guarda tus combinaciones favoritas para consultarlas después.

---

## 🎨 Estética: "Silk & Stone"
El diseño se basa en una paleta de colores sofisticada y femenina:
- **Fondo:** Crema suave (`#F9F1E3`) con texturas de gradiente.
- **Acentos:** Verde salvia (`#5B8C85`), Tan (`#A68A73`) y Carbón (`#2D2D2D`).
- **Tipografía:** Una combinación elegante de *Playfair Display* (Serif) y *DM Mono* para ese toque técnico y moderno.

---

## 🛠️ Tecnologías Utilizadas
- **HTML5 & CSS3:** Layouts personalizados con Grid y Flexbox, variables CSS y animaciones `@keyframes`.
- **Vanilla JavaScript:** Lógica de estado para la gestión del armario y el motor de recomendación.
- **LocalStorage:** Persistencia de datos para que tu armario y tu historial se mantengan al recargar la página.

---

## 🧠 Lógica del Motor Neural
El sistema utiliza una función de **Embeddings** que mapea las características de las prendas a un vector de 20 dimensiones.
- Los primeros 8 índices corresponden a la activación por **Estilo**.
- Los siguientes 12 índices corresponden a la activación por **Color**.
- Se aplica un *boost* de contexto según la ocasión seleccionada para normalizar el vector y generar la recomendación ideal.