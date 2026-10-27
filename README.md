# AMS-PRE-Salazar - Sistema de Gestión de Pedidos en Línea

## 1. Introducción y Objetivo
Sistema centralizado de gestión de pedidos en línea orientado a optimizar la relación comercial entre usuarios y el catálogo de productos disponibles.
- **Plazo de implementación:** Máximo 8 semanas.
- **Integridad de datos:** 100% de integridad referencial entre `users`, `products` y `orders`.
- **Rendimiento:** Tiempo de respuesta en creación de pedidos inferior a 2 segundos.

## 2. Alcance y Módulos
- **Módulo de Usuarios (`users`):** Registro, consulta (`id`, `name`, `email`) y validación de credenciales.
- **Módulo de Productos (`products`):** Visualización y consulta de catálogo activo (`id`, `name`, `price`).
- **Módulo de Pedidos (`orders`):** Creación de órdenes (`user_id`, `product_id`, `quantity`, `order_date`) y consulta de historial por usuario.

## 3. Requerimientos Implementados
- **RF-01 (Gestión de Pedidos):** Creación de orden con fecha actual y retorno de ID único de confirmación.
- **RF-02 (Catálogo e Historial):** Visualización de precios en formato monetario e historial privado por cliente.
- **RNF-01 (Integridad Referencial):** Restricción mediante claves foráneas (`FOREIGN KEY`) en `orders` hacia `users` y `products`.

## 4. Artefactos de Diseño (UML y DER)
1. [Diagrama de Casos de Uso](./docs/a_casos_de_uso.png)
2. [Diagrama de Clases](./docs/b_diagrama_clases.png)
3. [Diagrama de Actividades](./docs/c_diagrama_actividades.png)
4. [Diagrama Entidad-Relación](./docs/d_entidad_relacion.png)
