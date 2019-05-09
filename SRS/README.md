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

  ## Elicitación
   * En la App de celulares la función principal que deberá de tener será ordenar a domicilio de las diferentes sucursales de la ciudad  y que los clientes puedan crear una cuenta para saber su nombre y dirección.
  
  * En la App se encontrara el menú de SubWay incluyendo la información de los sub del día.
  
  * También se deberá encontrar información en la App de las sucursales que estén en la ciudad y la información de contacto de cada sucursal.
  
  * El sistema de la empresa debera de contar con lo siguiente:
     1. registro de entrada y salida de cada empleado.
     2. recibir las ordenes que hagan los clientes desde la App movil y dirección para entregar cada orden.
     3. guardar todas las ordenes echas por los clientes.
     
Los puntos anteriores se obtuvieron en una entrevista realizada a un gerente de SubWay, después de escuchar los puntos del gerente se acordó que la App para móviles tendrá la función principal de ordenar a domicilio además de contar con información básica como: menú, sucursales, información de contacto, etc.
 En el sistema que se desarrollara para la empresa se llegó al acuerdo de que cada empleado, administrativo y jefe tendrán su propia cuenta en la que se registrara las horas de trabajo. Este sistema recibira las ordenes detalladas de cada cliente y estará conectado a una base de datos en la que registrara las órdenes vendidas y las horas trabajadas de los empleados, a esta base de datos solo tendrá acceso el jefe de la sucursal y los administrativos.

     
     

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
   
   ### Requerimientos específicos
   En esta sección se encontraran a detalle los requerimientos específicos del sistema a desarrollar.
   
   ### Interfaz
   
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
    
    
 ### Requirimiento No funcionales
  1. El requerimiento más importante que el sistema va a tener es la estabilidad, ya que si el producto final no es estable tiene el riesgo de cambiar o dañar los pedidos de los clientes y esto afectaría a la empresa y al cliente.
   
   2. La documentación es necesaria para que el usuario sea capaz de resolver sus dudas, las dudas de los usuarios surgirán mientras estén usando el nuevo sistema. La documentación debe ser completa pero no tan extensa para que el usuario le sea facil entenderla y le sea de utilidad.
   
   3. Seguridad para todos los usuarios, al momento de la especificación de usuario y contraseña, se necesita que el sistema cuenta con seguridad para resguardar todos esos datos.
   
   4. Mantenimiento cada cierto tiempo al software.

  

  
   
   
   
   
   
   
  
