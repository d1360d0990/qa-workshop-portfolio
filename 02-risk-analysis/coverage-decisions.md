# Coverage Decisions

## Riesgos que se probarán primero

1. El usuario no puede completar el proceso de compra
2. El sistema permite agregar productos sin stock en el carrito
3. Errores del servidor durante acciones críticas

## ¿Por qué esos riesgos son prioridad?

Estos riesgos tienen un impacto directo en el negocio. El proceso de compra es la funcionalidad más importante del sistema, ya que es el mecanismo mediante el cual la empresa genera ingresos.

Si el checkout falla o el carrito calcula mal los pedidos, los usuarios no podrán completar compras o podrían generarse pedidos incorrectos.

Además, los errores del servidor afectan la confiabilidad general de la aplicación y pueden provocar abandono del usuario.

## Qué se probará menos o quedará fuera por ahora

- Aspectos visuales menores de la interfaz
- Optimización de performance en búsquedas
- Pruebas de compatibilidad en navegadores menos utilizados

## Justificación de exclusiones

Estas áreas tienen menor impacto inmediato en el negocio comparado con el proceso de compra y la gestión del carrito.

En una estrategia basada en riesgos, el equipo de QA prioriza primero las funcionalidades críticas para el negocio y posteriormente se enfoca en mejoras de usabilidad o rendimiento.