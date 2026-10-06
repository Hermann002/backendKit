**Hello BackendKit**
Honnetement je ne sais pas ce que je suis en train de vouloir développer, encore un projet que je vais commencer sans terminer ?

V1 — objectif de livraison
À la fin, un développeur doit pouvoir faire :
```bash
git clone ...
cp .env.example .env
# configurer PostgreSQL + Redis
docker compose up -d
```
Puis :
```bash
pip install backendkit
```

et dans son application :
```python
from backendkit import BackendKit
client = BackendKit(
    base_url="http://localhost:8080",
    api_key="...")
user = client.auth.create_user(...)
```
