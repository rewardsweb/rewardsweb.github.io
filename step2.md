# Paso 2 – Dar de alta o baja una tarjeta

### 📋 Descripción
Rewardsweb enviará a un endpoint la lista de PAN enrolados en la plataforma, junto con su token interno asociado.

---

### 🔗 Endpoints propuestos
- `POST /api/v1/cards`
- `DELETE /api/v1/cards/{card_id}`

---

### 🧩 Ejemplo de request
```http
curl -X POST https://verifier.com/api/v1/cards \
  -H "Content-Type: application/json" \
  -H "Authorization: Bearer <token>" \
  -H "Idempotency-Key: 7b4e6d9a-2e3a-4b53-9f9c-1a2b3c4d5e6f" \
  -d '{
    "card_id": "CARDID1",
    "pan": "4111111111111111"
  }'