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
    
  * Sub: sándwiches 
  * Sub del día: Cada dia de la seman tiene un sub en oferta
  
  
  ## Referencias
  ## Overview
# Overall Description

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

  ### Restricciones
   La única opción de paga que tiene el cliente es mediante una tarjeta de débito o crédito, desde la App no se podrá ordenar para pagar en efectivo.
   El usuario tendrá que crear una cuenta para poder ordenar desde la App, al crear la cuenta se le pedirá nombre y número de teléfono, esta información se mostrara en el sistema de la empresa para tener contacto con el cliente
   
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
  Se mostrara el precio de cada producto y un precio total del pedido, en la parte inferior estará la ventana para introducir los datos de la tarjeta de crédito o débito para proceder con la compra.
  
  
  ### Interfaz Empresa
  
  * **Empleados:**
  Se mostrara en forma de lista cada pedido que se genere, al seleccionar un pedido se mostrara la orden a detalle y la información del cliente, una vez terminen la orden podrán eliminar la orden de la lista.
  
  * **Repartidor:**
 Cada repartidor tendrá su cuenta para acceder a la App y poder ver las direcciones de los pedidos que debe entregar
 
 * **Dueño: **
El dueño tendrá acceso a la base de datos donde se mostrara el total de productos vendidos.   
  
   
   
   
   
   
   
  
