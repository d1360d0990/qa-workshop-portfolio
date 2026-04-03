# Sesión 1

## Charter  
Explorar el flujo completo de compra para detectar problemas en validación de datos, cálculo de precios y confirmación de pedidos.

## ÁREAS
Catálogo de productos, carrito de compras, proceso de registro/login, checkout y confirmación de orden.

## INICIO  
01/04/2026 - 09:00 hs

## TESTER  
Diego Díaz

## DESGLOSE DE TAREAS  
- 10 min: Navegación por categorías y selección de productos  
- 10 min: Pruebas en carrito (agregar, eliminar, modificar cantidades)  
- 15 min: Intento de checkout con usuario nuevo  
- 10 min: Pruebas con datos inválidos y casos límite  

## ARCHIVOS DE DATOS  
- Usuario nuevo (registro)  
- Datos de pago simulados  
- Inputs inválidos (campos vacíos, caracteres especiales, cantidades altas)

## NOTAS DE PRUEBA  
- El sistema permite navegar correctamente por las categorías y visualizar productos.  
- El agregado de productos al carrito funciona correctamente.  
- El sistema no permite ingresar cantidades negativas (validación correcta).  
- Se detecta que el sistema permite ingresar cantidades muy grandes sin restricción aparente.  
- No se observan validaciones claras de límites máximos en cantidades.  
- Durante el proceso de registro (necesario para comprar), el sistema devuelve un error 500, impidiendo continuar con el flujo de compra.  
- Debido a este error, no fue posible completar el proceso de checkout.  

## LISTA DE RIESGOS  
- Riesgo de indisponibilidad del sistema en funcionalidades críticas (registro/checkout).  
- Riesgo de pérdida de ventas debido a fallos en el proceso de compra.  
- Riesgo de sobrecarga o inconsistencias en pedidos por falta de límites en cantidades.  
- Riesgo de mala experiencia de usuario debido a errores no controlados (error 500).  

## DEFECTOS (BUGS)  
- BUG 1: El sistema retorna error 500 durante el registro de usuario, bloqueando el proceso de compra.  
- BUG 2: No existe un límite máximo visible al ingresar cantidades en el carrito.  
- BUG 3: Se observan productos con imágenes incorrectas o no representativas.  
- BUG 4: Se listan productos sin indicar claramente su disponibilidad de stock.  

## INCIDENTES (ISSUES)  
- No está claro si el error 500 es un problema temporal del servidor o un fallo funcional persistente.  
- No se especifican reglas de negocio sobre límites de compra por producto.  
- No hay claridad sobre cómo se maneja el stock en la interfaz de usuario.