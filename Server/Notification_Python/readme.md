# Flask

# Estructura

```
project-root/
|-- app/
|   |-- __init__.py
|   |-- api/
|       |-- __init__.py
|       |-- notifications.py
|   |-- tasks/
|       |-- __init__.py
|       |-- send_notification.py
|-- config/
|   |-- __init__.py
|   |-- settings.py
|-- migrations/
|   |-- __init__.py
|   |-- versions/
|-- requirements.txt
|-- celery_worker.py
|-- run.py
```
# Modelo
```python
# OPCIONAL
from datetime import datetime
from sqlalchemy import Column, Integer, String, DateTime
from sqlalchemy.ext.declarative import declarative_base

Base = declarative_base()

class Notification(Base):
    __tablename__ = 'notifications'
    
    id = Column(Integer, primary_key=True)
    recipient = Column(String)
    message = Column(String)
    timestamp = Column(DateTime, default=datetime.utcnow)

# ... Puedes agregar más campos según sea necesario

```
# To learn
- Flask
- Celery
- API RESTful
- Configuracion de Aplicacion
- Manejo de Tareas Asincronas
- Trabajadores Celery
- OPCIONAL Almacenamiento de datos
- Manejo de Fechas y Horas
