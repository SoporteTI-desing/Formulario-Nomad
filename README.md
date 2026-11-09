# Formulario Nomad

Abre `index.html` para el formulario de ingreso de venta. El botón **Quiero solicitar una prueba** abre `solicitud-prueba.html`, un formulario independiente para pacientes, familiares y profesionales de la salud.

Las solicitudes se guardan en la colección `ingresosNomad` de Firestore con `tipoRegistro: solicitudPruebaGenomica`. El panel de `base.html` las muestra con el estado **SOLICITUD RECIBIDA**. La exportación del formulario completo incluye sus respuestas.

Para usar el envío, se necesita conexión a Internet y acceso de escritura a la colección configurada en Firebase. La página informa si el guardado falla y conserva las respuestas para que se pueda reintentar.
