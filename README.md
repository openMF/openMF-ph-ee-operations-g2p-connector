# openMF-ph-ee-operations-g2p-connector

## Overview
`openMF-ph-ee-operations-g2p-connector` is a Spring Boot application designed to facilitate G2P (Government to Person) operations. This project uses Java and Gradle as its build tool.

## Setup

### Clone the repository
```bash
git clone https://github.com/your-repo/openMF-ph-ee-operations-g2p-connector.git
cd openMF-ph-ee-operations-g2p-connector
```

### Configure the database
Update the `src/main/resources/application.properties` file with your database configuration:
```properties
spring.datasource.url=jdbc:mysql://<your-database-url>:<port>/<database-name>
spring.datasource.username=<your-username>
spring.datasource.password=<your-password>
```

### Build the project
```bash
./gradlew build
```

### Run the project
```bash
./gradlew bootRun
```

### Usage 
The application will be accessible at `http://localhost:8084`

## API Documentation

### DFSPS API:

| Method   | URL                                                               | Description                |
|----------|-------------------------------------------------------------------|----------------------------|
| `GET`    | `/dfsp`                                                           | Retrieve all dfsps.        |
| `GET`    | `/dfsp/{id}`                                                      | Retrieve a specific dfsp . |
| `POST`   | `/dfsp`                                                           | Create a dfsp.             |
| `PUT`    | `/dfsp/{id}`                                                      | Update a specific dfsp.    |
| `DELETE` | `/dfsp/{id}`                                                      | Delete a specific dfsp.    |

### Government Entities API:
| Method   | URL                      | Description                             |
|----------|--------------------------|-----------------------------------------|
| `GET`    | `/governmentEntity`      | Retrieve all government entities.       |
| `GET`    | `/governmentEntity/{id}` | Retrieve a specific government entity . |
| `POST`   | `/governmentEntity`      | Create a government entity.             |
| `PUT`    | `/governmentEntity/{id}` | Update a specific government entity.    |
| `DELETE` | `/governmentEntity/{id}` | Delete a specific government entity.    |

### Programs API:
| Method   | URL            | Description                   |
|----------|----------------|-------------------------------|
| `GET`    | `/program`     | Retrieve all programs.        |
| `GET`    | `/program/{id}` | Retrieve a specific program . |
| `POST`   | `/program`     | Create a program.             |
| `PUT`    | `/program/{id}` | Update a specific program.    |
| `DELETE` | `/program/{id}` | Delete a specific program.    |

### G2P Payment Configuration API:
| Method   | URL | Description                             |
|----------|-----|-----------------------------------------|
| `GET`    | `/g2pPaymentConfig` | Retrieve all g2p payment configuratons. |
| `GET`    | `/g2pPaymentConfig/{id}` | Retrieve a specific g2p payment configuraton .           |
| `POST`   | `/g2pPaymentConfig` | Create a g2p payment configuraton.                       |
| `PUT`    | `/g2pPaymentConfig/{id}` | Update a specific g2p payment configuraton.              |
| `DELETE` | `/g2pPaymentConfig/{id}` | Delete a specific g2p payment configuraton.              |

### Postman Collection
 - Go to `docs` folder and import the postman collection to your postman application
