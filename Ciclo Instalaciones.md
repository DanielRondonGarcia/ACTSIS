# Ciclo de Instalación

## Índice de contenido

*   [Definición](#definición)
*   [Instalación](#Instalación)
*   [FI-14](#FI-14)
*   [Formatos](#Formatos)
*   [Duplicación de Instalaciones](#Duplicación-de-Instalaciones)
*   [Paso a Paso](#Paso-a-Paso)

### **Definición**

Se supone que cuando ya se va a hacer una instalación, sea un Req nuestro o alguen nos pidió que hicieramos la instalación, el Req ya debe estár terminado el desarrollo, el desarrollador ya hizo sus pruebas y asociados todos los obetos.

*   Generalmente el estado del Req está en `T :Trámite`
*   Si es una mejora que se envía a un cliente, entonces abrían 2 Req, uno externo del cliente y uno interno de ACTSIS, ambos Req deberían estar en `T :Trámite` 

¿Qué debemos mirar cuando nos entregan el Req para instalación?
*   Que las casilla Descripción, Restricciones, Supuestos, Análisis General, Escenarios de Uso y Riesgos e Impacto.
*   Tener todos los objetos relacionados y tener cargado el desarrollo.
![image](https://user-images.githubusercontent.com/61068392/160190827-37bf0610-ec48-4b14-be6c-43663e013b3d.png)


#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Instalación**

*   Casilla Envio cliente? :si lo marco quiere decir que lo estoy enviando directa, cuando no lo marco quiere decir que la instalación va a estar en `"Stan by"`.
*   Pre Requisitos: Se lo da la persona que lo mandóa hacer la instalación o si es usted mismo es el Resultado de haber hecho la integración del Req como el Siguiente cuadro:
![image](https://user-images.githubusercontent.com/61068392/160202256-01e84c97-48a0-4866-a7cf-b5c82f22b039.png)

*   Observación; Explicación de lo que se arregló o mejoró.
*   ### **Generar Objetos**: Tener mucho cuidado, porque le saldrá una advertencia, donde le pedirá confirmación para generar el Número de Req para la instalación.

![image](https://user-images.githubusercontent.com/61068392/160204112-2c32288e-5954-4eef-8b3c-155005375d3d.png)
¡Debe darle en si!
`Lo que hace es ir a buscarme en el proyecto asociado al Req y va a traer los objetos que tienen que ver con el Req`.

*   El le genera unos check button que dice si lo va a enviar, dar al botón Env para marcar todos.
*   Scripts de la instalación: se Coloca el nombre del script y las observaciones de lo que hay en el script.
*   ### **Datos para Pruebas**:
    *   `Carpeta de Desarrollo:` Donde se encuentra la carpeta en el Zeus
    *   `URL de Repositorio:` Las Rutas de URL que se Utilizan en el SVN
    *   `Carpeta de Repositorio:` La carpeta donde se encuentra el Req para las pruebas
        *   Solo para CELSIA diligenciar carpeta de Pru (Pruebas), si es otro cualquier caso se diligenciará: N\A
    *   Ruta en el Menú: Ruta del menú dentro del SAC
    *   Observaciones: Es el paso a paso de lo que se debe hacer, sale del proyecto en `Escenarios de Uso`.
    ![image](https://user-images.githubusercontent.com/61068392/160208141-d8d1a635-026e-4898-902e-87e656df0090.png)

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **FI-14**
Nos saldrá una advertencia.
*  Si le damos si, nos generará un FI-14 que solo se usa para Roadmap, una hoja por cada objeto
*  `No` para todo en una sola Hoja, Nosotros siempre le damos en NO
![image](https://user-images.githubusercontent.com/61068392/160208355-b4a0da4e-62db-42db-9b75-0bc4210b417b.png)
Luego le damos en generar Reporte
![image](https://user-images.githubusercontent.com/61068392/160504787-8af028d7-8b67-4a83-9a58-3570204d4528.png)
Generalmente se guarda en C:/Listados
Le cambiamos el nombre del archivo con el siguiente formato
```
FI-14 Registro de Instalación 2022-03-25-01_74981 >>>> Nombre del FI-14 (Cambia fecha_#RQ al final)
```

Luego entramos al archivo y quitamos lo que no se necesita, ponemos en color negro y sin cursiva en los objetos, se acomoda el ancho, quitar texto de la primera fila y primer col.

En Condiciones Generales poner el Siguiente Formato:
```
Ejecutar los script en HORARIO NO LABORAL, con los usuarios de la nomenclatura de cada script, en el orden que lo indique el número ubicado antes del tipo
de script.
"Ejecutar el script ###.sql con usuario SAC.
"Ejecutar el script #sql con usuario GEN.
                                                                                          
Mover los ejecutables de las formas a su respectiva ubicación: .\EXE\FMX\
Mover los ejecutables de las ayudas en línea de las formas a su respectiva ubicación: ..NEXEVHLPI
Mover los ejecutables de los reportes Report a su respectiva ubicación: .NEXEIREPI
Mover los ejecutables de los reportes SQL a su respectiva ubicación: ..\EXEISQLI
Mover los ejecutables de las plantillas a su respectiva ubicación: ..NEXEVLSI
```

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Formatos**
*   Importante: Encoding in UTF-8
*   ### **¿Cuales se Wrap?**
    *   Ruta en el Teams: Si el PK se encuentra en la lista, debe ir Wrapped
    ```
    Equipos/SAC/General/Archivos/Paquetes con wrap.pdf
    ```
*   ### **Tipos de Instalación**:
    *   Nueva
    *   Complementaria: solo se envian losobjetos que van de más.
    *   Sustituyente: la anterior no aplica, etnonces debe tener en cuenta todos los objetos.

*   ### **Acciones a realizar**:
El estandar es que todas van para pruebas
    *   Prueba
    *   Revisión: Ya hubo un ciclo de pruebas.
*  Errores
   *  Solo para CELSIA diligenciar carpeta de Pru (Pruebas), si es otro cualquier caso se diligenciará: N\A

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Duplicación de Instalaciones**
¿Qué se necesita?
*  El Req Origen (Generalmente un Req ACTSIS) este en está D : para Envio que halla pasado por la parte de soporte

1. Empresa: cick derecho para elegir la empresa.
2. Contrato: El contrato que corresponde
3. Proyecto: va ligado al contrato
4. Proyecto ID: Tenemos que colocar el proyecto donde cae el Req por ejemplo `(Actualización del mes de octubre para la ESSA)`

![image](https://user-images.githubusercontent.com/61068392/160473864-14ea949f-62b1-4c71-a248-e930fc712262.png)


#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Paso a Paso**
1. Buscar el Requerimiento
2. Revisar si el Requerimiento se encuentra en estado `T :Tramite` ya asociado al proyecto
3. Revisar que las casillas ya estén diligenciadas.
4. Revisar en Diseño de objetos que todas las modificaciones tengan la versión base a excepción de los objetos nuevos.
5. Revisar si el Req interno ya cuenta con una aprovación (Los 3 chulitos)
6. Despues de verificar lo anterior, tenemos que poner el estado del Req en `G :Integración` a nombre de la Ing. Liliana por ejemplo y la fecha fin estado.
7. Volvemos otra vez al botón de Py
8. Revisar a nivel de carpeta:
   *  En Obd tener todos los objetos que se tocaron [¿Cuales se Wrapean?](#cuales-se-wrap)
   *  Tener encuenta que la decodificacion debe estar en UTF-8
9. Despues debemos ir al botón de Instalaciones estando parado en el Requerimiento
10. Nos paramos en instlaciones y damos `F6` para agregar un nuevo registro
   *  En empresa la cual le vamos a hacer la instalación
   *  Poner el tipo de instalación [Tipos de Instalación](#Tipos-de-Instalación)
   *  Acción: se definen las [Acciones a realizar](#Acciones-a-realizar)
   *  Envio Cliente?: es muy importante principalmente para Paula que es la que hace los despliegues, para ella poder meter el Req a despliegue, se supone que está casilla debe estar desmarcada, si está marcada quiere decir que la estoy enviando directa
   *  El responsable de la instalación
   *  Tab ....
11. Los pre Requisitos se los da la persona que le mandó a que hiciera la instalación.
12. En observación: va un texto que indique está instalacion cual es la parte funcional de está instalación. `F10`
13. `F7` Y `F8`
14. Ya le genera numero de instalación (Anotar ese número de instalación)
15. Despues le damos al Botón + que está en Requerimientos de la Instalación
![image](https://user-images.githubusercontent.com/61068392/160503429-e0cfabf9-7c42-4c3f-843c-87b6f44adca7.png)
Aquí deberia salirme el numero del Req, lo marcamos y damos en ACEPTAR, si no me sale es porque faltó ponerlo en `G :Integración`.
16. Dar clicl en el botón generar Objetos [Generar Objetos](#Generar-Objetos)
17. Marcar todos los bojetos en Enviar
18. Luego ponemos los Scripts de la instalación que está dentro de la Carpeta del Req/Exe/Scr Ejemplo: `\\zeus\ACTSIS\ACTSIS\SAC\Des\75010\Exe\Scr` y en observación ponemos lo que tiene el script y el responsable del script por ejemplo "68918_01_01_WGR_O_SAC.sal > Script de Objetos de SAC"
"
19. Despues le damos en Datos para Pruebas [Datos para Pruebas](#Datos-para-Pruebas), cerrar y dar `F10`.
20. Creamos dentro de la Carpeta del Req/App/Doc la Revisión de integración.
21. [FI-14](#FI-14)
22. Luego hacemos el correo
Ruta del archivo en Teams
```
SAC>Despliesuges SACNNET>Archvios>INFORME_CAMBIOS.XLSX
```


#
[🔝 Volver al índice](#índice-de-contenido)
#
