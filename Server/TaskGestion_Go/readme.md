# Estructura

```
project-root/
|-- main.go
|-- api/
|   |-- handlers.go
|   |-- routes.go
|-- db/
|   |-- models.go
|   |-- tasks.go
|-- utils/
|   |-- middleware.go
|-- go.mod
|-- go.sum
```
# Modelo
```go
use serde::{Serialize, Deserialize};
use sqlx::FromRow;

#[derive(Debug, Serialize, Deserialize, FromRow)]
pub struct User {
    pub id: i64,
    pub username: String,
    pub email: String,
    pub password_hash: String,
    pub role: String,
}
```
# To learn
- net/http
- gorilla/mux
- CRUD en DB {database/sql}
- JSON Serialization/Deserialization {encoding/json}
- Middleware
- Error management
- Trato de fechas y tiempos
