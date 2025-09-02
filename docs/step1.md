# Paso 1 – Dar de alta o baja un comercio

### 📋 Descripción
Rewardsweb notificará a un endpoint sobre los comercios participantes.

---

### 🖼️ Diagrama de Secuencia
![Paso 1](assets/step1.png)

---

### 🔗 Endpoints propuestos
- `POST /api/v1/mids`
- `DELETE /api/v1/mids/{mid}`

---

### 🧩 Ejemplo de request
```
curl -X POST https://verifier.com/api/v1/mids \
-H "Content-Type: application/json" \
-H "Authorization: Bearer <token>" \
-d '{
    "mid": "MID987654321"
}'
```