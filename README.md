# OWASP-Juice-Shop

## SQL Inyection

La web tiene vulnerabilidades a inyecciones SQL.

Para explotarlo en el Login ingresamos la siguiente sentencia SQL con una contraseña cualquiera y ya nos permitiría el Login:

![image](https://github.com/user-attachments/assets/c8ce89a3-5bff-425c-a1dd-c92960e8c14b)

![image](https://github.com/user-attachments/assets/1fda8b2b-9ca7-462c-a4d9-a286d9c55a8d)


## Exposición de datos del usuario

No tiene sanizadas las entradas de las peticiones en las URLs, permietiendo ver indormación del usuario logueado:

![image](https://github.com/user-attachments/assets/5be1bd34-dd4b-45f3-b834-62f3e32e1a13)
