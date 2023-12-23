# Estructura

```
project-root/
|-- src/
|   |-- main.rs
|   |-- lib.rs
|   |-- api/
|       |-- mod.rs
|       |-- routes.rs
|   |-- db/
|       |-- mod.rs
|       |-- models.rs
|       |-- migrations/
|   |-- auth/
|       |-- mod.rs
|       |-- middleware.rs
|   |-- models/
|       |-- user.rs
|-- Cargo.toml

```
# Modelo
```rust
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
- Actix Framework
- SQLx
- Seguridad {Almacenamiento seguro, hashing, middleware de auth y auto}
- Serde
- Middleware
