# Pruebas GEN

## Índice de contenido

*   [Paso 1 - Contextualización de la prueba en el correo](#paso-1---Contextualización-de-la-prueba-en-el-correo)
*   [Paso 2 - Construcción de escenarios de prueba](#paso-2---Construcción-de-escenarios-de-prueba)
*   [Paso 3 - Montar y compilar la solucion en Visual Studio](#paso-3---Montar-y-compilar-la-solucion-en-Visual-Studio)
*   [Paso 4 - Probar dentro del sitio las funcionalidades afectadas](#paso-4---Probar-dentro-del-sitio-las-funcionalidades-afectadas)
*   [Paso 5 - COMMIT](#paso-5---COMMIT)
*   [Paso 6 - SGI](#paso-6---SGI)

### **Paso 1 - Contextualización de la prueba en el correo**

* Generalmente llega un correo primero diciendolo que cree los escenarios de prueba
* Verificar Req, No Instalación, si es envío al cliente, los repositorios que tuvieron cambios
* Leer las observaciones

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Paso 2 - Construcción de escenarios de prueba**
Pre-condiciones:
Guía en repositorio SVN de ACTSIS (https://svn.actsis.com/svn/SGC/Guías-Desarrollo/EscenarioDePrueba)
* Consultamos el Rq en el SGI
```sql
SELECT :REQ || '-----------------------------------------------------------------------' REQ,
        NVL(pry_req.descripcion,    'No hay registro') SOLICITUD,
        NVL(pry_req.comentarios,    'No hay registro') ANALISIS,
        NVL(pry_req.restricciones,  'No hay registro') RESTRICCIONES,
        NVL(pry_req.supuestos,      'No hay registro') SUPUESTOS,
        NVL(pry_req.escenarios,     'No hay registro') ESCENARIO,
        NVL(pry_req.riesgos,        'No hay registro') RIESGOS
FROM    sgi.pry_requerimientos      pry_req
WHERE   numero_requerimiento =      :REQ
```

Ejemplo:

![image](https://user-images.githubusercontent.com/61068392/175323490-f5be3535-6d24-457a-b739-4020e633c82d.png)

* Revisar objetos modificados a nivel de SGI
* agregar dichos objetos con su descripción en Diseño
* Nos dirigimos a la ruta del Zeus (Des)
* Debemos copiar y pegar la carpeta del Rq dentro de `Pru`, luego debemos eliminar la carpeta dentro de `Des` (No cortar!)
* Despues dentro de `Exe` creamos una carpeta llamada `Doc`
* Pegamos la ultima versión del formato de pruebas (\\\zeus\SGC\DOCUMENTOS_SGC\Instalación y Entrega\Formatos)`FI-22 Escenarios de pruebas.docx`

<a href="file://zeus/SGC/DOCUMENTOS_SGC/Instalación y Entrega/Formatos" type="button">Abrir carpeta de formatos</a>

#

[Abrir carpeta de formatos]("file://zeus/SGC/DOCUMENTOS_SGC/Instalación y Entrega/Formatos")
[Prueba]("file://zeus/SGC/DOCUMENTOS_SGC/")

* Identificar el objetivo general [Contenido](https://svn.actsis.com/svn/SGC/Guías-Desarrollo/EscenarioDePrueba/Contenido)
* Verificar con el branch y el diseño obtenido del SGI que tenga los mismos objetos modificados
* Verificar objetos de base de datos en los scripts
* Ejecutar cada Script y verificar funcionamiento del mismo
  * Ejemplo:
  * 
  ```sql
  @\\zeus\ACTSIS\ACTSIS\GEN\Pru\57817\Exe\Scr\57817_01_01_MVC_O_GEN.sql
  ```
  
* El escenario de pruebas, si las pruebas son exitosas, se finaliza este documento bajo el nombre original y se le agrega `_PRUEBAS` y se hace una copia en `.PDF`

* [Más documentación acerca de las pruebas](\\\zeus\SGC\DOCUMENTOS_SGC\Instalación y Entrega\Procedimientos\PI-03 Pruebas internas.docx)

Observaciones
=============

Pueden ser error de sintaxis y ortografia, generalidades, etc.

* Ir diligenciando las observaciones con su imagen

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Paso 3 - Montar y compilar la solucion en Visual Studio**

* Verificar si en pre-requisitos necesita un repositorio aparte (Se deberá descargar el repositorio al mismo nivel del resto de repositorios y con el mismo nombre)
* Compilar los proyectos y verificar que estén correctos

Publicación
===========
Instructivo: (\\\zeus\SGC\DOCUMENTOS_SGC\Mantenimiento y Desarrollo\Instructivos\IM-09 Instalación de Aplicaciones .NET.DOCX)
* Clic derecho al proyecto web y vamos a la opcion `Publicar`
* Todas se llaman  `presentación.ACTSIS`
* Encontramos 3 opciones para publicar

  ![image](https://user-images.githubusercontent.com/61068392/175347491-02b6ca48-07eb-4451-b5f8-0fe00bc19e42.png)

* Configuración de los archivos de publicación
  
  ![image](https://user-images.githubusercontent.com/61068392/175348197-d5857778-5a6d-4bec-ae4d-3dee628ffa2d.png)

* Hacemos el despligue a nviel local y luego copiamos y pegamos al sitio de nosotros

* Url de mi sition: (file://vmact03/SitiosIIS/DRONDON) (https://drondon.actsis.com/)

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Paso 4 - Probar dentro del sitio las funcionalidades afectadas**

* Vamos iterando por los escenarios de uso y revisando funcionalidad  (Tambien a nivel de codigo)
* Vamos diligenciado el escenario de pruebas de la pantalla que se está revisando


Hallazgos
=========

El formato FI-24 se encuentra en: (\\\zeus\SGC\DOCUMENTOS_SGC\Instalación y Entrega\Formatos\FI-24_Reporte de Hallazgos.docx)
* Se guarda en una carpeta especial con la siguiente estructura:
               ```
                →App/Pru/Hallazgos
                ```
* Si se requiere, dentro de hallazgos se crea carpeta de anexos donde se agregan todos los anexos
                ```
                →App/Pru/Anexos
                ```

#
[🔝 Volver al índice](#índice-de-contenido)
#


### **Paso 5 - COMMIT**

* jenkins.runsettings: Cambiar los testCase para conveniencia.
* Debemos agregar el sitio en App.config del Test (host)

[Tutorial](https://actsis.sharepoint.com/sites/ACTSISQA/SitePages/GenTests-7-1-2563.aspx)

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Paso 6 - SGI**

*       Nos dirigimos a `Gestión/Verificación y Validación`.
*       Buscamos el REQ que probamos
*       Vamos diligenciando el correo
        
![image](https://user-images.githubusercontent.com/61068392/182729760-87867010-12ee-445c-8289-31ffd792dd19.png)


*       Luego le damos clic al botón Verificación
*       Verificamos que sea el # de la instalación
*       Verificamos cada Requerimiento del cliente
*       Verificar cada requerimiento funcional (Tiene el mismo nombre al REQ del ciente) y no funcional (por lo general son 3)
        *       Si no fue posible probarlo seleccionamos `No verificado`
        *       Agregamos en la Observación `Ok` si pasó y `No Aplica` si no se pudo probar
        *       En el caso del REQ funcional agregamos la misma observación que tenemos en el Correo
*       Marcamos verificado el REQ del cliente y de observación ponemos `Pruebas Satisfactorias`
*       Si hubieron devoluciones marcamos la casilla `Ind.Devol`
*       No marcar Liberar Instalación
*       Cambiar de responsable en la ventana `Verificación y Válidación de Instalaciones` a JREYES
*       ACT[5-31]
#
[🔝 Volver al índice](#índice-de-contenido)
#
