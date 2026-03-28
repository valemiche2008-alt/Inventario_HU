# Inventario_HU
# PROGRAMA DE INVENTARIO SIMPLE

# Solicitar el nombre del producto
nombre = input("Ingrese el nombre del producto: ")

# Validar y solicitar el precio
while True:
    try:
        precio = float(input("Ingrese el precio del producto: "))
        if precio < 0:
            print("Error: el precio no puede ser negativo.")
        else:
            break
    except ValueError:
        print("Error: ingrese un número válido para el precio.")

# Validar y solicitar la cantidad
while True:
    try:
        cantidad = int(input("Ingrese la cantidad del producto: "))
        if cantidad < 0:
            print("Error: la cantidad no puede ser negativa.")
        else:
            break
    except ValueError:
        print("Error: ingrese un número entero válido para la cantidad.")


# Cálculo del costo total
costo_total = precio * cantidad


# Mostrar resultados en consola

print("--- RESULTADO ---")
print(f"El Producto es: {nombre} Su valor es de: {precio} la cantidad que pediste fue: {cantidad} y su total: {costo_total}")


# Descripción general del programa
# Este programa solicita al usuario el nombre, precio y cantidad de un producto.
# Valida que los datos numéricos sean correctos.
# Luego calcula el costo total multiplicando el precio por la cantidad.
# Finalmente, muestra toda la información en consola de forma clara.
