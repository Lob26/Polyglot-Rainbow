# Ruby on Rails

# Estructura

```
project-root/
|-- Gemfile
|-- Gemfile.lock
|-- config/
|   |-- database.yml
|-- app/
|   |-- controllers/
|       |-- tags_controller.rb
|   |-- models/
|       |-- tag.rb
|   |-- views/
|-- db/
|   |-- migrate/
|       |-- xxx_create_tags.rb
|-- config.ru
|-- Rakefile
```
# Modelo
```ruby
class Tag < ApplicationRecord
  # Asumiendo que ActiveRecord se usa para la interacción con la base de datos
  validates :name, presence: true, uniqueness: true
end
```
# To learn
- Ruby on Rails 
- Active record
- Migraciones de Base de Datos
- Controladores y Rutas
- Validaciones
- Vistas
- Gemas en Ruby
- Rack
