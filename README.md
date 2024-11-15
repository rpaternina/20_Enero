<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
</head>
<body>
    <header>
        <h1>Proyecto Gestión de Estudiantes y Cursos</h1>
        <p><strong>Desarrollado por:</strong> Robert Paternina</p>
        <p><strong>Correo Electrónico:</strong> <a href="mailto:paterninayolir@gmail.com">paterninayolir@gmail.com</a></p>
        <p><strong>LinkedIn:</strong> <a href="https://www.linkedin.com/in/robert-paternina/" target="_blank">https://www.linkedin.com/in/robert-paternina/</a></p>
        <p><strong>Institución:</strong> Colegio 20 de Enero - Sincelejo, Sucre, Colombia</p>
    </header>
    <section>
        <h2>Descripción del Proyecto</h2>
        <p>Este proyecto tiene como objetivo la creación de un sistema de gestión de estudiantes y cursos utilizando la arquitectura de microservicios. Los estudiantes y los cursos estarán gestionados mediante microservicios independientes, facilitando la escalabilidad, mantenimiento y futuras integraciones.</p>
        <p>El sistema estará basado en los siguientes componentes clave:</p>
        <ul>
            <li><strong>API Gateway:</strong> Puerta de entrada a los microservicios, gestionando el enrutamiento de las peticiones.</li>
            <li><strong>Spring Eureka Server:</strong> Para la localización y descubrimiento de microservicios.</li>
            <li><strong>Spring Config Server:</strong> Para la configuración centralizada de los microservicios.</li>
            <li><strong>Spring Boot 3.3.5:</strong> Framework utilizado para desarrollar los microservicios.</li>
            <li><strong>Java 17:</strong> Versión de Java utilizada para el desarrollo del proyecto.</li>
            <li><strong>Docker:</strong> Utilización de contenedores Docker para las bases de datos PostgreSQL (para estudiantes) y MySQL (para cursos).</li>
            <li><strong>Microservicios Modulares:</strong> Arquitectura modular para una fácil gestión y escalabilidad de los microservicios.</li>
        </ul>
    </section>
    <section>
        <h2>Arquitectura</h2>
        <p>El sistema está compuesto por varios microservicios, que incluyen:</p>
        <ul>
            <li><strong>Microservicio de Estudiantes:</strong> Gestiona la información de los estudiantes. Utiliza una base de datos PostgreSQL, alojada en un contenedor Docker.</li>
            <li><strong>Microservicio de Cursos:</strong> Gestiona la información sobre los cursos disponibles. Utiliza una base de datos MySQL, alojada también en un contenedor Docker.</li>
            <li><strong>API Gateway:</strong> Unifica las peticiones y las distribuye a los microservicios correspondientes. Actúa como puerta de entrada para la plataforma.</li>
            <li><strong>Eureka Server:</strong> Permite la localización y el descubrimiento de servicios dentro de la arquitectura de microservicios.</li>
            <li><strong>Config Server:</strong> Centraliza la configuración de todos los microservicios, permitiendo su gestión de manera centralizada.</li>
        </ul>
        <p>La comunicación entre los microservicios será gestionada a través de un protocolo REST, y el API Gateway se encargará de enrutarlas correctamente.</p>
    </section>
    <section>
        <h2>Requisitos Técnicos</h2>
        <ul>
            <li><strong>Java:</strong> 17</li>
            <li><strong>Spring Boot:</strong> 3.3.5</li>
            <li><strong>Docker:</strong> Para contenedores de bases de datos PostgreSQL y MySQL.</li>
            <li><strong>Base de Datos:</strong> PostgreSQL para el microservicio de estudiantes y MySQL para el microservicio de cursos.</li>
            <li><strong>Spring Eureka Server:</strong> Para la localización de microservicios.</li>
            <li><strong>Spring Config Server:</strong> Para la gestión centralizada de la configuración de los microservicios.</li>
        </ul>
    </section>
    <section>
        <h2>Cómo Ejecutar el Proyecto</h2>
        <p>Para ejecutar el proyecto, siga los siguientes pasos:</p>
        <ol>
            <li><strong>Clonar el repositorio:</strong> Descargue el repositorio del proyecto desde GitHub (u otro servicio de repositorios).</li>
            <li><strong>Construir los contenedores Docker:</strong> Use los comandos <code>docker-compose up</code> para iniciar los contenedores de bases de datos.</li>
            <li><strong>Ejecutar los microservicios:</strong> Puede ejecutar cada microservicio de manera independiente usando Spring Boot. Asegúrese de tener las configuraciones correctas de la base de datos y las URLs de Eureka y Config Server.</li>
            <li><strong>Iniciar API Gateway:</strong> El API Gateway debe ser configurado para enrutar las peticiones a los microservicios de estudiantes y cursos.</li>
            <li><strong>Probar el sistema:</strong> Puede acceder a los microservicios a través de la API Gateway y verificar su funcionamiento.</li>
        </ol>
    </section>
    <section>
        <h2>Contribuciones</h2>
        <p>Este es un proyecto personal, pero si deseas contribuir, puedes enviar pull requests para mejorar la arquitectura, la documentación o agregar nuevas funcionalidades.</p>
    </section>
    <section>
        <h2>Licencia</h2>
        <p>Este proyecto se distribuye bajo la licencia MIT. Puedes usar, modificar y distribuir el código conforme a los términos de la licencia.</p>
    </section>
</body>
</html>
