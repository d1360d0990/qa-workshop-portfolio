# Risk Matrix

| ID  |Riesgo|Impacto|Probabilidad|Nivel| Mitigación|
|-----|------|-------|------------|-----|--------------|
| R1  | El usuario no puede completar el proceso de checkout.  El checkout es la funcionalidad principal para generar ventas en el sistema.|    5    |        5     |   25    |Nivel crítico porque impacta directamente en las ventas y ocurre en un flujo complejo. Se deben realizar pruebas E2E del checkout, pruebas exploratorias del flujo completo y monitoreo en producción |
| R2  | El sistema permite ingresar cantidades extremadamente grandes en el carrito|    5    |        3     |   15    | Cantidades excesivas pueden provocar errores en cálculos de precio, inventario o procesamiento de pedidos|
| R3  | El sistema permite registrar usuarios con datos inválidos  |    3    |        5     |   15    | Datos incorrectos afectan la calidad de la base de datos y comunicación      |
| R4  | El sistema muestra productos sin stock disponible          |    3    |        3     |    9    | Puede generar frustración en los usuarios al intentar comprar un producto    |
| R5  | La aplicación presenta errores del servidor (500)          |    5    |        3     |   15    | Los errores del servidor afectan la confiabilidad del sistema                |
| R6 | El producto muestra imágenes que no corresponden al producto ofrecido | 3 | 3 | 9 | Las imágenes incorrectas pueden confundir al usuario y afectar la confianza en la tienda |