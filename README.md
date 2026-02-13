# 🚀 Tarea 14: Gestión de Base de Datos en Odoo 18

En esta tarea tuvimos que montar, con docker compose, Odoo con PostgreSQL en el cual tuvimos que hacer lo que nos indicaba los distintos apartados del trabajo.

Antes de empezar, tenemos que crear la base de datos en PostgreSQL y luego, una vez creada, iniciar sesión en Odoo e instalar el módulo "Facturación"

<img width="961" height="796" alt="Captura desde 2026-02-13 09-13-20" src="https://github.com/user-attachments/assets/413d664d-45da-4f09-b823-9c7ff510735a" />

<img width="961" height="796" alt="Captura desde 2026-02-13 08-59-19" src="https://github.com/user-attachments/assets/9d1b3b00-5ead-4c84-b4ba-d43465f7b15b" />
---

## Apartado 1: Creación de Tablas Personalizadas

En este primer paso, creamos la tabla `EmpresasFCT`

## Apartado 2: Población de Datos
Una vez definida la estructura, se han insertado cinco registros representativos mediante la sentencia `INSERT INTO`. Los datos son ficticios y sirven para validar que los tipos de datos (booleanos, enteros y fechas) funcionan correctamente.

## Apartado 3: Consulta de Gestión de Empresas
Se ha realizado una consulta de selección simple para listar todas las empresas de la nueva tabla. El orden de los resultados se ha establecido de forma descendente basándose en la fecha de contacto, permitiendo visualizar primero las interacciones más recientes.

## Apartado 4: Filtrado de Contactos en Odoo
Este apartado requiere trabajar con la tabla nativa `res_partner`. Hemos filtrado los registros para obtener únicamente personas físicas (contactos) que no pertenezcan a la ciudad de **Tracy**.

* Se ha utilizado un `LEFT JOIN` para vincular el contacto con su empresa padre.
* Los resultados se presentan ordenados alfabéticamente por el nombre comercial de la empresa asociada.

## Apartado 5: Análisis de Reembolsos de Proveedores
Utilizando la tabla `account_move`, hemos extraído un listado de facturas rectificativas de proveedor (tipo `in_refund`). Esta consulta es vital para el control contable de devoluciones.

* Se muestran campos clave como el número de factura y el total sin impuestos.
* El listado se organiza cronológicamente, priorizando las facturas más nuevas.

## Apartado 6: Segmentación de Clientes por Volumen
En este ejercicio hemos aplicado funciones de agregado para identificar clientes recurrentes. Se han filtrado únicamente facturas de venta confirmadas (`posted`).

* Se ha empleado la cláusula `GROUP BY` sobre el nombre de la empresa.
* Se ha utilizado `HAVING` para filtrar solo aquellos clientes que superan el umbral de dos facturas emitidas.

## Apartado 7: Actualización Masiva de Dominios
Finalmente, se ha ejecutado una sentencia de actualización (`UPDATE`) para modificar los correos electrónicos de los contactos. Se ha reemplazado el dominio `@bilbao.example.com` por el nuevo dominio corporativo `@bilbao.bizkaia.neus`.

