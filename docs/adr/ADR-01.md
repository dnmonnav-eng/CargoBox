ADR-01, registro, cotización y creación del envío
Campo	Contenido
Título	Registro, cotización y creación del envío
Estado	Aceptado
Contexto	Se requiere un mecanismo centralizado para procesar solicitudes de envío, validar datos, calcular tarifas según peso y dimensiones, procesar pagos y generar una guía única sin inconsistencias.
Alternativas	1. Transaction Script. 2. Table Module. 3. Domain Model (elegida).
Decisión	Adoptar Domain Model respaldado por una Capa de Aplicación, donde la clase principal y el agregado gestionan validaciones, tarifas y confirmación de pago antes de emitir la guía.
Consecuencias	Beneficios: alta cohesión y transparencia de costos. Riesgos: mayor curva de aprendizaje inicial.
Trazabilidad	CU-01, reglas de validación y cotización, Diagrama de Secuencia 1.
