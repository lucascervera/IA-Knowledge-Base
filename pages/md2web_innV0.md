## Outline template
	- [[AI Application Company Landing Page]] # Root Block
	  title:: AI Application Company # From original <title>
	  lang:: en # From original <html> tag
		- ## Site Header # Section: Header
		  section_type:: header
		  id:: site-header
		  
		  logo_text:: innV0 # From <h1>innV0</h1>
			- Lab # Navigation link
			  element_type:: link
			  link_url:: ./innV0_logseq/published/#/page/innv0_labs # From <a> href
			  link_target:: _blank # From <a> target
		- ## Innovation Kick-off Program # Section: Hero
		  section_type:: hero
	- # ID will be "innovation-kick-off-program" (inferred and sanitized from heading)
	    image_src:: img/main.webp # From <img> src
	    image_alt:: Innovation Kick-off Program illustration # Added descriptive alt text
		- Innovation Kick-off Program # This text is the main title in the HTML Hero (H2).
		  element_type:: title # Property indicates it's a title element.
		- Structured methodology to guide you from zero to validated prototype # Paragraph in HTML Hero
		  element_type:: paragraph
		- Contact # Button text
		  element_type:: button
		  link_url:: mailto:lucas@lucascervera.com # From <a> href inside button
		  link_target:: _blank # From <a> target
		- ## Value Proposition # Section: Content Block (Image Left)
		  section_type:: content_block
	- # ID will be "value-proposition"
	    layout:: image_left # From original HTML layout (image first)
		- Image Column # Container for the image
		  column:: image
			- element_type:: image # Image element
			  image_src:: img/1.webp # From <img> src
			  image_alt:: Value Proposition Illustration # Added alt text
		- Content Column # Container for text content
		  column:: content
			- ### Value Proposition # HTML H3
			  element_type:: title # Inferred H3 from ###
			- A step-by-step innovation framework: We provide a repeatable, proven sequence of phases so you never wonder what to tackle next # Paragraph with bolded span
			  element_type:: paragraph
			  highlight_first_sentence:: true # To make the first part bold
		- ## Our Phases # Section: Timeline
		  section_type:: timeline
	- # ID will be "our-phases"
	    section_title:: Our Phases # Central title based on the main ## heading
	- # Introductory paragraph before timeline items in HTML
	- # The original HTML didn't have introductory text here, it was in Process Flow. Let's keep the Process Flow structure for Process Flow.
	- # This section is just the list of phases.
	- # Each phase item in HTML is a timeline item in Logseq
		- Identification # Title of Phase 1
		  timeline_item:: true
		  element_type:: item_title # Use item_title as defined in template
			- Systematically uncover unmet needs, market gaps, and strategic opportunities. # Description of Phase 1
			  element_type:: paragraph
		- Evaluation & Ranking # Title of Phase 2
		  timeline_item:: true
		  element_type:: item_title
			- Score ideas against real-world criteria (feasibility, impact, effort) to prioritize the most promising. # Description of Phase 2
			  element_type:: paragraph
		- Prototyping # Title of Phase 3
		  timeline_item:: true
		  element_type:: item_title
			- Build low-fidelity mock-ups that allow fast learning without heavy investment. # Description of Phase 3
			  element_type:: paragraph
		- Validation # Title of Phase 4
		  timeline_item:: true
		  element_type:: item_title
			- Test prototypes with actual users or stakeholders and collect actionable feedback. # Description of Phase 4
			  element_type:: paragraph
		- Deployment Plan # Title of Phase 5
		  timeline_item:: true
		  element_type:: item_title
			- Apply insights to enhance the solution, reduce risk, and prepare for deployment and scaling. # Description of Phase 5
			  element_type:: paragraph
		- ## Solution Structure # Section: Content Block (Image Right)
		  section_type:: content_block
	- # ID will be "solution-structure"
	    layout:: image_right # From original HTML layout (text first, then image)
		- Content Column # Container for text content (lists)
		  column:: content
			- ### Solution Structure # HTML H3
			  element_type:: title # Inferred H3 from ###
			- Modular Work Units: Self-contained building blocks you can plug into existing workflows or run as standalone sprints # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
			- Inputs: Key documents, concepts, and tools such as strategic plans, customer personas, and ideation templates # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
			- Tasks: # List item with bolded span, contains a nested list
			  element_type:: list_item
			  highlight_first_sentence:: true
	- # Nested list items
		- Autonomous exercises: Pre-recorded videos and guided worksheets for self-paced work # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item if needed by generator
		  highlight_first_sentence:: true
		- Guided workshops: Live or virtual sessions led by our innovation coaches to deepen learning and collaboration # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Outputs: Tangible deliverables like opportunity maps, idea scorecards, prototype schematics, and user-test summaries # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Image Column # Container for the image
		  column:: image
		- element_type:: image # Image element
		  image_src:: img/2.webp # From <img> src
		  image_alt:: Solution Structure Diagram # Added alt text
		- ## Our Process Flow # Section: Timeline (Modified)
		  section_type:: timeline # Using timeline type as it's sequential steps
	- # ID will be "our-process-flow"
	    section_title:: Our Process Flow # Central title from main ## heading
		- We provide minimalist educational content to ensure clients grasp concepts before activities... # Introductory paragraph before timeline items
		  element_type:: paragraph # This paragraph is a direct child of the section, before items
	- # Each step in HTML is a timeline item in Logseq
		- Self-Diagnostic (AI-Guided) # Title of Step 1
		  timeline_item:: true
		  element_type:: item_title
			- Method: Online chatbot questionnaire that assesses current innovation capabilities and mindset # Description 1 (Method) with bolded span
			  element_type:: paragraph
			  highlight_first_sentence:: true
			- Focus: Measures risk tolerance, leadership buy-in, resource allocation, failure mindset, etc., and generates a personalized report highlighting strengths and gaps # Description 2 (Focus) with bolded span
			  element_type:: paragraph
			  highlight_first_sentence:: true
		- Initial Diagnosis # Title of Step 2 (Note: HTML reverses layout for this item)
		  timeline_item:: true
		  element_type:: item_title
	- # Optional: Maybe add a property like item_layout:: reversed if the generator supports item-level layout variations in timeline
	- # item_layout:: reversed # e.g., text on right
		- Method: Facilitated discovery session where stakeholders map out existing processes, pain points, and potential quick wins # Description 1 (Method) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Deliverable: Current State & Opportunity Map – a visual chart showing high-impact areas to address first # Description 2 (Deliverable) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Idea Generation & Evaluation # Title of Step 3
		  timeline_item:: true
		  element_type:: item_title
		- Activities: Guided brainstorming (e.g., SCAMPER, How-Might-We) followed by weighted scoring of ideas # Description 1 (Activities) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Deliverable: Ranked Idea Backlog with rationale and estimated benefits for each concept # Description 2 (Deliverable) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Prototype Conceptualization # Title of Step 4 (Note: HTML reverses layout)
		  timeline_item:: true
		  element_type:: item_title
	- # item_layout:: reversed # e.g., text on right
		- Method: Rapid design sprint to sketch, decide, and storyboard key features # Description 1 (Method) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Deliverables: Low-fidelity mock-ups and user journey sketches to illustrate core experiences # Description 2 (Deliverable) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Validation & Feedback # Title of Step 5
		  timeline_item:: true
		  element_type:: item_title
		- Activities: User interviews and usability tests to capture quantitative and qualitative data # Description 1 (Activities) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Deliverable: Feedback & Insights Report with actionable recommendations on improvements, pivots, or eliminations # Description 2 (Deliverable) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Iteration & Refinement # Title of Step 6 (Note: HTML reverses layout)
		  timeline_item:: true
		  element_type:: item_title
	- # item_layout:: reversed # e.g., text on right
		- Purpose: Continuous improvement through lean cycles to refine prototypes, optimize features, and prepare for pilot launch # Description 1 (Purpose) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- Deliverable: Refined Prototype & Next Steps Plan outlining final mock-ups and a roadmap for scaling # Description 2 (Deliverable) with bolded span
		  element_type:: paragraph
		  highlight_first_sentence:: true
		- ## Integration with Best-Practice Methodologies # Section: Content Block (Image Left)
		  section_type:: content_block
	- # ID will be "integration-with-best-practice-methodologies"
	    layout:: image_left
		- Image Column # Container for the image
		  column:: image
			- element_type:: image
			  image_src:: img/3.webp # From <img> src
			  image_alt:: Integration Diagram # Added alt text
		- Content Column # Container for text content (list)
		  column:: content
			- ### Integration with Best-Practice Methodologies # HTML H3
			  element_type:: title # Inferred H3
			- 24 Steps of Disciplined Entrepreneurship: End-to-end framework for building a scalable venture from idea to launch # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
			- Lean Startup: Build–Measure–Learn cycles emphasizing quick experiments and data-driven decisions # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
			- Running Lean: Rapid hypothesis validation to align teams on assumptions, risks, and metrics # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
			- Design Thinking: Empathize → Define → Ideate → Prototype → Test for human-centered solutions # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
		- ## Key Benefits # Section: Content Block (Single Column)
		  section_type:: content_block
	- # ID will be "key-benefits"
	- # No 'layout' property implies single column, centered text styling is typical for content_block without layout.
	- # Original HTML had md:flex-row-reverse but no image, so interpreting as single column content block.
		- ### Key Benefits # HTML H3
		  element_type:: title # Inferred H3
		- Clarity: Defined path eradicates confusion and aligns teams # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Speed: Jump from zero to prototype in weeks, not months # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Risk Mitigation: Test assumptions early to reduce costly missteps # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Empowerment: Builds client capability through guided autonomy and learning # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Clients # Section: List Block
		  section_type:: list_block
	- # ID will be "clients"
	    section_title:: Clients # Central title based on main ## heading
		- Allocated innovation budget: Companies that have dedicated funding for R&D or innovation initiatives # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Desire for structured innovation: Organizations looking for a clear process to manage their innovation efforts effectively. # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Awareness of the need to innovate: Teams that recognize stagnation risks and are motivated to adopt new approaches # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- No established innovation process: Organizations lacking internal frameworks, templates, or experience to systematically innovate # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Case Example # Section: Content Block (Image Left)
		  section_type:: content_block
	- # ID will be "case-example"
	    layout:: image_left
		- Image Column # Container for the image
		  column:: image
			- element_type:: image
			  image_src:: img/4.webp # From <img> src
			  image_alt:: Case Example Illustration # Added alt text
		- Content Column # Container for text content (headings, lists)
		  column:: content
			- ### Case Example # HTML H3
			  element_type:: title # Inferred H3
			- #### Mid-Sized Event Company (40 Employees) # HTML H4
			  element_type:: title # Inferred H4
			- Profile: Overwhelmed with manual processes yet eager to innovate without derailing operations # List item with bolded span
			  element_type:: list_item
			  highlight_first_sentence:: true
			- Application Steps: # List item with bolded span, contains nested list
			  element_type:: list_item
			  highlight_first_sentence:: true
	- # Nested list items
		- AI Self-Diagnostic Chatbot identifies lack of formal process and moderate risk aversion # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Initial Diagnosis Workshop uncovers scheduling chaos and manual speaker coordination # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Idea Workshop Generates concepts like speaker-management dashboard and email automation # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Prototype Sprint Designs wireframes for dashboard and automated flow in one day # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Validation Conducts usability tests with staff and a pilot cohort of attendees, gathering NPS and task-completion data # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Iterations Refines UI elements and workflow logic; simplifies onboarding steps # Nested list item with bolded span
		  element_type:: list_item # Or nested_list_item
		  highlight_first_sentence:: true
		- Outcome: Pilot tool saves 30 % of planning time and increases on-time communications by 80 % # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- Insights: Leadership will fund full rollout after seeing pilot ROI and show openness to external tech partnerships, preferring small-scale pilots before enterprise-wide changes # List item with bolded span
		  element_type:: list_item
		  highlight_first_sentence:: true
		- ## Site Footer # Section: Footer (Manually added, wasn't a specific section in original HTML)
		  section_type:: footer
		  id:: site-footer # Explicit ID
	- # Add some placeholder footer content if needed, or leave empty if the generator template adds default footer HTML.
	- # - [Copyright Text or Links]
	- #   element_type:: paragraph
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