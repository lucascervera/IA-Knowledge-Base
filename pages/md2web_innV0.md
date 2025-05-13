## Outline template
	- [[Your Website Name]] # Root Block: The page title in Logseq and the base name for the generator.
	  title:: [Title that will appear in the browser tab] # Property for the HTML <title>.
	  lang:: en # Property for the HTML <html> lang attribute. Use 'es', 'fr', etc., depending on your content.
	- # This Level 0 block does NOT directly generate an HTML section; it is the logical container.
	- # --- MAIN SECTIONS (Level 1 Blocks) ---
	- # Each Level 1 block (direct child of the root block) generates a <section> in the HTML.
	- # Each section will have an ID automatically generated from the heading or the 'id::' property.
		- ## Site Header # Level 1 Block: Section for the page header/navigation bar.
		  section_type:: header # REQUIRED property to define the section type.
	- # Sanitized ID: "site-header" (inferred from the ## heading)
	- # You can use id:: [manual-name] if you don't want the ID generated from the heading.
	  
	    logo_text:: [Your Brand or Name] # Text that will appear as the logo/title in the header.
	- # Navigation links usually go as children of this section.
		- Home # A navigation link
		  element_type:: link # Property to generate an <a> tag.
		  link_url:: #main-section # Link to a section by its ID (e.g., the sanitized ID of the Hero section).
		- [Section Name 1] # Another navigation link
		  element_type:: link
		  link_url:: #[sanitized-id-section1] # Make sure #[...] matches the ID of the target section.
		- [Section Name 2] # Another link
		  element_type:: link
		  link_url:: #[sanitized-id-section2]
	- # For external links that open in a new tab:
	- # - Blog or News
	- #   element_type:: link
	- #   link_url:: https://your-blog.com # Full URL
	- #   link_target:: _blank # Property to open in a new tab.
		- ## Main Section (Hero) # Level 1 Block: The prominent section (right after the header).
		  section_type:: hero # REQUIRED property.
	- # Sanitized ID: "main-section-hero" (inferred from the ## heading)
	  
	    image_src:: img/[your-hero-image-name].webp # Property for the main Hero image.
	    image_alt:: [Short description of the image for accessibility] # Property for the image alt attribute.
	- # Hero content (main title, subtitle, call-to-action button) goes as child blocks.
		- [Large, Catchy Hero Title] # This block will be the main title of the Hero.
	- # You do NOT need a ## here if you use element_type:: title and section_type:: hero.
	- # The generator already knows it's the main title and will apply the correct H2/styling.
	      element_type:: title # Property to indicate this block is a content title.
		- [Catchy subtitle or slogan describing your offer.]
		  element_type:: paragraph # Property to indicate this block is a paragraph.
	- # The generator will apply Hero subtitle classes to paragraphs under a Hero section.
		- [Call to Action Button Text] # Block for the main button.
		  element_type:: button # Property to generate a button.
		  link_url:: [Button destination URL] # E.g., mailto:your.email@example.com or https://wa.me/... or #[contact-section-id]
		  link_target:: _blank # Optional: opens the link in a new tab.
		- ## Content Block with Image # Level 1 Block: Section to display content (text/lists) next to an image.
		  section_type:: content_block # REQUIRED property.
	- # Sanitized ID: "content-block-with-image"
	  
	    layout:: image_left # REQUIRED property for this section type: 'image_left' or 'image_right'.
	- # This tells the generator to split this section into two visual columns on medium+ screens.
	- # Direct children of this section WITH THE 'column::' property will define the content of each column.
		- Content Column # Container block for the text column.
		  column:: content # REQUIRED property if the parent has layout:: image_...
	- # Child blocks nested here will go inside the text column.
		- ### [Title within the Content Block] # Markdown Heading: Will generate an <h3> (due to ###).
		  element_type:: title # Property to indicate it's a title. DO NOT use level::; it's inferred from Markdown.
		- [Introductory or main paragraph for this section. Describe your service, product, story, etc.]
		  element_type:: paragraph # Property to indicate it's a paragraph.
		- [Another paragraph if needed.]
		  element_type:: paragraph
	- # You can add lists here
	- # - List Item 1: Description of the first point.
	- #   element_type:: list_item # Property for a list item (<li>).
	- #   highlight_first_sentence:: true # Optional: Bolds the part before the ':' or the beginning.
	- # - List Item 2.
	- #   element_type:: list_item
		- Image Content Column # Container block for the image column.
		  column:: image # REQUIRED property if the parent has layout:: image_...
	- # The child block nested here SHOULD be the image.
		- element_type:: image # Property to generate an <img> tag.
		  image_src:: img/[your-content-image-name].webp # URL of the image for this column.
		  image_alt:: [Description of the content image for accessibility]
	- # Alternatively, if your Logseq parser allows, you could use Markdown image syntax directly under 'column:: image':
	- # - ![Description of the image](img/[your-content-image-name].webp)
	- #   # element_type:: image (May not be needed if using Markdown syntax and parser is smart)
	- #   # image_src:: img/[your-content-image-name].webp (May not be needed if using Markdown syntax)
	- #   # image_alt:: [Description of the image] (May not be needed if using Markdown syntax)
		- ## Simple List Section # Level 1 Block: To present a list of items (e.g., features, services, agenda).
		  section_type:: list_block # REQUIRED property.
	- # Sanitized ID: "simple-list-section".
	  
	    section_title:: [Central Title for the List] # Optional property for a centered title above the list.
	- # Direct children of this section will be the main list items (<li>).
		- First item in your list: Description of the item.
		  element_type:: list_item # REQUIRED property for each item.
		  highlight_first_sentence:: true # Optional: Bolds the part before ':' or the beginning.
		- Second item in your list: Another relevant description.
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Third simple item.
		  element_type:: list_item # This one doesn't have highlight:: to show the difference.
	- # You can nest content under a list item if you need details or sub-points.
	- # - Item with Sub-points:
	- #   element_type:: list_item
	- #   - Sub-point A. # This will be nested as another list (<ul>) inside the parent item.
	- #     element_type:: nested_list_item # Or simply list_item if the parser handles it.
	- #   - Sub-point B.
	- #     element_type:: nested_list_item
		- ## Timeline Section # Level 1 Block: For sequential steps or events (e.g., process, history).
		  section_type:: timeline # REQUIRED property.
	- # Sanitized ID: "timeline-section"
	  
	    section_title:: [Main Title for the Timeline] # Optional central title.
	- # Each direct child of this section is a step or event in the timeline.
		- [Title of Step 1] # This block is the title of a timeline item.
		  timeline_item:: true # REQUIRED property to mark a block as a timeline item.
		  element_type:: item_title # Property to indicate this block is the item's title.
			- [Detailed description of Step 1.] # Child block with the step's description.
			  element_type:: paragraph # Property to indicate it's a paragraph.
		- [Title of Step 2]
		  timeline_item:: true
		  element_type:: item_title
			- [Detailed description of Step 2.]
			  element_type:: paragraph
	- # ... Repeat the structure (Step Title -> timeline_item + item_title, with Description -> paragraph as child) for each step.
		- ## Footer Section # Level 1 Block: Section for the footer.
		  section_type:: footer # REQUIRED property.
		  id:: site-footer # Explicit 'id::' property recommended for the footer for a fixed ID.
			- [Copyright text, basic contact info, legal links, etc.]
			  element_type:: paragraph # Property to indicate it's a paragraph.
	- # You can add legal or social media links as children:
	- # - Legal Notice
	- #   element_type:: link
	- #   link_url:: /legal-notice.html
	- # - Instagram Link
	- #   element_type:: link
	- #   link_url:: https://instagram.com/yourprofile
	- #   link_target:: _blank
	- # --- GENERAL INSTRUCTIONS ---
	- # - Fill in the "[...]" placeholders with your actual content.
	- # - Properties are written as property:: value.
	- # - The generator will infer the HTML heading level (H1, H2, etc.) ONLY from the # symbols at the start of the block (## -> H2, ### -> H3). DO NOT use the level:: property.
	- # - Section IDs are automatically generated from the heading or the id:: property, sanitized (lowercase, spaces to -, removes special chars) and made unique by adding a suffix (-2, -3) if duplicates occur.
	- # - Styling (colors, fonts, spacing) is handled by the generator applying predefined Tailwind classes based on the section_type, element_type, etc. You do NOT need (or want) to add Tailwind classes in this file.
	- # - Export this outline as a Markdown (.md) file from Logseq and use it as input for your generator script.
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