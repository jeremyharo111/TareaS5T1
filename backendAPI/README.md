# Backend API - Productos

## Variables de Entorno (.env)

```
DB_CONNECTION_STRING="Server=TU_SERVIDOR;Database=BDCRUD;Trusted_Connection=True;TrustServerCertificate=True;"
```

## Endpoints

### 1. Obtener todos los productos

`GET` `http://localhost:5000/api/Productos`

### 2. Obtener un producto por ID

`GET` `http://localhost:5000/api/Productos/{id}`

### 3. Crear un nuevo producto

`POST` `http://localhost:5000/api/Productos`

```json
{
  "nombre": "Arroz Extra 1kg",
  "descripcion": "Arroz blanco de grano largo",
  "precio": 1.5,
  "stock": 100,
  "categoria": "Abarrotes",
  "descontinuado": false
}
```

### 4. Actualizar un producto existente

`PUT` `http://localhost:5000/api/Productos/{id}`

```json
{
  "id": 1,
  "nombre": "Arroz Extra 1kg (Oferta)",
  "descripcion": "Arroz blanco de grano largo - Promoción",
  "precio": 1.25,
  "stock": 90,
  "categoria": "Abarrotes",
  "descontinuado": false,
  "fechaCreacion": "2024-02-17T10:00:00Z"
}
```

### 5. Descontinuar un producto

`DELETE` `http://localhost:5000/api/Productos/{id}`
