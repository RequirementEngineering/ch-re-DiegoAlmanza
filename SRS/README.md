 - [Table of contents and index](#Table-of-contents-and-index)
 - [Introducción](#Introducción)
    - [Propósito](#Propósito)
    - [Alcance](#Alcance)
    - [Definiciones, acrónimos y abreviaturas.](#Definiciones-,-acrónimos-y-abreviaturas.)
    - [Referencias](#Referencias)
 - [Descripción general](#Descripción-general)
    - [Perspectiva del producto](#Perspectiva-del-producto)
    - [Caracteristicas del usuario](#Caracteristicas-del-usuario)
 - [Suposiciones y dependencias](#Suposiciones-y-dependencias)
 - [Requerimientos](#Requerimientos)
    - [Requerimientos de sistema](#Requerimientos-de-sistema)
    - [Requerimientos funcionales](#Requerimientos-funcionales)
      - [Caso de uso general](#Caso-de-uso-general)
      - [Caso de uso especifico 1](#Caso-de-uso-especifico-1)
      - [Caso de uso especifico 2](#Caso-de-uso-especifico-2)
      - [Caso de uso especifico 3](#Caso-de-uso-especifico-3)
      - [Caso de uso especifico 4](#Caso-de-uso-especifico-4)
      - [Caso de uso especifico 5](#Caso-de-uso-especifico-5)
      - [Caso de uso especifico 6](#Caso-de-uso-especifico-6)
     
    - [Requerimientos No funcionales](#Requerimientos-No-funcionales)
  - [Appendixes](#Appendixes)
      - [Elicitación](#Elicitación)
      - [BPM](#BPM)
    
    
      
    


# Introducción 
  ## Propósito
   
   El presente documento tiene como proposito definir todos los requerimientos del sistema para la implementación de una aplicación para móviles que permitirá ordenar a domicilio de las diferentes sucursales de la cadena de restaurantes SubWay, esto con el fin de facilitar el proceso de servicio a domicilio de la empresa.
   Tambien se entregara un sistema para la empresa en la cual se recibiran todos los pedidos que se hagan desde la app y la direccion a donde se entregara el pedido.
    
   En el documento se analizaran los requerimientos del cliente, se describirá el plan de acción para desarrollar la aplicación móvil, se presentara la interfaz de la app y una interfaz para el sistema de la empresa para recibir los pedidos.      
  
  ## Alcance  
  El producto final constara de dos sistemas: 
  
 * SubWay APP será una App para móviles que será desarrollada en Java, en esta App se podrá ordenar a domicilio cualquier cosa del menú de las diferentes sucursales de la cadena de comida rápida SubWay. 
  
  * Un sistema para empleados de la empresa para recibir todos los pedidos especificados, dirección para entregar el pedido e información de contacto con el cliente en caso de dudas. Este sistema se conectara a una base de datos para tener información de cuantos productos vendió la sucursal.
 
      
  ## Definiciones, acrónimos y abreviaturas.
  * SubWay:  cadena de restaurantes de comida rápida especializada en la elaboración de sándwich submarino, bocadillos y ensaladas.   
  * Sub: sándwiches 
  * Sub del día: Cada dia de la seman tiene un sub en oferta
  * App: Aplicación
  
  ## Referencias
  * https://www.subway.com/es-MX/MenuNutrition/Menu/All

# Descripción general


  ## Perspectiva del producto
  La finalidad del producto es facilitar el servicio a domiciliio de la empresa, el producto sera una aplicación móvil que funcionara en smartphones en la cual se podara ordenar lo siguiente:
 
   •sándwiches


   •ensaladas 


   •desayunos 


  •bebidas  


  •extras 


tambien se podra encontrar la siguiente informacion: 

  •diferentes sucursales de la ciudad donde estes ubicado


  •puntos de entrega 


  •Sub del día


  •información de contacto  


  •promociones nacionales


  •Servicio de facturación

  La app funcionara en los sistemas operativos ios y android, se descargara de las tiendas virtuales de cada sistema operativo y sera de manera gratuita para los usuarios.
  
  ### Caracteristicas del usuario
 En total existirán cinco tipos de usuarios que van a interactuar con los sistemas:
   1. **Cliente:**
      El cliente usará la App desde su celular para ordenar de la sucursal de su preferencia, el usuario podrá ordenar cualquier cosa que esté disponible en el menú de SubWay a su domicilio.
   2. **Cajero:**
      El cajero recibirá una notificación cuando llegue un pedido e informara al cocinero de la orden. Cuando el cocinero termine de preparar la orden, el cajero se encargara de generar el ticket del pedido y entregárselo al repartidor.  
   3. **Cocinero:**
      El cocinero se encargara de revisar la orden y prepararla, una vez termine de preparar la orden se la entregará al cajero.
   4. **Repartidor:**
        El repartidor entregará la orden al cliente y tendrá la información de contacto (Dirección, Nombre del cliente y teléfono) en la App. 
   5. **Dueño:**
      El dueño tendrá acceso a la base de datos que genere el sistema para estar informado del total de ventas en el día y un inventario.
   6. **Administrativo:**
      Al igual que el dueño tendrán acceso a la base de datos y la información de las horas trabajadas de cada empleado.
   
   ### Suposiciones y dependencias
   Para el funcionamiento completo de SubWay App es necesario tener conexion a internet y se recomiendan los siguientes sistemas operativos:
   * En android: sistema operativo android 4.0 o superior. 
   * En Iphone: Ios 10 o superior.
   
   ### Requerimientos
   En esta sección se encontraran a detalle los requerimientos específicos del sistema a desarrollar.
   
   ### Requerimientos de sistema
   
   ### Interfaz Cliente
   La interfaz de la App para los clientes deberá ser intuitiva de manera que, sin un manual el usuario pueda ininteractuar de manera sencilla con la aplicación. La interfaz a demas deberá contar con los colores caracteristicos de SubWay los cuales son verde y amarillio. 
   * **Mensaje de Bienvenida:**
   Al abrir la App se mostrara un mensaje de bienvenida y se mostrara en pantalla el logo de subway.
   
   * En la parte superior central estará el logo de SubWay
   
   * En la parte superior izquierda estará la opción para que el usuario ingrese a su cuenta o cree su cuenta
   
   * **Informacion:**
   En esta opcion se encontrara:
   
  1. diferentes sucursales de la ciudad donde estes ubicado.

  2. Sub del día

  3. Información de contacto  

  4. Promociones nacionales

   * **Ordenar:** 
  Esta será la opción principal y será la más grande, si se selecciona esta opción se preguntara que desea ordenar y se le mostrara el menú. En un costado de cada opción del menú el usuario podrá escoger la cantidad deseada de cada producto.
   
   * Escoger los ingredientes
   Una vez seleccionado los productos y las cantidades empezara el proceso de preparación:
   
   1. Tipo de Sub: Se mostraran todos los tipos de sándwich 
   
   2. Tipo de pan: Se mostraran en lista los diferentes tipos de pan
   
   3. Escoger vegetales: Se mostrara una imagen de cada vegetal y se pedirá al usuario que seleccione que vegetales quiere en su Sub.
   
   4. Escoger líquidos: Se mostrara una imagen de cada líquido disponible y se pedirá al usuario que seleccione que líquidos quiere en su Sub.
   
   5. Escoger extras: Se preguntara al usuario si desea agregar extras a su Sub, si el usuario acepta agregar extras se mostrara una imagen de cada ingrediente extra disponible y se pedirá al usuario que seleccione los extras que quiere en su sub

  * Paga de pedido:
  Se mostrara el precio de cada producto y un precio total del pedido, en la parte inferior se encontraran dos opciones de pago efectivo y tarjeta de crédito, si se escoge con tarjeta de crédito aparecerá la ventana para introducir los datos de la tarjeta de crédito o débito para proceder con la compra.
  
  
  ### Interfaz Empresa
  
  * **Empleados:**
  Se mostrara en forma de lista cada pedido que se genere, al seleccionar un pedido se mostrara la orden a detalle y la información del cliente, una vez terminen la orden podrán eliminar la orden de la lista.
  
  * **Repartidor:**
 Cada repartidor tendrá su cuenta para acceder a la App y poder una lista de órdenes que debe entregar, información del cliente y los detalles del pedido, cuando el repartidor entregue la orden podrá eliminar la orden de la lista entregas.  
 
 * **Dueño:**
El dueño tendrá acceso a la base de datos donde se mostrara a detalle el total de órdenes que se vendieron cada día y los detalles de cada orden.

* **Administrador:**
El Administrador se le mostrara una base de datos con las horas de trabajo de cada empleado y una base de datos con las órdenes vendidas cada día y los detalles de cada una.


### Requerimientos funcionales
* Cliente:
    1. Inicio de sesión.

    2. Ordenar del menú de SubWay a domicilio.

    4. Consultar la información general de SubWay (Sucursales, Contacto, Ofertas, Facturación).
    
    
 * Empresa:
    1. Inicio de sesión.
    
    2. Sistema de empleados para recibir en lista las ordenes de los clientes y la información de contacto del cliente.
    
    3. Base de datos en la que se mostraran todas las órdenes vendidas, los detalles de cada orden y el total de cada producto vendido.
    
    4. Base de datos en la que se mostraran las horas trabajadas de cada empleado. 
    
    5. Cuentas especiales para el uso de los repartidores, en estas cuentas el repartidor encontrara lo necesario para realizar las entregas de los pedidos 
    
 ## Caso de uso general
   <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/SubWay%20app%20caso%20de%20uso%20(1).png" height=50% width=50%></img></p>
   
  Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |La funcion principal del sistema sera ordenar a domicilio de las tiendas SubWay desde una app para moviles, el sistema tambien contara con una base de datos para guardar las horas de trabajo de los empleados, ventas e inventario.
 Actores | Empleados, Cliente y dueño
 Condiciones | Tener una cuenta creada.
 Flujo| Cliente .- Iniciar sesion, Ordenar. Cajero.- Iniciar sesion, Registrar hora de entrada y salida, Recibir Orden, Cobrar Orden. Cocinero .- Iniciar sesion, Registrar hora de entrada y salida, Cocinar orden.  Repartidor.- Iniciar sesion, Registrar hora de entrada y salida, Recoger orden, entregar Orden, Cobrar Orden. Dueño.- acceso a la base de datos.

  ## Caso de uso especifico 1
  <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/EMIS.png"></img></p>
  
 Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |Cuando los empleados inicien sesion se registrara la hora de entrada y al cerrarla la hora de salida en la base de datos, se guardara informacion basica del empleado y un ID para identificar cada empleado.
 Actores | Cajero, Cocinero y Repartidor.
 Condiciones | Tener una cuenta creada.
 Flujo| Ingresar ID y la contraseña para ingresar, una vez en la cuuenta el cajero recibira las ordenes de los clientes.
 
  ## Caso de uso especifico 2
  <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/CAOR.png"></img></p>
  
 Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |El cajero recibe la orden en el sistema, después notificara al cocinero para que este proceda a preparar la orden, una vez terminada la orden el cajero la cobrara y se la entregara al repartidor.
 Actores | Cajero, Cocinero y Repartidor.
 Condiciones | Tener los ingredientes para la orden.
 Flujo| Recibir orede, prepar la orden y entregarla a domicilio.
 
  ## Caso de uso especifico 3
  <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/CLIS.png"></img></p>
  
 Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |El cliente iniciara sesión para poder ordenar.
 Actores | Cliente.
 Condiciones | Tener cuenta creada.
 Flujo| ingresar nombre de usuario y contraseña.
 
 ## Caso de uso especifico 4
 <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/CLOR.png"></img></p>
 
 Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |El cliente creara su orden y despues de confirmar la orden sera enviada al sistema de los empleados.
 Actores | Cliente.
 Condiciones | Tener cuenta creada.
 Flujo| El usuario ingresara a su cuenta y creara su orden a gusto personal escogiendo los tipos de sub y los ingredientes que estos llevara.
   
 ## Caso de uso especifico 5
 <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/COOR.png"></img></p>
 
 Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |El cocinero preparara la orden del cliente
 Actores | Cajero, Cocinero y Cliente.
 Condiciones | Tener los ingredientes necesarios para preparar la orden.
 Flujo|El cajero recibe la orden del cliente y se le notifica al cocinero, el cocinero revisa la orden y la prepara.
 
 ## Caso de uso especifico 6
 <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/DUBA.png"></img></p>
 
 Usuario  | Descripcion
 ----- | -------------
 Nombre | SubWay App
 Autor | Diego Almanza Beyless
 Fecha | 25/04/2019
 Descripción |El Dueño tendra acceso a la base de datos.
 Actores | Dueño.
 Condiciones | Tener cuenta para acceder a la base de datos.
 Flujo|El dueño ingresa a su cuenta y encontrara la base de datos con la informacion de ventas y horas trabajadas de los empleados.
 
 ### Requerimientos No funcionales
  1. El requerimiento más importante que el sistema va a tener es la estabilidad, ya que si el producto final no es estable tiene el riesgo de cambiar o dañar los pedidos de los clientes y esto afectaría a la empresa y al cliente.
   
   2. La documentación es necesaria para que el usuario sea capaz de resolver sus dudas, las dudas de los usuarios surgirán mientras estén usando el nuevo sistema. La documentación debe ser completa pero no tan extensa para que el usuario le sea facil entenderla y le sea de utilidad.
   
   3. Seguridad para todos los usuarios, al momento de la especificación de usuario y contraseña, se necesita que el sistema cuenta con seguridad para resguardar todos esos datos.
   
   4. Mantenimiento cada cierto tiempo al software.

  ## Appendixes
  ## Elicitación
  
   * El proceso de preparacion de los Sub es:
     1. Ordenar los tipos de Sub.
     2. Seleccionar los tipos de pan.
     3. Seleccionar tipo de queso.
     4. Escoger entre frio, caliente o tostado.
     5. Escoger vegetales.
     6. Escoger liquidos.
     7. Escoger extras.
  
   * En la App de celulares la función principal que deberá de tener será ordenar a domicilio de las diferentes sucursales de la ciudad  y que los clientes puedan crear una cuenta para saber su nombre y dirección.
  
  * En la App se encontrara el menú de SubWay incluyendo la información de los sub del día.
  
  * También se deberá encontrar información en la App de las sucursales que estén en la ciudad y la información de contacto de cada sucursal.
  
  * El sistema de la empresa debera de contar con lo siguiente:
     1. registro de entrada y salida de cada empleado.
     2. recibir las ordenes que hagan los clientes desde la App movil y dirección para entregar cada orden.
     3. guardar todas las ordenes echas por los clientes.
     
Los puntos anteriores se obtuvieron en una entrevista realizada a un gerente de SubWay, después de escuchar los puntos del gerente se acordó que la App para móviles tendrá la función principal de ordenar a domicilio además de contar con información básica como: menú, sucursales, información de contacto, etc.
 En el sistema que se desarrollara para la empresa se llegó al acuerdo de que cada empleado, administrativo y jefe tendrán su propia cuenta en la que se registrara las horas de trabajo. Este sistema recibira las ordenes detalladas de cada cliente y estará conectado a una base de datos en la que registrara las órdenes vendidas y las horas trabajadas de los empleados, a esta base de datos solo tendrá acceso el jefe de la sucursal y los administrativos.
  ## BPM
  <p align="center"><img src="https://github.com/RequirementEngineering/ch-re-DiegoAlmanza/blob/master/SRS/Caso%20de%20uso/bpm%20Subway/Business%20Process%20Diagram1.jpg" height=70% width=70%></img></p>
  ## Proceso 1
 * El evento principal inicia con el cliente iniciando sesión.
  * El sistema detecta si tiene cuenta o no, si el usuario no tiene cuenta se crea un sub proceso para crear una cuenta.
  * Cuando el usuario ingrese podrá ordenar, cuando se confirme la orden el cajero la recibirá y le notificara al cocinero la orden.
  * El cocinero prepara la orden en un tiempo estimado de 15 minutos y le entregara la orden al cajero 
  * El cajero cobrara la orden y genera el ticket, después le entregara la orden al repartidor.
  
  * El repartidor llevara la orden en un tiempo estimado de 30 minutos al domicilio del cliente.
   * Si el cliente paga con tarjeta de crédito se abre el sub proceso para paga con tarjeta de crédito.
  * El cliente pagara la orden, si la paga es en efectivo le entrega el dinero al repartidor y el repartidor le entregara la orden al cliente.
  * Fin de proceso.

  
  ## Proceso 2
 * El evento de registro de horas de trabajo comienza con los empleados iniciando sesión.
  * El sistema detecta si tiene cuenta o no, si el usuario no tiene cuenta se crea un sub proceso para crear una cuenta.
  * El administrativo creara la cuenta del nuevo empleado.
  * El empleado registrara sus horas de entrada y de salida.
  * El sistema guardara las horas trabajadas de cada empleado en la base de datos.
  * El administrativo tendrá acceso a la base de datos para conocer las horas trabajadas de cada empleado.
  * Fin de proceso


 
   
   
   
   
   
  
