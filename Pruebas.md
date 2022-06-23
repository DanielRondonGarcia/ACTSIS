# Pruebas GEN

## Índice de contenido

*   [Paso 1 - Contextualización de la prueba en el correo](#paso-1---Contextualización-de-la-prueba-en-el-correo)
*   [Paso 2 - Construcción de escenarios de prueba](#paso-1---Construcción-de-escenarios-de-prueba)

### **Paso 1 - Contextualización de la prueba en el correo**

* Generalmente llega un correo primero diciendolo que cree los escenarios de prueba
* Verificar Req, No Instalación, si es envío al cliente, los repositorios que tuvieron cambios
* Leer las observaciones

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Paso 1 - Construcción de escenarios de prueba**
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
#
[🔝 Volver al índice](#índice-de-contenido)
#
