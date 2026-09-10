Prompt para Claude: 

<rol> Eres analista senior de mercado y producto especializado en telemedicina, marketplaces de salud y wellness digital en Latinoamérica, con 10+ años evaluando viabilidad de startups para fondos de venture capital y founders pre-seed. Tu trabajo es destilar señal de ruido: identificar gaps explotables, riesgos que matan ideas y unit economics realistas. Eres directo, no edulcoras conclusiones, prefieres "esto no funciona porque X" antes que "habría que considerar". Tienes acceso a hasta 20 subagentes paralelos para investigación profunda y dominas la creación de informes web interactivos premium (estilo McKinsey, a16z, Stripe Atlas) en HTML/CSS/JS autocontenidos. </rol> <contexto> Soy founder evaluando la viabilidad de escalar Vitalio, un marketplace de telemedicina que conecta pacientes con profesionales de salud de múltiples especialidades (nutrición, psicología, medicina general, dermatología, endocrinología, y cualquier otra que el mercado demande) en Latinoamérica. Tengo un prototipo funcional desplegado en producción (vitaliowellness.com) con videoconsultas, pagos integrados, agenda, y verificación de credenciales profesionales. El stack es React + TypeScript / Node.js + Express + Prisma + PostgreSQL, desplegado en AWS (ECS Fargate + CloudFront + RDS). 
Necesito un dictamen estilo consultora externa (5.000 €): exhaustivo, honesto, con datos verificables y veredicto claro. El informe servirá para una demo en vídeo a posibles socios, advisors e inversores — por eso debe ser una WEB INTERACTIVA navegable, no un PDF plano. Si la idea no es viable en su forma actual, prefiero saberlo ahora con datos que descubrirlo en 6 meses.
 
Mercado objetivo primario: Uruguay, Argentina, Brasil. Mercado secundario: resto de LATAM (Colombia, México, Chile, Perú). Interfaz 100 % en español (portugués como expansión futura para Brasil). Especialidades: múltiples (nutrición, psicología, medicina general, dermatología, endocrinología, ginecología, pediatría, y más según demanda). Modelo a validar: comisión por consulta (70/30 profesional/plataforma) + posible suscripción premium para profesionales. </contexto>
 <funcionalidades-vitalio> 1. ONBOARDING DUAL: registro diferenciado para pacientes y profesionales. Los profesionales suben credenciales (título, matrícula, cédula) que la plataforma verifica antes de habilitarlos. 2. BÚSQUEDA Y RESERVA: pacientes buscan profesionales por especialidad (múltiples categorías: nutrición, psicología, medicina general, dermatología, etc.), ven perfiles con disponibilidad, precios y reseñas, y reservan turno directamente. 3. VIDEOCONSULTAS EN VIVO: integración con Daily.co para consultas por video sin salir de la plataforma, con sala de espera y controles de cámara/micro. 4. PAGOS INTEGRADOS: PayPal Orders API para cobro al paciente + Payouts API (pendiente aprobación live) para liquidación al profesional. Split 70/30 automático. 5. GESTIÓN DE AGENDA: los profesionales configuran su disponibilidad semanal, los pacientes ven solo horarios disponibles en su zona horaria. 6. SISTEMA DE CRÉDITOS (en desarrollo): "saldo a favor" en USD que reemplaza reembolsos automáticos en cancelaciones/reprogramaciones. 7. AUTENTICACIÓN SEGURA: email/password + Google OAuth + LinkedIn OAuth, reCAPTCHA v3, rate limiting por IP. 
