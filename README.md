# Proyecto Urban Grocers 
# Descripción: Un equipo QA Engineer está comprobando cómo la aplicación Urban Grocers crea kits de productos.
# En este proyecto se trabajará la lista de comprobación para el campo "name" en la solicitud de creación de un kit de productos.

# Lista de comprobación:
  1.- El número permitido de caracteres (1): kit_body = { "name": "a"}
  2.- El número permitido de caracteres (511): kit_body = { "name":"El valor de prueba para esta comprobación será inferior a"}
  3.- El número de caracteres es menor que la cantidad permitida (0): kit_body = { "name": "" }
  4.- El número de caracteres es mayor que la cantidad permitida (512): kit_body = { "name":"El valor de prueba para esta comprobación será inferior a” }
  5.- Se permiten caracteres especiales: kit_body = { "name": ""№%@"," }
  6.- Se permiten espacios: kit_body = { "name": " A Aaa " }
  7.- Se permiten números: kit_body = { "name": "123" }
  8.- El parámetro no se pasa en la solicitud: kit_body = { }
  9.- Se ha pasado un tipo de parámetro diferente (número): kit_body = { "name": 123 }

# Pasos:
# 1.- Iniciar el servidor y actualizar el URL en el archivo configuration.py
# 2.- Abrir el archivo create_kit_name_kit_test.py
# 3.- Correr cada una de las pruebas y comrpobar el resultado.