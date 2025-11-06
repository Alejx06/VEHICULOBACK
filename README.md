🚀 Sistema de Gestión de Vehículos – Backend

Este proyecto corresponde al backend del sistema de gestión de vehículos, encargado de administrar los datos y operaciones principales del sistema.
Está desarrollado con Spring Boot y sigue una arquitectura limpia, enfocada en mantener el código modular, fácil de mantener y escalable.

El sistema permite registrar, actualizar, eliminar y consultar información de vehículos, conectándose a una base de datos y ofreciendo los servicios mediante API REST.

👨‍💻 Autor

Alejandro Benítez

📎 Repositorio del proyecto

Backend del sistema de gestión de vehículos desarrollado en Spring Boot.

⚙️ Tecnologías utilizadas

Tipo	Tecnología

Lenguaje principal	Java 

Framework	Spring Boot

Dependencias principales	Spring Web, Spring Data JPA, Lombok

Control de versiones	Git + GitHub

📁 Estructura del proyecto

Lenguajes-de-programacion-backend/
├── src/

│   ├── main/

│   │   ├── java/com/vehiculos/

│   │   │   ├── controller/   # Controladores REST (VehiculoController)

│   │   │   ├── model/        # Clases de entidad (Vehiculo.java)

│   │   │   ├── repository/   # Interfaces JPA (VehiculoRepository)

│   │   │   ├── service/      # Lógica de negocio

│   │   │   └── VehiculosApplication.java

│   │   └── resources/

│   │       ├── application.properties  # Configuración de la app

│   │       └── data.sql / schema.sql   # Datos o estructura inicial (opcional)

│   └── test/                           # Pruebas unitarias

├── pom.xml                             # Dependencias Maven

└── README.md

🧠 Descripción general

El backend se encarga de toda la lógica de negocio y de la comunicación con la base de datos.
Ofrece una API que puede ser consumida por el frontend (por ejemplo, el desarrollado en React con Vite).

Funcionalidades principales

Registrar nuevos vehículos.

Consultar todos los vehículos registrados.

Buscar vehículo por su ID o características.

Actualizar información existente.

Eliminar registros de vehículos.

🧩 Endpoints principales
Método	Endpoint	Descripción

GET	/api/vehiculos	Lista todos los vehículos.

GET	/api/vehiculos/{id}	Obtiene un vehículo por su ID.

POST	/api/vehiculos	Registra un nuevo vehículo.

PUT	/api/vehiculos/{id}	Actualiza los datos de un vehículo existente.

DELETE	/api/vehiculos/{id}	Elimina un vehículo.

📸 Evidencias del funcionamiento

CREAR UN VEHICULO
<img width="1380" height="809" alt="Captura de pantalla 2025-11-06 171957" src="https://github.com/user-attachments/assets/b1b6dfc4-b221-4812-bfa4-b08ab808ba40" />

OBTENER TODOS LOS VEHICULOS 
<img width="1366" height="914" alt="Captura de pantalla 2025-11-06 172151" src="https://github.com/user-attachments/assets/4d2ba9b6-1475-4963-9090-3b6acb6d982c" />

OBTENER POR ID A UN VEHICULO
<img width="1374" height="862" alt="Captura de pantalla 2025-11-06 172705" src="https://github.com/user-attachments/assets/987c4855-c859-4327-bddc-4efc9ded76de" />

EDITAR UN VEHICULO
<img width="1379" height="861" alt="Captura de pantalla 2025-11-06 172802" src="https://github.com/user-attachments/assets/0b5c6764-1f52-46c6-81dc-3258b2894702" />

ELIMINAR UN VEHICULO
<img width="1375" height="867" alt="Captura de pantalla 2025-11-06 172833" src="https://github.com/user-attachments/assets/3bba5ebe-b660-4e48-9f44-09c158de8c82" />

CREAR UNA MOTO 
<img width="1380" height="873" alt="Captura de pantalla 2025-11-06 172435" src="https://github.com/user-attachments/assets/068cfdd1-3174-4049-8df1-4bf8f76d5fca" />

OBTENER TODAS LAS MOTOS 
<img width="1375" height="860" alt="Captura de pantalla 2025-11-06 172524" src="https://github.com/user-attachments/assets/690f10ed-8971-4e0e-9801-e1cd93fcec84" />

OBTENER POR ID UNA MOTO
<img width="1377" height="865" alt="Captura de pantalla 2025-11-06 172854" src="https://github.com/user-attachments/assets/ba6de953-7e70-4c7b-8288-8dab7510657b" />

EDITAR UNA MOTO
<img width="1385" height="859" alt="Captura de pantalla 2025-11-06 172939" src="https://github.com/user-attachments/assets/1e2ec7f8-a1a4-4136-b748-d8844fc026d3" />

ELIMINAR UNA MOTO
<img width="1364" height="867" alt="Captura de pantalla 2025-11-06 173006" src="https://github.com/user-attachments/assets/4cb332bc-0ce5-45e3-9acd-d2ecdd304e78" />



🧩 Arquitectura general

El sistema sigue una arquitectura en capas, bien organizada:

Controller: recibe las solicitudes HTTP y las envía al servicio correspondiente.

Service: contiene la lógica de negocio (validaciones, procesos, etc.).

Repository: interactúa directamente con la base de datos usando JPA.

Model: define las entidades (tablas del sistema).