Posicionamiento tentativo: "Tu salud, sin fronteras. Conectá con profesionales de salud verificados desde cualquier lugar de LATAM." </funcionalidades-vitalio>
 <alcance-investigacion> 1. PANORAMA DEL MERCADO - TAM global de telemedicina, TAM LATAM, TAM por país (Uruguay, Argentina, Brasil, Colombia, México) con CAGR 2020-2030, fuente y año. - Segmentación: telemedicina generalista, telepsicología, telenutrición, marketplaces de salud, SaaS para profesionales de salud, wellness digital. - Tendencias 2024-2026: regulación de telemedicina por país en LATAM (marco legal Argentina Ley 27.553, Brasil Resolução CFM 2.314/2022, Uruguay decreto 118/014 y regulaciones del MSP), IA en salud mental y nutrición, penetración de medios de pago digitales en LATAM, adopción post-COVID de teleconsulta, interoperabilidad de historias clínicas, burnout de profesionales de salud, seguros de salud y cobertura de teleconsulta, EU AI Act (relevancia para expansión futura), protección de datos de salud (Ley 18.331 Uruguay, Ley 25.326 Argentina, LGPD Brasil). 

2. MAPA COMPETITIVO (mínimo 20-25 competidores analizados a fondo) Por cada uno: nombre, URL, país de origen, año de lanzamiento, usuarios/MAU si es público, funding si es público, propuesta de valor en 1 frase, features core, especialidades cubiertas (¿mono vs multi-especialidad?), pricing exacto (comisión, consulta, suscripción en USD y moneda local), canales de adquisición dominantes, 3 fortalezas, 3 debilidades, rating App Store / Play Store con nº de reviews, 1-2 QUOTES LITERALES de reviews negativas con link verificable. Cubrir obligatoriamente:
   * Marketplaces de telemedicina LATAM: Doctoranytime (Argentina), Doctoralia, Reservo, Mediké, Mi Doctor Online, Saluspot, Top Doctors, Docplanner Group, SOS Telemedicina
   * Telepsicología LATAM: Terapify, Mindy, Yana, Enterapia, Psiconlinea, BetterFly (componente wellness), Ifeelonline
   * Telenutrición: Nutrium, Nutritionist Pro, Noom (componente coaching), Fay, SimplePractice (vertical salud)
   * Teledermatología / otras especialidades: First Derm, DermatologistOnCall, Skinive, plataformas verticales mono-especialidad relevantes en LATAM
   * Plataformas globales con presencia LATAM: BetterHelp, Talkspace, Teladoc, Amwell, MDLIVE, Cerebral
   * Salud digital Brasil: Conexa Saúde, Docway, BoaConsulta, Zenklub, Vittude, Psicologia Viva
   * SaaS para profesionales: SimplePractice, Practice Better, Healthie, Jane App, Calendly (uso en salud)
   * Verticales de nutrición: Fitia (Argentina), MyRealFood (España), Nooddle/ ekilu, Avena (México)
   * Seguros/corporativo con teleconsulta: OSDE (Argentina), Sura, Emergencia/SEMM (Uruguay), Allianz Partners
3. POSICIONAMIENTO
   * Matriz 2x2 visual: precio por consulta vs amplitud de especialidades.
   * Matriz 2x2 visual: verificación de credenciales/confianza vs facilidad de uso/UX.
   * Tabla feature-by-feature (≥10 features × ≥10 competidores) con Vitalio destacado en color distinto. Features a comparar: videoconsulta integrada, pagos integrados, verificación de credenciales, multi-país, agenda configurable, reseñas de pacientes, recetas/prescripciones, historial clínico, app móvil nativa, IA/chatbot, sistema de créditos/reembolsos, soporte multi-idioma, multi-especialidad, integración con seguros, coordinación entre especialistas.
4. PRECIOS
   * Benchmark de comisiones de marketplace (% del profesional vs plataforma) en telemedicina LATAM y global.
   * Precio promedio de consulta online por especialidad y país (nutrición, psicología, medicina general, dermatología, endocrinología en UY, AR, BR, CO, MX).
   * Matriz Free vs Premium: qué ofrecen gratis vs de pago las plataformas tanto a pacientes como a profesionales.
   * LTV de paciente, CAC, ARPU, retención D1/D7/D30, tasa de rebooking, GMV por profesional activo (fuentes: Crunchbase, App Annie/data.ai, reportes de Docplanner, informes de Frost & Sullivan, IQVIA, McKinsey Digital Health).
   * Recomendación de pricing para Vitalio: comisión óptima, precio sugerido de consulta, plan premium para profesionales, pricing diferenciado por país (paridad de poder adquisitivo UY/AR/BR), trial, descuentos por paquete de consultas.
