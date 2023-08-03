# Changelog

## Version 1.0.1

### Cambios en la organización de archivos:

- Archivo `backend.php`: Contiene las funciones relacionadas con el backend del plugin.
- Archivo `frontend.php`: Contiene las funciones relacionadas con el frontend del plugin.
- Archivo `cron.php`: Contiene las funciones relacionadas con la programación de tareas cron para actualizar los precios.

### Funciones Backend:

- Se ha agregado un registro de errores en el caso que no pueda obtener el API del Dolar Blue

## Version 1.0

### Funciones Backend:

- `dolarblue_wc_is_woocommerce_active()`: Verifica si WooCommerce está activo.
- `dolarblue_wc_show_install_notice()`: Muestra un mensaje de aviso si WooCommerce no está activo.
- `dolarblue_wc_check_woocommerce_dependency()`: Verifica si WooCommerce está activo y muestra el mensaje de aviso si no lo está.
- `add_product_custom_field()`: Muestra el campo personalizado "precio_dolar_blue" en el backend del producto.
- `save_product_custom_field($post_id)`: Guarda el valor del campo personalizado como meta data del producto.
- `update_product_prices_in_ars()`: Actualiza los precios en ARS de todos los productos basado en el valor del dólar blue.
- `schedule_update_product_prices_cron()`: Programa la tarea cron para actualizar cada 15 minutos.
- `define_every_15_minutes_interval($schedules)`: Define el intervalo de tiempo "every_15_minutes".

### Funciones Frontend:

- `get_dolar_blue_value()`: Obtiene el valor del dólar blue desde la API.
- `add_dolar_blue_value_to_price_html($price_html, $product)`: Agrega el valor del 'precio_dolar_blue' en el HTML del precio.
- `add_custom_styles_to_frontend()`: Agrega el CSS en el frontend para estilizar el contenido.
- `get_product_dolar_blue_value($product_id)`: Obtiene el valor del 'precio_dolar_blue' desde el producto.
- `display_cart_and_checkout_prices($product_name, $cart_item, $cart_item_key)`: Muestra el precio en ARS en el carrito y en el checkout.

### Otras funciones:

- `get_dolar_blue_value()`: Obtiene el valor del dólar blue desde la API.