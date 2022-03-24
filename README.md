<div>
<p style = 'text-align:center;'>
<img src="https://user-images.githubusercontent.com/61068392/158889190-5344bfc7-84fe-4392-be22-b5ce970c8a93.png" alt="JuveYell" width="300px">
</p>
</div>




## Índice de contenido

*   [Consultas](#consultas)
    *   [Datos Generales (ATC_CONGEN)](#datos-generales-atc_congen)
    *   [Consulta Saldo (ATC_SALDOS)](#consulta-saldo-atc_saldos)
    *   [Consulta Conexos (FAC_CNXCON)](#consulta-conexos-fac_cnxcon)
    *   [Módulo de consulta de Medidores (LAB_ACTCON)](#módulo-de-consulta-de-medidores-lab_actcon)
    *   [Consulta de Sellos (LAB_INGSEL)](#Consulta-de-Sellos-LAB_INGSEL)
    *   [Consulta Instaladores Técnicos Electricistas (MAT_MEELEC)](#consulta-instaladores-técnicos-electricistas-mat_meelec)
    *   [Consulta Agenda Facturación (FAC_AGEFAC)](#consulta-agenda-facturación-fac_agefac)
    *   [Impuesto de Alumbrado público (EQT_ACTALU)](#impuesto-de-alumbrado-público-eqt_actalu)
    *   [Refacturaciones (AUD_CONREF)](#refacturaciones-aud_conref)
    *   [Estadísticas por Ciclo (FAC_CICVER)](#estadísticas-por-ciclo-fac_cicver)
    *   [Buscar Clientes (ATC_BUSCLI)](#buscar-clientes-atc_buscli)


### **Consultas**

### **Datos Generales (ATC_CONGEN)**

URL: 
```
https://172.25.3.17:4443/SAC/Vistas/App/ATC_CONGEN.aspx
```
Ruta: 
```
Consultas/Datos Generales
```

*   Consultar toda la informacion de ese cliente 
como Estados del cliente, lugar de residencia, etc.
*   Historico de consecutivos de facturación.
*   Pagos.
*   Cartera actual, pendiente y congelada.
*   Las financiaciones
*   Los medidores e historico de consupor por medidor/franja.
*   Elementos asociados.
*   Revisiones (Visitas).
*   Los procesos de recuperacion de consumo.
*   Auditoría de datos sensibles.

Resumen de todo el cliente.
![image](https://user-images.githubusercontent.com/61068392/158891238-f2e19336-3fd8-41b5-9317-7c5cce20895d.png)

Datos generales del cliente.
![image](https://user-images.githubusercontent.com/61068392/158891872-1098f457-995e-4782-985f-9401b1d5219f.png)

La gráfica de Consumos Históricos visualiza el consumo del cliente durante los últimos 6 meses, comparado contra el consumo promedio del grupo al que pertenece el cliente.
![image](https://user-images.githubusercontent.com/61068392/158893325-57f23e85-1fd5-4fb2-b460-1583a4dd8b45.png)

Agrupación de Clientes:
*   Municipio
*   Código de Área
*   Clase de Servicio
*   Estrato
*   Área Común
*   Ciclo
*   Sección de Ruta Lectura

Para los No Residenciales, adicionalmente
Rango del promedio del consumo entre 0-
500, 501-2000, 2001-10000 y mayor a 10000.



#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Consulta Saldo (ATC_SALDOS)**
URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/ATC_SALDOS.aspx
```
Ruta: 
```
Consultas/Consulta Saldo
```

Consulta la cartera de un cliente: Cartera actual,
Cartera financiada, Cartera congelada y Conceptos
programados a próximas facturaciones

Consultar saldos pendiente para un código del cliente esécifico y realizar abonos por cualquier concepto.
![image](https://user-images.githubusercontent.com/61068392/158900674-f3726594-c489-4fa0-87e5-d4c384f232d5.png)



#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Consulta Conexos (FAC_CNXCON)**
URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/FAC_CNXCON.aspx
```
Ruta: 
```
Consultas/Consulta Conexo
```
Consulta los conexos de un cliente: Conexos en
crédito, Financiación, Conexos Próximas facturaciones, Conexos Inmediatos, Conexos Futura

Permite la consulta y/o anulacipon de liquidaciones y/o cotizaciones de servicios conexsos realizadas a un cliente y a la actualizacion de los mensajes ingresados a la liquidacion.
![image](https://user-images.githubusercontent.com/61068392/158901933-3902287c-39e8-4041-a5f6-b4ab40a50b5e.png)



#
[🔝 Volver al índice](#índice-de-contenido)
#


### **Módulo de consulta de Medidores (LAB_ACTCON)**

Consulta de Medidores: Consultar la información general, de predio y técnica del medidor, además de la información de lecturas, sellos e historia general del medidor.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/LAB_ACTCON.aspx
```
Ruta: 
```
Consultas/Consulta medidores
```

Trae información historica del medidor
*  Información General: Nos trae la información básica del medidor.
*  Información del predio: Nos trae la información de donde se encuentra ubicado el medidor.
*  Información Técnica: Caracteristicas  del medidor
*  Información Adicional: Información técnica del proveedor, calificacion.
*  Lecturas del medidor: La información de la ultima lectura y promedio historico
*  Sellos: Los sellos que se encuentran instalados en el medidor, ubicación, tipo de sello, fecha de instalación, etc.
*  Historia dle medidor
*  Detalles de  lecturas


#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Consulta de Sellos (LAB_INGSEL)**

Consulta de Sellos: Consultar la información general, histórica y técnica del sello

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/LAB_INGSEL.aspx
```
Ruta: 
```
Consultas/Consulta Sellos
```


#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Consulta Instaladores Técnicos Electricistas (MAT_MEELEC)**

Consulta de Técnicos Electricistas: Consultar datos de los Técnicos Electricistas autorizados para realizar y presentar obras ante la empresa y las instalaciones realizadas y rechazadas.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/MAT_MEELEC.aspx
```
Ruta: 
```
Consultas/Consulta Instaladores
```
*  Instalaciones aprovadas y rechazadas
*  Datos básicos
*  Suspenciones
*  Póliza


#
[🔝 Volver al índice](#índice-de-contenido)
#


### **Consulta Agenda Facturación (FAC_AGEFAC)**

Consulta Agenda de Facturación: Consultar las programaciones y ejecuciones de las fechas de facturación para los ciclos activos.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/FAC_AGEFAC.aspx
```
Ruta: 
```
Consultas/Consulta Agenda Facturación
```
Nos muestra todos los ciclos que se encuentran antivos en la empresa, se puede buscar por ciclos programados o ejecutados.

Se pueden buscar clientes activos, clientes nuevos, medidores instalados, etc


#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Impuesto de Alumbrado público (EQT_ACTALU)**

Consulta Alumbrado Público: Consultar los porcentajes, topes y valores liquidados por concepto de Impuesto de Alumbrado Público.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/EQT_ACTALU.aspx
```
Ruta: 
```
Consultas/Consulta Imp. Alumbrado Público
```



#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Refacturaciones (AUD_CONREF)**

Consulta de Refacturaciones: Auditar los ajustes refacturaciones que se han realizado a un cliente.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/AUD_CONREF.aspx
```
Ruta: 
```
Consultas/Consulta Refacturaciones
```



#
[🔝 Volver al índice](#índice-de-contenido)
#


### **Estadísticas por Ciclo (FAC_CICVER)**

Estadísticas por Ciclo: Consultar estadísticas generales por ciclo, permitiendo ver el detalle de los clientes y sus respectivas gráficas.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/FAC_CICVER.aspx
```
Ruta: 
```
Consultas/Estadisticas por ciclo
```

Muestra los clienters actives, los medidores instalados, estado de los clientes, la calse de servicio, el municipio, estado de suministro, grupos CU, codigo de área 

#
[🔝 Volver al índice](#índice-de-contenido)
#


### **Buscar Clientes (ATC_BUSCLI)**

Consultar en el sistema clientes que coincidan con los diferentes criterios de búsqueda ingresados en la pantalla.

URL: 
```
https://sacnet-rc.actsis.com/SAC/Vistas/App/ATC_BUSCLI.aspx
```
Ruta: 
```
Consultas/Buscar Clientes
```

Muestra los clienters actives, los medidores instalados, estado de los clientes, la calse de servicio, el municipio, estado de suministro, grupos CU, codigo de área 

#
[🔝 Volver al índice](#índice-de-contenido)
#