5. GAPS Y OPORTUNIDADES (la sección más importante)
   * Huecos funcionales no resueltos por nadie en telemedicina LATAM.
   * Necesidades en reviews 1-2★ y Reddit/foros (r/argentina, r/uruguay, r/brasil, r/psicologia, r/nutricion, foros de profesionales de salud LATAM).
   * Segmentos mal servidos: expatriados latinos, profesionales de salud independientes sin plataforma, pacientes en ciudades intermedias/rurales, pacientes que necesitan coordinar múltiples especialidades (ej: nutrición
      * endocrinología + psicología), usuarios de GLP-1 que necesitan seguimiento multidisciplinario.
   * Ventaja competitiva CONCRETA de Vitalio: marketplace multi-especialidad (no vertical mono-nicho), foco LATAM con pagos en USD (dollarized), verificación de credenciales multi-país, experiencia end-to-end (búsqueda → pago → videoconsulta) sin dependencia de seguros.
   * ≥5 riesgos/amenazas que pueden matar la idea con mitigaciones específicas (incluir: regulación por país, concentración en PayPal como único PSP, dependencia de Daily.co, chicken-and-egg del marketplace, tipo de cambio y volatilidad AR/BR, competencia de hospitales/mutualistas con sus propias plataformas).
6. INSIGHTS DE USUARIO
   * 10 pain points recurrentes de PACIENTES con QUOTES LITERALES y enlace verificable a review/hilo original (tanto sobre telemedicina como sobre encontrar profesionales de salud confiables online en LATAM).
   * 10 pain points recurrentes de PROFESIONALES de salud (múltiples especialidades) buscando plataforma o gestionando pacientes online.
   * 5+ hilos de Reddit/foros relevantes con link.
   * Patrones "ojalá existiera una plataforma que..." extraídos de foros.
   * Jobs-to-be-done del paciente tipo y del profesional tipo.
7. GO-TO-MARKET
   * Canales priorizados por ROI con CASOS REALES (Doctoralia, Terapify, Zenklub, Conexa, BetterHelp LATAM) y datos cuantitativos (CAC, ARR, MAU, GMV).
   * Estrategia supply-side: cómo atraer los primeros 50 profesionales verificados (múltiples especialidades, empezando por las de mayor demanda en teleconsulta) en Uruguay y Argentina.
   * Estrategia demand-side: cómo generar los primeros 200 pacientes sin quemar presupuesto.
   * Partnerships potenciales: universidades con carreras de salud (UDELAR, UBA, UTEC), colegios y asociaciones profesionales de múltiples especialidades, gimnasios/ centros de fitness, empresas con programas de bienestar corporativo, mutualistas/prepagas que no tienen teleconsulta propia, farmacias, influencers de salud/wellness LATAM.
   * Roadmap en 3 fases (MVP actual → v1 con créditos y multi-PSP → escala regional) con USD, KPIs go/no-go y entregables por fase.
   * Cold start strategy específica: ¿profesionales primero o pacientes primero? Con datos de cómo lo resolvieron otros marketplaces de salud.
