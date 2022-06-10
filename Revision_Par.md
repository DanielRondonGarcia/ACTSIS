# Revisión Par

## Índice de contenido

*   [Paso 1 - Branch](#paso-1---branch)
*   [Paso 2 - Notas de Versión](#paso-2---notas-de-versión)
*   [Paso 3 - Verificación del codigo](#paso-3---verificación-del-codigo)
*   [Paso 4 - Verificación si el objeto no se wrappea](#paso-4---verificación-si-el-objeto-no-se-wrappea)
*   [Paso 5 - Verificar si lleva spool y el tipo de script](#paso-5---verificar-si-lleva-spool-y-el-tipo-de-script)
*   [Paso 6 - Verificar FI-14](#paso-6---verificar-fi-14)
*   [Paso 7 - Verificar la integración](#paso-7---verificar-la-integración)
*   [Paso 8 - Verificar Informe de cambios](#paso-8---verificar-informe-de-cambios)
*   [Paso 9 - SGI](#paso-9---SGI)
*   [Paso 10 - Correo](#paso-10---correo)
*   [Paso 11 - Carpeta](#paso-11---carpeta)
*   [Paso 12 - Aspectos especiales](#paso-12---aspectos-especiales)


### **Paso 1 - Branch**

Verificar si lleva branch.
* El numero del Requerimiento debe ser con el interno, NO EL EXTERNO
* Si lleva branch, empezar a revisar el codigo de cada objeto desde el branch.
* si el objeto es nuevo, revisar si se agregó al maestro en orden alfabetico.
* Veificar si el tipo de objeto está en la carpeta correcta.
#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 2 - Notas de Versión**

*   No deben ir numeros de Requerimientos
*   Revisar que la descripción sea acorde al cambio realizado
*   En el body solo va la nota de versión actual, es decir, no deben de haber notas de versión antiguas
*   Revisar que las fechas sean las misma de la ultima modificación del archivo y sea la misma al de la carpeta zeus o el branch o si es el caso en el SGI cuando son versiónes propias de empresas
*   Tambien revisar si la fecha del objeto está actualizado en el SGI en el apartado de objetos
*   Verificar las versiones sean las correctas
*   Quitar comentarios de versión en la línea


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 3 - Verificación del codigo**
* Se debe probar el desarrollo realizado
* Verificar codigo sea el mismo en las diferentes partes como SGI, Zeus, SVN y Script
* No dejar nada comentado que no sea nada funcional
* Alineación del código
#### Estandar:
  *   Diferente es `"<>"` y no así `"!="`


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 4 - Verificación si el objeto no se wrappea**
Verificar en el archivo ubicado en el grupo SAC
https://actsis.sharepoint.com/:b:/s/SAC/ETkGkIbpFItCoiS0b_VfvnEBiLLfdsYq7EJSc0HnS5CV9Q?e=fH4lLv


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 5 - Verificar si lleva spool y el tipo de script**
Ir a verificar si
https://actsis.sharepoint.com/:t:/s/SAC/EXqyK71NxqJCvvf-4dF2wYMBnXLi32TPznv3_vk1bxlydw?e=8OL6TF
```SQL
UNA LINEA EN BLANCO AL PRINCIPIO
-- SPOOL ARCHIVOS 
CENS 
\\epm-file02\APLIC\Externos\adminfo\Filiales\cens\Spool\ 

CHEC 
\\epm-file02\APLIC\Externos\adminfo\Filiales\chec\Spool\ 

EDEQ 
\\epm-file02\APLIC\Externos\adminfo\Filiales\edeq\Spool\ 

ESSA DATOS 
CONNECT &usuario/&clave@&base 
SPOOL \\essa-file08\ETI\c-ti\TEMPORAL\ACTSIS\ 

ESSA OBJETOS 
CONNECT SAC/&clave@&base 
SPOOL \\essa-file08\ETI\c-ti\TEMPORAL\ACTSIS\ 

Otras empresas: SIN RUTA DE SPOOL 

Identificación del tipo de script 
O = para objetos = CREATE, ALTER, DROP 
D = para datos = INSERT, DELETE, UPDATE  
A = para auditoria 
```


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 6 - Verificar FI-14**
*Instalación sea una sola
*El nombre sea el mismo al del archivo
*Dejar el Req ext
*Nombre de objetos y script sean correctos


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 7 - Verificar la integración**
*Verificar si es para todas las empresar solo cuando es despliegue
*Verificar si la versión anterior es la correcta a la de la del documento
*se omite las versiones temporales


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 8 - Verificar Informe de cambios**
*Funcionalidad no va nada técnico
*MejoraAjustes es la explicación al minimo detalle del cambio
![image](https://user-images.githubusercontent.com/61068392/170584850-cb1a27d8-25e5-4d44-9635-a3a37cabc09c.png)


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 9 - SGI**
*   Solo por despliegue se pone el INFORME_CAMBIOS


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 10 - Correo**
*   Manejar la mismo tamaño y tipo de letra.


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 11 - Carpeta**
*   Cuando son reportes, se crea fichro al mismo nivel del Scr.

    Ejemplo:
    ```
    //74884--
            |-App--.
            |-Exe--
                   |-Scr
                   |-Sql
                   |-Crystal
                   |-Etc.
    ```


#
[🔝 Volver al índice](#índice-de-contenido)
#

#

### **Paso 12 - Aspectos especiales**
*   ESPY no lleva reportes Progen, solo reportes



#
[🔝 Volver al índice](#índice-de-contenido)
#

#
