-
- ## Sample outline
	- [[Alma Flamenca - Web Oficial]] # Este es el bloque raíz de la página (Nivel 0)
	  title:: Alma Flamenca - La Fusión del Duende
	  lang:: es
	- # Este bloque no necesita section_type ni ID, es solo el contenedor lógico.
		- ## Encabezado del Sitio # Bloque de Nivel 1 - Sección Header
		  section_type:: header
	- # ID sanitizado será "encabezado-del-sitio". No requiere id:: explícito.
	    logo_text:: Alma Flamenca
	- # Los enlaces de navegación pueden ser hijos con element_type:: link
		- Inicio
		  element_type:: link
		  link_url:: #la-esencia-de-alma-flamenca # Enlace a una sección por su ID
		- Música
		  element_type:: link
		  link_url:: #discografia
		- Gira
		  element_type:: link
		  link_url:: #proximos-eventos
		- Contacto
		  element_type:: link
		  link_url:: #contacta-con-alma
		- ## La Esencia de Alma Flamenca # Bloque de Nivel 1 - Sección Hero
		  section_type:: hero
	- # ID sanitizado será "la-esencia-de-alma-flamenca"
	    image_src:: img/alma-hero.webp # Imagen principal del héroe
	    image_alt:: Alma Flamenca en vivo, escenario vibrante
		- #hero_title Alma Flamenca # Este tag ayuda al parser a identificar el tipo de elemento
		  element_type:: title # H2 inferido del ##
	- # Aquí el parser debería aplicar clases de título grandes y estilos de Hero
		- El Flamenco que rompe fronteras con sonidos innovadores.
		  element_type:: paragraph # Párrafo base, que el script estilizará como subtítulo de Hero
	- # Aquí el parser debería aplicar clases de subtítulo de Hero
		- Escucha su último single
		  element_type:: button
		  link_url:: https://open.spotify.com/artist/almaflamencaXYZ # URL del botón de acción
		  link_target:: _blank
	- # Aquí el parser debería aplicar clases de botón
		- ## Sobre Alma Flamenca # Bloque de Nivel 1 - Sección de Contenido con Imagen
		  section_type:: content_block
	- # ID sanitizado será "sobre-alma-flamenca"
	    layout:: image_left # Define el layout: imagen a la izquierda, contenido a la derecha
		- Columna de Imagen # Bloque hijo para agrupar la imagen
		  column:: image # Define que este bloque y sus hijos van en la columna de imagen
			- ![Alma Flamenca - Retrato](img/alma-bio.webp) # Puedes usar sintaxis Markdown o property
	- # O con propiedad explícita:
	- # element_type:: image
	- # image_src:: img/alma-bio.webp
	- # image_alt:: Retrato del cantaor
		- Columna de Texto # Bloque hijo para agrupar el contenido de texto
		  column:: content # Define que este bloque y sus hijos van en la columna de contenido
			- ### Una Voz que Transciende
			  element_type:: title # H3 inferido del ###. Se aplica a este bloque.
			- Nacido en el corazón de Andalucía, Alma Flamenca fusiona la pasión ancestral con ritmos electrónicos y sonoridades globales.
			  element_type:: paragraph # Párrafo normal. Se aplica a este bloque.
			- Su música explora nuevas texturas manteniendo siempre la pureza del cante jondo. Ha colaborado con artistas de diversos géneros, llevando el flamenco a nuevos públicos.
			  element_type:: paragraph
		- ## Discografía Reciente # Bloque de Nivel 1 - Sección de Lista Simple
		  section_type:: list_block
		  id:: discografia # Usamos propiedad id:: porque el encabezado es diferente
		  section_title:: Álbumes y Singles Destacados # Título central para la sección
		- Álbum "Caminos Nuevos" (2024): Explorando fusiones inéditas.
		  element_type:: list_item # Este bloque es un ítem de lista
		  highlight_first_sentence:: true # Pone "Álbum 'Caminos Nuevos' (2024)" en negrita
		- Single "Ritmo del Mar" (2024): Sonido fresco y bailable.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- EP "Raíces Urbanas" (2023): Homenaje al flamenco de barrio.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Próximos Eventos
		  section_type:: list_block # Otra sección de lista
	- # ID sanitizado será "proximos-eventos". Notar que "Música" usó "discografia" y no "discografia-reciente", evitando un duplicado directo basado en el encabezado, pero si hubieran coincidido, se añadiría el sufijo.
	    section_title:: Gira 2025
		- 18 Mayo - Teatro Central, Sevilla: Entradas agotadas.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- 25 Mayo - Palau de la Música, Barcelona: Últimas entradas disponibles.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- 7 Junio - Live House, Londres, UK: ¡Primera vez en la ciudad!
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Contacta con Alma
		  section_type:: content_block # Sección simple para contacto
		  id:: contacta-con-alma # Usamos propiedad id:: para un ID más específico
		- ### Booking y Prensa
		  element_type:: title # H3
		- Para consultas profesionales, entrevistas o contrataciones, por favor contacte a través del siguiente email.
		  element_type:: paragraph
		- Enviar Email a Alma
		  element_type:: button
		  link_url:: mailto:management@almaflamenca.com
		  link_target:: _blank
		- ## Información Legal
		  section_type:: footer # Tipo de sección para el pie de página
		  id:: pie-de-pagina # ID explícito
		- © 2025 Alma Flamenca. Todos los derechos reservados. | Aviso Legal | Política de Privacidad
		  element_type:: paragraph # Contenido del footer
	- # Aquí podrías tener sub-bloques para los enlaces legales si quieres que sean clicleables