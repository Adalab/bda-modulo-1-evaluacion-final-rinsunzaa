# EVALUACION MODULO 1 - Rocío Insunza

Ejercicios de evaluacion del modulo 1

## FUNCIONES

##### 1. Agregar un producto

Permite añadir un producto al inventario. 
Si el producto ya existe, se actualiza su cantidad.  
Si no existe, se añade como un nuevo elemento de la lista.
```bash
def agregar_producto(nombre, precio, cantidad):
```

##### 2. Ver_inventario()
Muestra todos los productos guardados en el inventario con su nombre, precio y cantidad.
```bash
def ver_inventario(inventario):
```

##### 3. Buscar_producto(nombre)
Permite localizar un producto por su nombre y mostrar su información.  
Si no existe, indica que no ha sido encontrado.
```bash
def buscar_producto(inventario, nombre):
```

##### 4. Actualizar_stock(nombre, cantidad)
Modifica la cantidad disponible de un producto concreto dentro del inventario.
```bash
def actualizar_stock(nombre, cantidad):
```

##### 5. Eliminar_producto(nombre)
Elimina un producto de la lista de inventario.
```bash
def eliminar_producto(nombre):
```

##### 6. Calcular_valor_inventario()
Calcula el valor total del inventario a partir del precio y cantidad de cada producto.
```bash
def calcular_valor_inventario(nombre):
```

##### 7. Realizar_compra()
Simula una compra, actualiza el stock y registra la operación realizada.
```bash
def realizar_compra():
```