# Ciclo de Instalación

## Índice de contenido

*   [Definición](#definición)
*   [Instalación](#Instalación)
*   [Formatos](#Formatos)

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
*   Generar Objetos: Tener mucho cuidado, porque le saldrá una advertencia, donde le pedirá confirmación para generar el Número de Req para la instalación.

![image](https://user-images.githubusercontent.com/61068392/160204112-2c32288e-5954-4eef-8b3c-155005375d3d.png)
¡Debe darle en si!
`Lo que hace es ir a buscarme en el proyecto asociado al Req y va a traer los objetos que tienen que ver con el Req`.

*   El le genera unos check button que dice si lo va a enviar, dar al botón Env para marcar todos.
*   Scripts de la instalación: se Coloca el nombre del script y las observaciones de lo que hay en el script.
*   Datos para Pruebas:
    *   `Carpeta de Desarrollo:` Donde se encuentra la carpeta en el Zeus
    *   `URL de Repositorio:` Las Rutas de URL que se Utilizan en el SVN
    *   `Carpeta de Repositorio:` La carpeta donde se encuentra el Req para las pruebas
    *   Ruta en el Menú: Ruta del menú dentro del SAC
    *   Observaciones: Es el paso a paso de lo que se debe hacer, sale del proyecto en `Escenarios de Uso`.
    ![image](https://user-images.githubusercontent.com/61068392/160208141-d8d1a635-026e-4898-902e-87e656df0090.png)

#
[🔝 Volver al índice](#índice-de-contenido)
#

### **Formatos**
*   Importante: Encoding in UTF-8
*   ¿Cuales se Wrap?
    *   Ruta en el Teams: Si el PK se encuentra en la lista, debe ir Wrapped
    ```
    Equipos/SAC/General/Archivos/Paquetes con wrap.pdf
    ```
*   Tipos de Instlación:
    *   Nueva
    *   Complementaria: solo se envian losobjetos que van de más.
    *   Sustituyente: la anterior no aplica, etnonces debe tener en cuenta todos los objetos.
#
[🔝 Volver al índice](#índice-de-contenido)
#