8. VEREDICTO
   * Score 0-100 con desglose por ejes (tamaño de mercado, competencia, diferencial, monetización, retención, regulación, cold start/liquidez del marketplace).
   * 3 riesgos principales con mitigaciones concretas.
   * 3 next steps validables en 8 semanas con presupuesto estimado en USD.
   * Señales que deberían parar el proyecto o pivotar si aparecen.
   * Opinión directa: ¿el modelo comisión 70/30 es sostenible o Vitalio debería pivotar a SaaS para profesionales, suscripción de pacientes, o modelo híbrido? </alcance-investigacion>

 <reglas-de-investigacion> - Lanza 14-20 subagentes en paralelo distribuidos por áreas. Cada uno con dominio acotado y obligación de devolver datos VERIFICABLES con URL fuente. - Toda cifra cuantitativa debe citar fuente con URL y año. Si fuentes dan cifras distintas, reporta el rango y las fuentes en disputa. - Si un dato no se puede verificar: di "no disponible" o "estimado". NUNCA inventes números. - Para reviews: copia QUOTES LITERALES con link al review/hilo original. No parafrasees como si fueran textuales. - Verifica el estado actual de cada competidor (¿sigue activo? ¿fue adquirido? ¿pivoteó? ¿cerró?). Si no sigue activo, dilo. - Verifica el estado regulatorio actual de telemedicina en cada país objetivo. - Ante duda sobre profundidad o alcance: elige siempre la opción más exhaustiva. - Datos de LATAM son más difíciles de conseguir que US/EU — haz esfuerzo extra en fuentes locales (Crunchbase LATAM, LAVCA, Statista LATAM, informes de BID/IDB, CEPAL, ministerios de salud). </reglas-de-investigacion> <formato-salida> ARCHIVO ÚNICO: web interactiva en un solo HTML autocontenido (CSS + JS inline, salvo Chart.js / fuentes de Google vía CDN). NO PDF, NO múltiples archivos. 
UBICACIÓN CRÍTICA del archivo:
 

* Guarda el HTML en la carpeta del workspace que YO tengo conectada en Windows (típicamente algo bajo C:\Users\… que NO sea AppData\Roaming).
* Si NO tienes carpeta accesible conectada, llama a request_cowork_directory ANTES de empezar a investigar para que yo te conecte una. NO guardes en scratchpad/outputs/Roaming, NO ME LLEGA.
* Nombre del archivo: vitalio-market-research.html
* Al terminar, dame el link computer:// directo a ese path.

 
DISEÑO premium (McKinsey / a16z / Stripe Atlas):
 

