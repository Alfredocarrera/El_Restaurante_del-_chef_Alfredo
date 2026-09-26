# El_Restaurante_del-_chef_Alfredo
desarrollo de automatizacion de n8n para un restaurante en telegram usando agente de IA.

# Implementacion del Restaurante del Chef Alfredo

## Sistema Inteligente de Pedidos con Telegram, n8n AI Agent y Google Sheets

1. CONFIGURACIÓN DE LA BASE DE DATOS (Google Sheets)
Crea un libro en Google Sheets con el nombre exacto: Restaurante_del_Chef_Alfredo.
Configura 4 pestañas e ingresa los encabezados en la primera fila (Fila 1):
Hoja 1: MENU
Columna A Columna B Columna C Columna D Columna E Columna F
id_producto nombre descripcion precio categoria stock
Ejemplo de datos:
PROD-01 | Café Latte 12oz | Café espresso con leche | 12.00 | Bebidas | 50
PROD-02 | Empanada de Pollo | Empanada horneada | 15.00 | Comidas | 30
PROD-03 | Muffin Chocolate | Muffin recién horneado | 10.00 | Snacks | 20

Hoja 2: PEDIDOS
Columna A Columna B Columna C Columna D Columna E Columna F Columna G
id_pedido id_usuario detalles_pedido total_pago estado fecha hora
Hoja 3: USUARIOS
Columna A Columna B Columna C Columna D
telegram_id nombre_completo departamento_oficina puntos_lealtad

Hoja 4: CARRITOS_TEMPORALES
Columna A Columna B Columna C
telegram_id items_json ultima_actualizacion
