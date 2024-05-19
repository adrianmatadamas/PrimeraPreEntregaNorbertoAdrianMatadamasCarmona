# PrimeraPreEntregaNorbertoAdrianMatadamasCarmona
Primera pre entrega backend 1

Explicación Detallada

    Estructura y configuración del proyecto:
        Se creó la estructura del proyecto y se instalaron las dependencias necesarias.
        app.js configura el servidor de Express y define las rutas para productos y carritos.

    Rutas de Productos (routes/products.js):
        GET /api/products: Lista todos los productos, con una opción de límite.
        GET /api/products/:pid: Obtiene un producto por su ID.
        POST /api/products: Añade un nuevo producto. El ID se autogenera.
        PUT /api/products/:pid: Actualiza un producto existente sin cambiar su ID.
        DELETE /api/products/:pid: Elimina un producto por su ID.

    Rutas de Carritos (routes/carts.js):
        POST /api/carts: Crea un nuevo carrito con un ID autogenerado.
        GET /api/carts/:cid: Lista los productos de un carrito específico.
        POST /api/carts/:cid/product/:pid: Añade un producto a un carrito, incrementando la cantidad si ya existe.

    Persistencia de datos:
        Se utilizan archivos JSON (products.json y carts.json) para almacenar la información de productos y carritos respectivamente.
        Se implementan funciones auxiliares para leer y escribir en estos archivos.
