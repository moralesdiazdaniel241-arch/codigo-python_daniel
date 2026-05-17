# codigo-python_daniel
Este proyecto es un programa básico desarrollado en Python para gestionar el inventario de productos de una tienda. El sistema permite verificar el stock actual de cada artículo y calcular automáticamente la cantidad que se debe pedir cuando el inventario está por debajo del stock mínimo establecido.

# inventaro ={ codigo de articulo , nombre , stock  actual, stock minimo}
inventario = [1306, "leche", 20, 25] ,[1020,"galletas",15,15], [2050,"pan",5,5], [1120,"sal",8,8], [2020,"azucar",25,30]

def  calcular (stock_actual, stock_minimo):
 
 if stock_actual < stock_minimo:
    return stock_minimo - stock_actual
 
 else:
    return 0 
 
for articulo in inventario:
    codigo = articulo [0]
    nombre = articulo [1]
    stock_actual = articulo [2]
    stock_minimo = articulo [3]   

    cantidad_a_comprar = calcular(stock_actual, stock_minimo) 

    print(f" Código: {codigo}")
    print(f"Artículo: {nombre}")
    print(f"Stock actual: {stock_actual}")
    print(f"Stock mínimo: {stock_minimo}")
    print(f"Cantidad a pedir: {cantidad_a_comprar}")
