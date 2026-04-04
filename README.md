# EVALUACION MODULO 1 - Rocío Insunza

Ejercicios de evaluacion del modulo 1

## FUNCIONES

##### 1. Agregar un producto

Para agregar un producto, existente o no, a nuestra lista de productos hemos de crear un metodo (def) especificando los atributos del producto. 
```bash
def agregar_producto(nombre, precio, cantidad):
```

Luego hemos de usar un bucle (for) para que analice atributo a atributo la lista para por una parte revisar si el producto ya existe y solo tener que modificar la cantidad o añadir el producto nuevo a la lista.
```bash
for producto in inventario:
```

Para revisar si el producto ya esta en nuestra lista vamos a utilizar el codigo (if) para crear la condicion de si esta el producto ya ubicado en la lista con el igualando el primer atributo de nombre y en el caso de positivo que solo sume las cantidades del producto que queremos agregar con el que coincida en la lista. 
*Ponemos return al final para que una vez llegue a la similitud, pare de buscar y nos devuelva la informacion.
```bash
if producto["nombre"] == nombre:
    producto["cantidad"] = producto["cantidad"]+cantidad
    return
```
En caso negativo, saldremos del bucle para añadir a la lista el nuevo producto, creando un append descriptivo.
```bash
inventario.append({"nombre": nombre,"precio": precio, "cantidad": cantidad})
```

##### 2. Ver inventario
Para ver el inventario, creamos un metodo (def) señalizando lo que queremos visualizaar
```bash
def ver_inventario(inventario):
```
A partir de aqui, creamos un bucle for para que revise atributo por atributo para luego plasmarlo en un print.
```bash
for producto in inventario:
    print(f"Nombre: {producto['nombre']}, Precio: ${producto['precio']}, Cantidad: {producto['cantidad']}")
```
##### 3. buscar_producto(nombre)
Para buscar un prodcuto dentro de nuestra lista creamos un metodo (def) especificando nuestra listado y el atributo en el que queremos que busque.
```bash
def buscar_producto(inventario, nombre):
```
Creamos un bucle (for) para que revise y busque uno a uno el producto que le estamos solicitando dentro de nuestra lista.
```bash
for producto in inventario:
```
Y creamos la condicional para cuando encuentro el mismo nombre que le indicamos nos lo muestre.
```bash
if producto["nombre"] == nombre:
    print(f"Nombre: {producto['nombre']}, Precio: {producto['precio']}, Cantidad: {producto['cantidad']}")
    return
```
De lo contrario, si le estamos pidiendo que busque un producto que no esta en nuestra lista, salimos del bucle for para indicarlo que nos imprima que no esta el producto.
```bash
print("no encontrado")
```
