# PROGRA-3
password = input("Clave: ")

# Agregar prints para investigar (Tal cual pide la slide)
print(f"DEBUG tipo: {type(password)}")
print(f"DEBUG valor: [{password}]")
print(f"DEBUG len: {len(password)}")

# BUG: input() devuelve texto, pero aquí comparamos con un número (1234).
# Esto siempre dará False.
if password == 1234: 
    print("Acceso concedido")
else:
    print("Acceso denegado")


password = input("Clave: ")

# CORRECCIÓN: Quitamos los prints de debug y comparamos texto con texto ("1234").
if password == "1234": 
    print("Acceso concedido")
else:
    print("Acceso denegado")
