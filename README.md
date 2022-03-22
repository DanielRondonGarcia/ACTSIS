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