* Mucho whitespace.
* Tipografía: serif para titulares (Fraunces o similar) + sans moderno para cuerpo (Inter).
* Paleta wellness/telemedicina: azul profundo (#1a365d) como primario + verde salud (#2d8a6e) como acento + fondo cálido crema (#faf7f2 o similar). Toques de coral (#e07a5f) para CTAs y alertas.
* Mobile-responsive, optimizado para desktop.
* Sidebar sticky con tabla de contenidos y sección activa resaltada vía IntersectionObserver.
* Hero inicial con resumen ejecutivo, score de viabilidad destacado y 3 insights clave.
* Dark mode toggle.
* Barra de progreso de lectura arriba.

 
INTERACTIVIDAD:
 

* Tabla de competidores filtrable por categoría (marketplace multi-especialidad / telepsicología / telenutrición / teledermatología / SaaS / global) + ordenable por cualquier columna + buscador.
* ≥4 gráficos con Chart.js: evolución TAM telemedicina LATAM, segmentación por país, distribución de precios por consulta, matriz de canales GTM, comparativa de comisiones de marketplace.
* 2 matrices 2x2 visuales (dot plot) con todos los competidores y Vitalio destacado en color distinto + tooltip al hover.
* Tarjetas de competidor click-to-expand con fortalezas/debilidades y reviews.
* Tabla feature-by-feature con marcas ●/◐/○ comparando Vitalio con 10 competidores directos.

 
CITACIONES:
 

* Apéndice numerado al final con ≥50 fuentes [1]…[n] con URL clickable.
* Cada afirmación cuantitativa enlaza a su fuente en línea.

 
BOTÓN "DESCARGAR PDF" (print-to-PDF en sidebar):
 

* @media print con: page-break-inside: avoid en cards, charts, tablas, quotes y callouts.
* Sidebar, barra de progreso y herramientas flotantes ocultas al imprimir.
* Cards expandibles se abren automáticamente al imprimir.
* Charts no se cortan a la mitad de página.
* Headers no quedan huérfanos al final de página.
* Comprueba mentalmente: ¿se imprimiría limpio en A4 sin un solo elemento partido? </formato-salida>

 <criterios-de-exito> Marca el informe como ENTREGABLE solo cuando cumpla TODAS estas condiciones: 

1. Score de viabilidad 0-100 con justificación cuantitativa y desglose por ejes (mercado, competencia, diferencial, monetización, retención, regulación, liquidez de marketplace).
2. ≥20 competidores analizados con datos verificados (no inventados).
3. ≥50 fuentes citadas en apéndice con URL funcional.
4. Tabla filtrable y ordenable sin errores JS al abrir el archivo.
5. ≥4 gráficos Chart.js renderizan correctamente.
6. Botón PDF imprime el documento limpio en A4 sin cortes en cards/charts/tablas.
7. Modo oscuro alterna correctamente.
8. ≥5 gaps de mercado accionables con argumento concreto de por qué Vitalio puede atacarlos.
9. ≥5 riesgos con mitigaciones específicas.
10. Próximos pasos de validación en 8 semanas con presupuesto estimado en USD.
11. El archivo final está en mi carpeta accesible desde Windows (NO en Roaming).
12. Test final: si un VC o advisor lee solo el hero/resumen ejecutivo, ¿tiene suficiente para decidir si seguir explorando? Si la respuesta es no, no es entregable. </criterios-de-exito>

 <ejemplos-de-tono> ESTILO CORRECTO (informe a16z/McKinsey, prosa con backbone, opinión clara): 
"Doctoralia domina discovery en LATAM con 2M+ profesionales listados y SEO orgánico brutal. Pero es un directorio con booking, no un marketplace con videoconsulta integrada ni pagos. El paciente agenda en Doctoralia y después se las arregla solo. La pregunta para Vitalio no es 'cómo competir contra Doctoralia en volumen de listings' sino 'qué experiencia end-to-end puede ofrecer que Doctoralia no': videoconsulta sin salir de la plataforma, pago integrado con split automático, verificación real de credenciales multi-país, y la posibilidad de que un paciente coordine múltiples especialidades en una sola plataforma son ese terreno."
 
"Retención D30 en marketplaces de telemedicina: 8-15 % (mediana, data.ai 2025 [13]). Si Vitalio no consigue ≥20 % apoyado en el rebooking natural de especialidades recurrentes (psicología semanal/quincenal, nutrición mensual, control endocrinológico trimestral), la unit economics no cierra y el marketplace se vacía. La ventaja multi-especialidad es exactamente esa: más puntos de contacto recurrentes por paciente."
 
ESTILO INCORRECTO (genérico, sin opinión, fluff de consultora junior):
 
"Doctoralia tiene buenas funcionalidades. Es importante considerar la competencia. Vitalio podría diferenciarse en varios aspectos."
 
"La retención es un factor importante en apps de telemedicina y Vitalio debería trabajar en mejorarla."
 
REGLA: cada afirmación o tiene datos detrás, o tiene una opinión defendible. Si no tiene ni una cosa ni la otra, fuera del informe. </ejemplos-de-tono>
 <plan-de-trabajo> ANTES de empezar a investigar, comunícame en 2-3 frases: 1. Cuántos subagentes vas a lanzar y cómo los repartes temáticamente. 2. Si necesitas que conecte una carpeta de Windows accesible (llama a request_cowork_directory si no la tienes). 
Después ejecuta SIN pedir más confirmaciones. Voy a desconectar durante 60-90 minutos. Cuando vuelva quiero:
 

* El archivo vitalio-market-research.html en mi carpeta accesible.
* Un link computer:// directo en tu mensaje final.
* Un resumen de 5-7 líneas con el score, los 3 hallazgos clave y los 3 next steps. </plan-de-trabajo>

 
Lanza la investigación, sintetiza los hallazgos en el informe HTML interactivo y entrégamelo siguiendo todos los criterios de éxito. Si en cualquier punto debes elegir entre rápido y exhaustivo, elige exhaustivo — prefiero esperar 90 minutos a un informe impecable que recibir en 30 minutos algo que tenga que pedirte rehacer.
