# OWASP-Juice-Shop

## SQL Inyection

La web tiene vulnerabilidades a inyecciones SQL.

Para explotarlo en el Login ingresamos la siguiente sentencia SQL con una contraseña cualquiera y ya nos permitiría el Login:

![image](https://github.com/user-attachments/assets/c8ce89a3-5bff-425c-a1dd-c92960e8c14b)

![image](https://github.com/user-attachments/assets/bacc1ff8-b874-4828-a620-6b930f7a4070)

Y entramos como admin a la aplicación:

![image](https://github.com/user-attachments/assets/1fda8b2b-9ca7-462c-a4d9-a286d9c55a8d)


## Exposición de datos del usuario

No tiene controlada las entradas de las peticiones en las URLs, permietiendo ver indormación del usuario logueado:

![image](https://github.com/user-attachments/assets/5be1bd34-dd4b-45f3-b834-62f3e32e1a13)

## Servicio FTP

No tiene el directorio del servicio ftp oculto:

![image](https://github.com/user-attachments/assets/53e551d6-31a0-4736-a60a-710839035adf)


![image](https://github.com/user-attachments/assets/6b1fff73-7f81-4fff-8fe6-2aa5d91fe170)

## Endpoint Administración

Tiene un endpoint llamado administración donde podemos ver todos los usuarios registrados:

![image](https://github.com/user-attachments/assets/9e187548-fe49-452c-91c9-64211f58dcc7)


## Vulnerabilidad XSS

En la barra de búsqueda podemos insertar script xss:

![image](https://github.com/user-attachments/assets/b87fcd45-fe80-430a-9152-2cd3a162b81b)

![image](https://github.com/user-attachments/assets/c9ab2e27-d567-481e-99e1-fb42c87066c4)

Al ser vulnerable a XSS, he probado a levantarme un servidor python que escuche el puerto 4444, y en la web ejecuto un script que robe la cookie de sesion del usuario logueado, para que el servidor lo reciba:

![image](https://github.com/user-attachments/assets/5934c899-7294-46da-a780-1666e138b4e1)

![image](https://github.com/user-attachments/assets/4caa8e13-8fd9-4f3e-af67-48295d66314d)

