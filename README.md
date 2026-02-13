# 🚀 Tarea 14: Gestión de Base de Datos en Odoo 18

En esta tarea tuvimos que montar, con docker compose, Odoo con PostgreSQL en el cual tuvimos que hacer lo que nos indicaba los distintos apartados del trabajo.

Antes de empezar, tenemos que crear la base de datos en PostgreSQL y luego, una vez creada, iniciar sesión en Odoo e instalar el módulo "Facturación"

<img width="961" height="796" alt="Captura desde 2026-02-13 09-13-20" src="https://github.com/user-attachments/assets/413d664d-45da-4f09-b823-9c7ff510735a" />

<img width="961" height="796" alt="Captura desde 2026-02-13 08-59-19" src="https://github.com/user-attachments/assets/9d1b3b00-5ead-4c84-b4ba-d43465f7b15b" />

---

## Apartado 1
En este primer paso, creamos la tabla `"EmpresasFCT"`, añadiéndole los campose de "idEmpresa", "nombre", "quiereAlumnos", "numAlumnos" y "fechaContacto":

<img width="584" height="367" alt="Captura desde 2026-02-13 09-13-36" src="https://github.com/user-attachments/assets/e0aee906-a0bb-4231-866d-83feabfe0fbc" />

## Apartado 2
Ahora, con la empresa ya creada, introducimos los datos de empresas inventadas:

<img width="646" height="491" alt="Captura desde 2026-02-13 09-33-02" src="https://github.com/user-attachments/assets/f1da6fa4-ed36-4cfc-9cdf-7dc6ca555172" />

## Apartado 3
Para este apartado, tenemos que hacer una consulta que muestr estos datos en una tabla y que los ordene por fechaContacto:

<img width="646" height="570" alt="Captura desde 2026-02-13 09-33-20" src="https://github.com/user-attachments/assets/ba9e0475-4682-4cc6-82f5-4acf007ff079" />

## Apartado 4
Con el módulo de "Facturación" instalado, ahora tenemos que obtener el listado de todos los contactos de Odoo por su Nombre, Ciudad que no sea Tracy y Nombre comercial de la empresa:

<img width="646" height="851" alt="Captura desde 2026-02-13 09-43-03" src="https://github.com/user-attachments/assets/56ff763c-2dde-4162-bf26-edd02db71c6a" />

## Apartado 5
Con los datos de "Facturación", tenemos que listar las empresas que han emitido algún reembolso:

<img width="646" height="538" alt="Captura desde 2026-02-13 09-51-42" src="https://github.com/user-attachments/assets/4a993287-6616-4b38-b8c5-e19d76b190a2" />

## Apartado 6
Con los mismos datos de antes, ahora tenemos que listar las empresas que han emitido más de dos facturas de venta:

<img width="646" height="538" alt="Captura desde 2026-02-13 09-52-51" src="https://github.com/user-attachments/assets/a9ab6aca-9c5f-4893-82ae-24993dac67a1" />

## Apartado 7
Por último, tenemos que actualizar el correo de los contactos:

<img width="646" height="538" alt="Captura desde 2026-02-13 09-53-33" src="https://github.com/user-attachments/assets/df443ae8-056a-4c93-b756-7dda3a089a51" />
