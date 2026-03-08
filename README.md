
<div class="container">
    <h1>🤖 Agente de IA para E-commerce: Komiland</h1>
    <p>Este proyecto implementa un sistema de atención al cliente automatizado utilizando inteligencia artificial soberana y flujos de trabajo avanzados.</p>

<img width="1452" height="680" alt="image" src="https://github.com/user-attachments/assets/1aab7cf1-878a-4c1e-ac0c-15259a712447" />


  <h2>Arquitectura del Sistema</h2>
    <p>El flujo ha sido diseñado en <strong>n8n</strong> e integra los siguientes componentes:</p>
    <ul>
        <li><strong>Orquestador:</strong> n8n (Self-hosted).</li>
        <li><strong>Modelo de Lenguaje:</strong> Ollama ejecutando <code>llama3.2:latest</code> de forma local.</li>
        <li><strong>Memoria de Chat:</strong> Persistencia de mensajes en una base de datos <strong>PostgreSQL</strong>.</li>
        <li><strong>Interfaz:</strong> Webhook configurado para recibir peticiones POST y devolver respuestas en tiempo real.</li>
    </ul>

  <h2>Funcionalidades</h2>
    <ul>
        <li><strong>Gestión de Contexto:</strong> El agente utiliza un nodo de consulta SQL para recuperar el historial de mensajes de PostgreSQL antes de responder.</li>
        <li><strong>Lógica Agéntica:</strong> Capacidad para razonar sobre el catálogo de productos (tortillas, paellas, croquetas) y ofrecer recomendaciones personalizadas.</li>
        <li><strong>Seguridad:</strong> Procesamiento local mediante Ollama, evitando el envío de datos a APIs externas.</li>
    </ul>

  <h2>Instalación</h2>
    <ol>
        <li>Clona este repositorio.</li>
        <li>Asegúrate de tener levantado el entorno de https://github.com/n8n-io/self-hosted-ai-starter-kit.</li>
        <li>Importa el archivo <code>n8n-komiland.json</code> en tu instancia de n8n.</li>
        <li>Configura las credenciales de <strong>PostgreSQL</strong> y la URL de <strong>Ollama</strong> (<code>http://host.docker.internal:11434</code>).</li>
    </ol>

</div>
