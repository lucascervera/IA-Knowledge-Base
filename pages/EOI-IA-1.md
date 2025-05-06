public:: true

- ## Evolución de la inteligencia artificial aplicada a la generación de  imágenes
- IA imagen
- ## Herramientas de IA imagen
  collapsed:: true
	- Elección de la herramienta concreta
		- Principio de pareto.
		- Directorios de aplicaciones basadas en IA
		- Herramientas propietarias versus Open Source
		- Funcionalidad, SaaS, API o local
		- Para utilizar en tu trabajo
		- Para utilizar en esta clase
			- ChatGPT
			- Replicate
			- Leonardo
			- Pinokio
- ## Funcionalidades de la inteligencia artificial para la generación de imagen
	- Creación de imágenes a partir de promts de texto
	- Creación de imágenes a partir de imágenes
	- Edición de imágenes con out paint e in painting.
	- Creación de personajes consistentes
	- Quitar el fondo a una imagen
	- Crear una imagen de producto a partir de una foto de mala calidad.
	- Aumentar la resolución de una imagen
	- Generar un modelo 3D a partir de una descripción de texto
	- Generación de texto dentro de una imagen
	- Creación de logos
	- ...
	- Creación de imágenes a partir de prompts de texto
		- Permite generar ilustraciones o fotografías sintéticas a partir de descripciones en lenguaje natural.
		- Inputs: Prompt de texto (descripción detallada)
		- Outputs: Imagen digital (JPEG, PNG)
		- Herramientas: [DALL·E](https://openai.com/product/dall-e), [Midjourney](https://www.midjourney.com/), [Stable Diffusion](https://stability.ai/)
		- Pasos:  
		  1. Redactar prompt claro y detallado.  
		  2. Enviar a la API o interfaz.  
		  3. Revisar resultados y ajustar prompt si es necesario.
	- Creación de imágenes a partir de imágenes
		- Transforma o extiende una imagen existente para generar variaciones o completar zonas faltantes.
		- Inputs: Imagen base
		- Outputs: Imagen transformada
		- Herramientas: [Stable Diffusion img2img](https://stability.ai/), [Photoshop Generative Fill](https://www.adobe.com/products/photoshop.html)
		- Pasos:  
		  1. Subir o seleccionar la imagen original.  
		  2. Definir parámetros de transformación (fuerza, estilo).  
		  3. Ejecutar y revisar; iterar ajustes.
	- Edición de imágenes con outpainting e inpainting
		- Rellena zonas faltantes (outpaint) o corrige imperfecciones (inpaint) manteniendo coherencia visual.
		- Inputs: Imagen con área señalada para rellenar
		- Outputs: Imagen completa sin defectos
		- Herramientas: [Photoshop Generative Fill](https://www.adobe.com/products/photoshop.html), [Stable Diffusion Inpainting](https://stability.ai/)
		- Pasos:  
		  1. Marcar área a rellenar o corregir.  
		  2. Ejecutar algoritmo de in/outpainting.  
		  3. Ajustar máscara y repetir si es necesario.
	- Creación de personajes consistentes
		- Genera múltiples ilustraciones del mismo personaje manteniendo rasgos y estilo uniforme.
		- Inputs: Descripción del personaje y ejemplos de referencia
		- Outputs: Serie de imágenes del mismo personaje
		- Herramientas: [Character.ai](https://beta.character.ai/), Midjourney + prompt anchoring
		- Pasos:  
		  1. Definir y refinar prompt “anchoring” (rasgos clave).  
		  2. Generar lote de imágenes.  
		  3. Seleccionar y ajustar el prompt para consistencia.
	- Quitar el fondo a una imagen
		- Elimina automáticamente el fondo dejando el sujeto principal en primer plano.
		- Inputs: Imagen con sujeto y fondo
		- Outputs: PNG con fondo transparente
		- Herramientas: [remove.bg](https://www.remove.bg/), [Photoshop Select Subject](https://www.adobe.com/products/photoshop.html)
		- Pasos:  
		  1. Subir imagen.  
		  2. Aplicar detección de sujeto.  
		  3. Descargar recorte en PNG.
	- Crear una imagen de producto a partir de una foto de mala calidad
		- Mejora color, nitidez y elimina artefactos para obtener una imagen de catálogo.
		- Inputs: Foto de baja resolución o mal iluminada
		- Outputs: Imagen optimizada de alta calidad
		- Herramientas: [Topaz Gigapixel AI](https://www.topazlabs.com/gigapixel-ai), [Adobe Enhance](https://www.adobe.com/products/photoshop.html)
		- Pasos:  
		  1. Subir foto original.  
		  2. Aplicar mejoras automáticas (super‑res, balance de color).  
		  3. Ajustar manualmente si es necesario.
	- Aumentar la resolución de una imagen
		- Escala una imagen a mayor tamaño manteniendo detalle y reduciendo ruido.
		- Inputs: Imagen de baja resolución
		- Outputs: Imagen de resolución superior
		- Herramientas: [ESRGAN](https://github.com/xinntao/ESRGAN), [Gigapixel AI](https://www.topazlabs.com/gigapixel-ai)
		- Pasos:  
		  1. Seleccionar factor de escala (2×, 4×).  
		  2. Ejecutar modelo de super‑resolución.  
		  3. Revisar y recortar bordes si conviene.
	- Generar un modelo 3D a partir de una descripción de texto
		- Crea geometría 3D básica (mesh) basándose en instrucciones textuales.
		- Inputs: Prompt de texto con detalles de forma y medidas
		- Outputs: Archivo 3D (.obj, .fbx)
		- Herramientas: [OpenAI Point‑E](https://github.com/openai/point-e), [NVIDIA Instant NeRF](https://developer.nvidia.com/instant-nerf)
		- Pasos:  
		  1. Redactar prompt con dimensiones y estilo.  
		  2. Pasar a la API de modelado.  
		  3. Descargar y revisar en visor 3D; refinar si hace falta.
	- Generación de texto dentro de una imagen
		- Incorpora automáticamente rótulos, subtítulos o marcas de agua en imágenes.
		- Inputs: Imagen base + texto a insertar
		- Outputs: Imagen con texto integrado
		- Herramientas: [Canva Text‑to‑Image](https://www.canva.com/features/text-to-image/), [Photoshop Generative Type](https://www.adobe.com/products/photoshop.html)
		- Pasos:  
		  1. Especificar posición y estilo del texto.  
		  2. Ejecutar generación.  
		  3. Ajustar tamaño y tipografía.
	- Creación de logos
		- Diseña logotipos vectoriales o raster basados en brief de marca.
		- Inputs: Descripción de marca, colores y estilo preferido
		- Outputs: Archivo de logo (.svg, .png)
		- Herramientas: [Looka](https://looka.com/), [Tailor Brands](https://www.tailorbrands.com/)
		- Pasos:  
		  1. Proporcionar brief y ejemplos de inspiración.  
		  2. Generar varias propuestas.  
		  3. Seleccionar y afinar tipografía/colores.
	- Conversión de una foto a un estilo artístico (style transfer)
		- Aplica la apariencia de un pintor famoso o estilo gráfico a una imagen.
		- Inputs: Imagen original + imagen de estilo
		- Outputs: Imagen con nuevo estilo aplicado
		- Herramientas: [DeepArt](https://deepart.io/), [Fast Neural Style Transfer](https://github.com/jcjohnson/neural-style)
		- Pasos:  
		  1. Subir imagen de contenido y de estilo.  
		  2. Ejecutar transferencia de estilo.  
		  3. Ajustar intensidad del efecto.
	- Animación de retratos (p.ej. hacer que una foto hable o sonría)
		- Genera un vídeo corto animando expresiones faciales basadas en audio o guión.
		- Inputs: Retrato estático + audio o guión de voz
		- Outputs: Clip animado (MP4)
		- Herramientas: [Wombo](https://www.wombo.art/), [D‑ID](https://www.d-id.com/)
		- Pasos:  
		  1. Subir retrato y audio.  
		  2. Ajustar parámetros de sincronización labial.  
		  3. Descargar vídeo generado.
	- Interpolación entre imágenes para crear transiciones fluidas (morphing)
		- Crea cuadros intermedios para fundir dos imágenes en un clip animado.
		- Inputs: Imagen A, Imagen B
		- Outputs: Secuencia de imágenes o vídeo de transición
		- Herramientas: [RIFE](https://github.com/hzwer/arXiv2020-RIFE), [Flowframes](https://nmkd.itch.io/flowframes)
		- Pasos:  
		  1. Seleccionar pares de imágenes.  
		  2. Ajustar número de fotogramas intermedios.  
		  3. Generar y exportar vídeo.
	- Colorización automática de fotos en blanco y negro
		- Añade colores a imágenes monocromas preservando naturalidad y texturas.
		- Inputs: Fotografía B/N
		- Outputs: Fotografía a color
		- Herramientas: [Algorithmia Colorize](https://algorithmia.com/models/deeplearning/ColorfulImageColorization), [DeOldify](https://github.com/jantic/DeOldify)
		- Pasos:  
		  1. Subir foto en blanco y negro.  
		  2. Ejecutar modelo de colorización.  
		  3. Retocar tonos si es necesario.
	- Restauración de imágenes dañadas o antiguas
		- Elimina arañazos, manchas y recupera zonas perdidas en fotografías históricas.
		- Inputs: Imagen escaneada dañada
		- Outputs: Imagen restaurada
		- Herramientas: [PhotoGlory](https://photoglory.net/), [Photoshop Neural Filters](https://www.adobe.com/products/photoshop.html)
		- Pasos:  
		  1. Analizar zonas a reparar.  
		  2. Ejecutar algoritmo de restauración.  
		  3. Pulir detalles manualmente.
	- Detección de objetos dentro de imágenes
		- Identifica y localiza automáticamente elementos (personas, coches, señales).
		- Inputs: Imagen o vídeo
		- Outputs: Bounding boxes con etiquetas y puntuaciones
		- Herramientas: [YOLOv5](https://github.com/ultralytics/yolov5), [Detectron2](https://github.com/facebookresearch/detectron2)
		- Pasos:  
		  1. Cargar imagen en el detector.  
		  2. Evaluar resultados y revisar etiquetas.  
		  3. Exportar datos en JSON o CSV.
	- Clasificación de imágenes por contenido (etiquetado automático)
		- Asigna categorías o tags a cada imagen según su contenido.
		- Inputs: Lote de imágenes
		- Outputs: Lista de etiquetas por imagen
		- Herramientas: [Google Vision](https://cloud.google.com/vision), [Azure Computer Vision](https://azure.microsoft.com/services/cognitive-services/computer-vision/)
		- Pasos:  
		  1. Subir lote de imágenes.  
		  2. Ejecutar API de clasificación.  
		  3. Descargar informe de etiquetas.
	- Segmentación semántica (identificación de cada píxel por categoría)
		- Crea máscaras detalladas para cada objeto o región en la imagen.
		- Inputs: Imagen
		- Outputs: Mapas de segmentación
		- Herramientas: [U-Net](https://en.wikipedia.org/wiki/U-Net_(neural_network)), [DeepLab](https://github.com/tensorflow/models/tree/master/research/deeplab)
		- Pasos:  
		  1. Preprocesar imagen (ajuste de tamaño).  
		  2. Ejecutar modelo de segmentación.  
		  3. Aplicar máscara sobre la imagen.
	- Generación de imágenes a partir de datos médicos (radiografías, resonancias, etc.)
		- Sintetiza vistas médicas para entrenamiento o aumento de datos clínicos.
		- Inputs: Parámetros clínicos o imágenes de baja calidad
		- Outputs: Imágenes médicas generadas o mejoradas
		- Herramientas: [MedGAN](https://github.com/jsyoon0823/medgan), [NVIDIA Clara](https://developer.nvidia.com/clara-medical-imaging)
		- Pasos:  
		  1. Definir tipo de imagen y parámetros.  
		  2. Ejecutar generación o mejora.  
		  3. Validar consistencia clínica con experto.
	- Creación de fondos generativos para uso en videojuegos o diseño
		- Produce paisajes, nubes o texturas repetibles para escenarios 2D/3D.
		- Inputs: Parámetros de estilo y paleta de colores
		- Outputs: Texturas o tilesets
		- Herramientas: [NVIDIA Canvas (GauGAN)](https://www.nvidia.com/en-us/studio/canvas/), [Artbreeder](https://www.artbreeder.com/)
		- Pasos:  
		  1. Definir esquema de color y tema.  
		  2. Generar variaciones.  
		  3. Exportar assets.
	- Generación de imágenes hiperrealistas de personas que no existen
		- Crea retratos fotográficos de rostros ficticios con alta fidelidad.
		- Inputs: Parámetros demográficos (edad, sexo, etnia)
		- Outputs: Imagen de rostro (PNG/JPEG)
		- Herramientas: [StyleGAN2](https://github.com/NVlabs/stylegan2), [ThisPersonDoesNotExist](https://thispersondoesnotexist.com/)
		- Pasos:  
		  1. Ajustar sliders demográficos.  
		  2. Generar muestra de rostros.  
		  3. Seleccionar el más adecuado.
	- Reconocimiento facial y generación de rostros a partir de descripciones
		- Detecta rostros en fotos y puede generar retratos basados en texto.
		- Inputs: Foto de grupo o descripción textual
		- Outputs: Coordenadas de rostros / retrato generado
		- Herramientas: [Face++](https://www.faceplusplus.com/), [Generated Photos](https://generated.photos/)
		- Pasos:  
		  1. Ejecutar detección en la imagen.  
		  2. Para generación, redactar descripción.  
		  3. Generar y comparar con expectativas.
	- Creación de texturas y patrones para diseño gráfico o 3D
		- Genera estampados, mosaicos y mapas de desplazamiento para superficies.
		- Inputs: Ejemplos de patrón o prompt textual
		- Outputs: Textura seamless (PNG)
		- Herramientas: [Substance 3D Alchemist](https://www.adobe.com/products/substance3d-alchemist.html)
		- Pasos:  
		  1. Definir tipo de patrón y escala.  
		  2. Generar y ajustar seamlessness.  
		  3. Exportar en formato adecuado.
	- Diseño de ropa o moda virtual sobre modelos
		- Superpone diseños de prendas en maniquíes o fotografías de modelos.
		- Inputs: Fotografía de modelo + diseño de prenda
		- Outputs: Imagen de modelo vistiendo la prenda
		- Herramientas: [Clo3D](https://www.clo3d.com/), [Vue.ai](https://vue.ai/)
		- Pasos:  
		  1. Subir foto del maniquí o modelo.  
		  2. Cargar diseño de prenda (vectorial o imagen).  
		  3. Ajustar calce y renderizar.
	- Reconstrucción de escenas en 3D a partir de fotos 2D
		- Genera modelo volumétrico o malla 3D de un entorno real.
		- Inputs: Serie de fotografías desde distintos ángulos
		- Outputs: Modelo 3D texturizado
		- Herramientas: [Pix4D](https://www.pix4d.com/), [Agisoft Metashape](https://www.agisoft.com/)
		- Pasos:  
		  1. Importar todas las fotos.  
		  2. Ejecutar reconstrucción fotogramétrica.  
		  3. Limpiar malla y exportar.
	- Conversión de bocetos o dibujos en imágenes realistas
		- Transforma líneas y contornos en ilustraciones acabadas.
		- Inputs: Boceto escaneado o digital
		- Outputs: Imagen coloreada y sombreada
		- Herramientas: [Adobe Fresco](https://www.adobe.com/products/fresco.html), [Sketch2Image](https://github.com/tg-bomze/Sketch2Image)
		- Pasos:  
		  1. Subir boceto.  
		  2. Elegir estilo de coloreado.  
		  3. Ejecutar y retocar manualmente.
	- Creación de cómics o novelas gráficas a partir de guiones
		- Genera viñetas con personajes, diálogos y ambientación según un guión.
		- Inputs: Guión por escenas (texto)
		- Outputs: Páginas de cómic (PNG/PDF)
		- Herramientas: [ComicGen](https://www.comicgen.io/), Midjourney + prompts secuenciales
		- Pasos:  
		  1. Dividir guión en escenas.  
		  2. Generar cada viñeta por separado.  
		  3. Montar páginas y añadir bocadillos.
	- Composición automática de imágenes con múltiples elementos coherentes
		- Ensambla varios activos (personajes, fondos, objetos) en una sola escena equilibrada.
		- Inputs: Lista de elementos y prompt de composición
		- Outputs: Imagen compuesta final
		- Herramientas: [RunwayML Gen-2](https://runwayml.com/), [LayoutGAN](https://github.com/facebookresearch/LayoutGAN)
		- Pasos:  
		  1. Definir assets y posición aproximada.  
		  2. Ejecutar composición.  
		  3. Ajustar escala y luz.
	- Vectorización automática de imágenes
		- Convierte imágenes raster (píxeles) en trazados vectoriales escalables.
		- Inputs: Imagen raster (logo, ilustración)
		- Outputs: Archivo .svg o .ai
		- Herramientas: [Illustrator Image Trace](https://www.adobe.com/products/illustrator.html), [Inkscape Trace Bitmap](https://inkscape.org/)
		- Pasos:  
		  1. Importar imagen raster.  
		  2. Ejecutar trazado automático.  
		  3. Ajustar nodos y simplificar curvas.
	- Simulación de efectos fotográficos (profundidad de campo, desenfoque, etc.)
		- Añade bokeh, viñeteado o desenfoque selectivo para mejorar el aspecto.
		- Inputs: Imagen original + parámetros de efecto
		- Outputs: Imagen con efecto fotográfico aplicado
		- Herramientas: [Luminar AI](https://skylum.com/luminar-ai), [Photoshop Neural Filters](https://www.adobe.com/products/photoshop.html)
		- Pasos:  
		  1. Seleccionar tipo de efecto y área de aplicación.  
		  2. Ajustar intensidad.  
		  3. Aplicar y refinar máscaras si conviene.
- ## Preparación del entorno de trabajo
  collapsed:: true
	- Necesitas
		- Una cuenta de Google
		- Una cuenta de [Chat GPT](https://chatgpt.com/)
		- Una cuenta de [Leonardo.ai](https://leonardo.ai/)
		- Una carpeta de Google Drive llamada [EOI-IA-1 Carpeta de trabajo]("https://drive.google.com/drive/folders/1Yf1SwV3SgoEuY0yDKaa9s27yMXcVh_R8)
		- Una idea de negocio o producto
			- Beerbrella Patente: [https://patents.google.com/patent/US2...](https://patents.google.com/patent/US6637447B2/en)
- ## Generación de imágenes desde texto (Text-to-Image)
  collapsed:: true
	- **Descripción**: Crear imágenes originales a partir de descripciones en lenguaje natural.
	- ### Foto de producto.
		- Prompt:
			- ```
			  The present invention provides a small umbrella (“Beerbrella”) which may be removably attached to a beverage container in order to shade the beverage container from the direct rays of the sun. The apparatus comprises a small umbrella approximately five to seven inches in diameter, although other appropriate sizes may be used within the spirit and scope of the present invention. Suitable advertising and/or logos may be applied to the umbrella surface for promotional purposes. The umbrella may be attached to the beverage container by any one of a number of means, including clip, strap, cup, foam insulator, or as a coaster or the like. The umbrella shaft may be provided with a pivot to allow the umbrella to be suitably angled to shield the sun or for aesthetic purposes. In one embodiment, a pivot joint and counterweight may be provided to allow the umbrella to pivot out of the way when the user drinks from the container.
			  ```
		- ChatGPT
			- ![image.png](../assets/image_1745928266499_0.png){:height 174, :width 555}
		- [Invención de Beerbrella](https://chatgpt.com/share/6810c2c6-fe8c-800c-9ba1-682b71e568e3)
			- ![ChatGPT Image 29 abr 2025, 14_14_46.png](../assets/ChatGPT_Image_29_abr_2025,_14_14_46_1745929664533_0.png)
	- ### Foto de persona
		- [Bebedor de cerveza español](https://chatgpt.com/share/6810c535-4f48-800c-8e5f-9d233a6fa74d)
			- ![ChatGPT Image 29 abr 2025, 14_24_49.png](../assets/ChatGPT_Image_29_abr_2025,_14_24_49_1745929737774_0.png)
- ## Transformación de imágenes (Image-to-Image)
  collapsed:: true
	- **Descripción**: Tomar una imagen de entrada y generar variaciones manteniendo el estilo o contenido.
	- **Prompt**: `Ponle un poco más de tripa`
	- ![image.png](../assets/image_1745930103736_0.png)
	- ## Eliminación de fondo y segmentación
	  
	  **Descripción**: Separar sujeto y fondo para montajes o transparencias.
	-
	- ![image.png](../assets/image_1745931374965_0.png)
	- [Explore – Replicate](https://replicate.com/explore#featured-models)
	- ## 3. Edición de imágenes (Sustituir cara)
	  
	  **Descripción**: A partir de una imagen de referencia de una persona, sustituye su cara con la imagen de otra cara.
		- [Prediction cdingram/face-swap – Replicate](https://replicate.com/p/sdwjfxza0drj60cpg6nv7z65zr)
		- ![replicate-prediction-sdwjfxza0drj60cpg6nv7z65zr.jpg](../assets/replicate-prediction-sdwjfxza0drj60cpg6nv7z65zr_1745933183958_0.jpg){:height 527, :width 346}
	-
- ## Edición de imágenes (Upscaling)
  collapsed:: true
	- **Descripción**: Mejora la calidad de una imagen ampliando sus dimensiones y refinando los detalles.
	- [Prediction fermatresearch/high-resolution-controlnet-tile – Replicate](https://replicate.com/p/60wfkgat8srma0cpg6ra98byeg)
	- ![replicate-prediction-60wfkgat8srma0cpg6ra98byeg.jpg](../assets/replicate-prediction-60wfkgat8srma0cpg6ra98byeg_1745933210710_0.jpg)
	- ## Edición de imágenes mediante texto
		- [Cerveza personalizada playa fiesta](https://chatgpt.com/c/6810d739-dc88-800c-8f9d-149264d8b0b3)
		- ![image.png](../assets/image_1745934456186_0.png)
- ## Modelado 3D a partir de texto o imagen
  collapsed:: true
	- **Descripción**: Generar mallas y entornos 3D.
	- https://lumalabs.ai/genie?view=create
- ## Herramientas IA / imagen
  collapsed:: true
	- **Leonardo AI**: [https://www.leonardo.ai/](https://www.leonardo.ai/)
	- **Replicate**: [https://www.replicate.com/](https://www.replicate.com/)
	- **Pinokio**: [https://pinokio.computer/](https://pinokio.computer/)
- ## Automatización de creación de imágenes
  collapsed:: true
	- Consideraciones éticas ilegales de la generación de imágenes con IA.
	- Sesgos en la generación de imágenes con IA.
- ## Casos de uso inteligencia artificial para imagen y vídeo
  collapsed:: true
	- **12:33** [[quick capture]]:  Actualización de películas con IA #innovación #inteligenciaartificial #video - YouTube {{video https://www.youtube.com/watch?v=wVH1GcpcNFg}}
		- @misc{ai_2024, title={Luma Dream Machine}, url={[https://lumalabs.ai/dream-machine](https://www.youtube.com/redirect?event=video_description&redir_token=QUFFLUhqbkdQN2JwbTlYcllaY2tlU0hlVHY2TjI3LWlxQXxBQ3Jtc0traERQcmRZVl9fWDJyampYcThaYWNsM1VabE5NY2p6RUVjZFVkZVRYN1F2SnlpclEySkhyT2ZKWEJWYnJFM1VjcWpuRUhWeC1UaTJhUTM1Y1RQd0hSX2htWVVobGNyU1VKWHN5cjdpT25KdHg0bXZjYw&q=https%3A%2F%2Flumalabs.ai%2Fdream-machine&v=wVH1GcpcNFg)}, journal={Luma Dream Machine}, author={AI, Luma}, year={2024} }
		- En un escenario hipotético de rodaje en 2024, escenas icónicas del cine como la de "Casablanca" serían capturadas en selfies para Instagram. La tecnología actual podría recrear videos de alta calidad a partir de una simple foto y un texto con instrucciones. Otras películas como "Con la muerte en los talones" y "Cantando bajo la lluvia" se adaptarían al uso de drones y al cambio climático, respectivamente.
	- **12:37** [[quick capture]]:  Inteligencia Artificial y robótica - YouTube {{video https://www.youtube.com/watch?v=mFAMwTxULhw}}
	- **12:42** [[quick capture]]:  Texto a impresión 3D con inteligencia artificial - YouTube {{video https://www.youtube.com/watch?v=5HW13lm2RMQ}}
	- Inteligencia Artificial para traducir vídeos - YouTube {{video https://www.youtube.com/watch?v=nPEUs9ifZzY}}
	- **12:45** [[quick capture]]:  Inteligencia artificial para detectar cáncer #innovacion #ia - YouTube {{video https://www.youtube.com/watch?v=mbghc4c_QrY}}
	- **12:46** [[quick capture]]:  De imagen a modelo 3D con IA #innovacion #inteligenciaartificial #video - YouTube {{video https://www.youtube.com/watch?v=F6p6k5Vz3RE}}
	- **12:48** [[quick capture]]:  Añade efectos especiales a tu video con IA #innovación #video #inteligenciaartificial - YouTube {{video https://www.youtube.com/watch?v=cnp9A__4Egw}}
	- **12:49** [[quick capture]]:  Deepfakes y suplantación de identidad #innovacion #seguridad #inteligenciaartificial - YouTube {{video https://www.youtube.com/watch?v=RMUzzEg1Uhg}}
	- **12:51** [[quick capture]]:  Texto a vídeo con inteligencia artificial - YouTube {{video https://www.youtube.com/watch?v=-TV8rwwCne0}}
	- **12:52** [[quick capture]]:  Inteligencia artificial crea vídeos a partir de texto - YouTube {{video https://www.youtube.com/watch?v=cx4M6RQkcaI}}
	- **12:53** [[quick capture]]:  Inteligencia artificial para borrar cosas de vídeos - YouTube {{video https://www.youtube.com/watch?v=mKbe2MUh60o}}
	- **12:54** [[quick capture]]:  La inteligencia artificial ángel o demonio - YouTube {{video https://www.youtube.com/watch?v=1mQWcoSRYeE}}
	- **12:56** [[quick capture]]:  RunwayML gen 2 Crea vídeos a partir de texto #innovación #vídeo vertical subtitles - YouTube {{video https://www.youtube.com/watch?v=NfGh0_8576s}}
	- **12:58** [[quick capture]]:  Leonardo ai crea tu foto de prom #innovacion #ia #text2image - YouTube {{video https://www.youtube.com/watch?v=3qZQH8uf8uY}}
		- #LORA
	- **13:00** [[quick capture]]:  Crea un personaje con Dall e 3 #innovacion #inteligenciaartificial - YouTube {{video https://www.youtube.com/watch?v=G4AeRTs3HDc}}
	- **13:02** [[quick capture]]:  IA mezcla foto y vídeo #innovación #inteligenciaartificial - YouTube {{video https://www.youtube.com/watch?v=M60rKxEcvnw}}
	- **13:03** [[quick capture]]:  Crea canciones con inteligencia artificial #innovación #inteligenciaartificial #música - YouTube {{video https://www.youtube.com/watch?v=Dk_Eg_zCkuA}}
	- **13:04** [[quick capture]]:  Clona estilos musicales con IA (suno) #innovación #música #inteligenciaartificial - YouTube {{video https://www.youtube.com/watch?v=-dlEgstx6qY}}
	- **13:05** [[quick capture]]:  De ecografía 3D a rostro con IA #innovacion #inteligenciaartificial #medicina - YouTube {{video https://www.youtube.com/watch?v=xrWTWHbNmEk&t=13s}}
	- **13:08** [[quick capture]]:  App para generar tu avatar super realista - YouTube {{video https://www.youtube.com/watch?v=a9OQthbAYhQ&t=18s}}
	- **13:08** [[quick capture]]:  Avatar creado con inteligencia artificial - YouTube {{video https://www.youtube.com/watch?v=vOPX3UYZJEQ}}
	- **13:11** [[quick capture]]:  Crea vídeos con una foto y un texto con vidu.estudio #innovación #inteligenciaartificial #vídeo - YouTube {{video https://www.youtube.com/watch?v=vw13hKt1xPU&t=9s}}
	- **13:12** [[quick capture]]:  Imagen a texto con Inteligencia Artificial #innovacion #IA - YouTube {{video https://www.youtube.com/watch?v=Es65cvCrw6k}}
-