# cafe-utp-aqp
prototito en base de un proyecto de diseño basado en una problematica identificada
# Sistema de Información Multiplataforma

## Descripción del Proyecto
Este proyecto es un sistema de información multiplataforma diseñado para resolver las necesidades identificadas en la fase de investigación de usuarios. La solución emplea un enfoque API-First y está estructurada bajo los principios de Clean Architecture. Su objetivo es centralizar la lógica de negocio en un backend robusto que atiende simultáneamente y de manera escalable a un portal web y a una aplicación móvil.

## Arquitectura y Stack Tecnológico
El ecosistema de la aplicación se compone de frentes de desarrollo integrados pero totalmente desacoplados:

*   **Backend (.NET Core Web API):** Capa central que procesa las reglas de negocio, las validaciones y gestiona la seguridad mediante autenticación JWT. Expone endpoints RESTful documentados listos para su consumo.
*   **Frontend Web (Blazor):** Aplicación web que consume la API, diseñada para ofrecer una navegación fluida, gestión de estado eficiente y accesibilidad en entornos de escritorio.
*   **App Móvil (Flutter):** Aplicación nativa conectada al mismo backend, desarrollada para brindar una experiencia de usuario consistente, responsiva y optimizada para dispositivos móviles.
*   **Infraestructura y Persistencia:** El modelo de datos relacional está soportado por MariaDB. Todo el entorno de ejecución, tanto la base de datos como los servicios web, está orquestado mediante contenedores Docker para garantizar la integridad técnica desde el desarrollo hasta la producción.
