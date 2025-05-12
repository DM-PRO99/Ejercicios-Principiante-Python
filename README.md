# GESTION DE  INVENTARIO

Funcionalidades Principales del programa:
-Añadir productos al inventario.
-Consultar productos del inventario.
-Actualizar precios de los productos.
-Eliminar productos del inventario.
-Calcular el valor total del inventario.


## ¿Cómo funciona?

El programa tiene un menú de opciones para que facilite al encargado la opcion que se acomode en su momento poderla ejecutar y asi ahorrar tiempo
y que haya un orden en el inventario, un control de cada cosa.

OPCION 1 Y 2:
Cada que llegue un producto nuevo deberá ingresarse a la plataforma como adicion de un producto nuevo, luego la opcion 2 ya sea que pueda buscar
un nuevo o antiguo producto lo pueda encontrar en su base de datos.

OPCION 3:
Esta opcion nos permite poder hacer los pertinentes cambio de precio o cantidad,dependiendo de la salida de insumos o productos que se estén
demandando en el mercado para lelvar un pleno control.

OPCION 4:
Delete products nos permitirá que cuando un producto se haya agotado lo podamos eliminar de la base de datos para que asi no nos refleje ningun
desorden y confusiones a los clientes que quizás por error deseen comprarlo y ya no hayan existencias y todo para un mejor control y orden del
inventario.

OPCION 5:
Esta opcion nos permite hacer un calculo total del inventario de lo que tengamos a disposicion tanto en nuestra base de datos como en el inventario
local y llevar un registro y orden de lo que tenemos para ofrecer.

OPCION 6:
Es para cuando ya hayamos culminado las tareas podamos salir o retornar a otras opciones o dar por finalziado el uso.


**EJEMPLOS DE ENTRADA Y SALIDA DEL PROGRAMA:)**
Esta funcion me permite añadir productos a la base de datos la entrada es la cantidad que se van a añadir y como resultado la cantidad que queda en existencia
de los productos añadidos y ciertas caracteristicas como precio, y cantidad y se guardé exitósamente.


def add_product():
    """
   The user is prompted to enter the products
    """
    name = input("Enter product name: ")
    try:
        price = float(input("Enter product price: "))
        quantity = int(input("Enter product quantity: "))
        if price <= 0 or quantity < 0:
            print("Price must be positive and quantity must be non-negative.")
            return
        inventory[name] = {'price': price, 'quantity': quantity}
        print(f"Product '{name}' added successfully.")
    except ValueError:
        print("Invalid input. Price must be a number and quantity must be an integer.")



**OTRO EJEMPLO SERIA:)**
# Function to display the menu
def display_menu():
    """
    Displays the main menu with options.
    """
    print("\n--- Inventory Menu---")
    print("1. Add Product")
    print("2. Search Product")
    print("3. Update Product Price")
    print("4. Delete Product")
    print("5. Calculate Total Inventory Value")
    print("6. Exit")


**Se solicita al usuario que marque una opcion para asi mismo dar una salida a una funcion predeterminada detras de cada item,asi recibimos una entrada que seria marcar la opcion
que se requiere y la salida el resutlado que esperó de cada opcion puesta en el menu.**


Documentación:
[markdown] (https://docs.python.org/es/3/)
[markdown] (https://github.com/illuminaki/python-funciones)
