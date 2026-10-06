# GroStop- Un sitio web de comercio electrónico para una tienda de abarrotes usando Flask
Hemos incorporado la base de datos en forma de una aplicación en la que hemos intentado asemejarla a un sitio web de comercio electrónico en funcionamiento, donde los usuarios, vendedores y administradores pueden trabajar como deseen en una plataforma de la vida real. Hemos creado el Front-end para habilitar la interfaz y la experiencia de usuario de la mejor manera posible. Aquí nuestros usuarios pueden interactuar realmente con nuestro sitio web y realizar los cambios que deseen según su alcance en el proyecto. Va desde la compra y venta para usuarios, hasta la realización de cambios para administradores y para que los vendedores vendan sus productos. También permite que el sitio funcione con todas las restricciones necesarias para establecer un sitio de comercio electrónico real. Hemos conectado la base de datos a nuestro sitio web actual, el cual mantiene el registro en consecuencia: si hacemos algún cambio básico, ocurre algún cambio en nuestra base de datos.

## El Equipo
Todos nosotros somos estudiantes de licenciatura en Ciencias de la Computación en `IIIT Delhi`
- Vibhor Agarwal
- Anshak Goel
- Pritish Poswal
- Deeptorshi Mondal

## Reporte del Proyecto
Aquí encontrarás el [`Reporte`](https://drive.google.com/file/d/1gwSO9Enmp2_QrMFgUFrtEVAthKgwKdty/view?usp=sharing) más detallado que jamás obtendrás. Tiene hasta los detalles más minúsculos de nuestro proyecto.
La carpeta `submit` contiene el reporte del proyecto, varias `Consultas SQL` y `Triggers SQL`.

## Tecnologías Utilizadas
- `Frontend` - HTML, CSS, Bootstrap 5, Jinja Template.
- `Backend` - Python, Flask, Base de Datos MySQL.
- Hemos poblado nuestra base de datos con una cantidad real y considerable de datos para probar el sitio web correctamente. Se ha tenido el máximo cuidado con la coherencia de los datos.
- Se han mantenido las entidades adecuadas en nuestro [Diagrama ER](https://drive.google.com/file/d/1gwWgqiIbi1ccUUxpN0GYY3s55nHbmFaf/view?usp=sharing) y 
[Diagrama Relacional](https://drive.google.com/file/d/1oxjCmVsO1gFkM2QC8il61GxXf2bP8CS7/view?usp=share_link)

![image](https://user-images.githubusercontent.com/76804249/189937796-1c29cdbc-a151-4b2a-a95f-8d3744407aa2.png)

Elegimos `Flask` como nuestro backend porque necesitábamos que el sitio web estuviera funcionando lo más rápido posible para alinearse con nuestro cronograma del proyecto. También elegimos `MySQL` como nuestra base de datos porque estábamos trabajando con ella en nuestro curso de DBMS en la licenciatura.

## Pasos para desplegar el sitio web
- Primero clona este repositorio
- Luego abre la carpeta clonada
- Ahora necesitamos restaurar la base de datos desde el dump.
- Abre la consola de comandos (CMD) en la carpeta actual y ejecuta el siguiente comando:

- - Ahora crea un entorno virtual usando el siguiente comando:

py -m venv online_store

- Ahora activa este entorno ejecutando `.\online_store\Scripts\Activate.ps1`
- Ahora necesitamos instalar los requisitos del proyecto. Ejecuta el siguiente comando:

- pip install -r .\requirements.txt

 - Esto completa el proceso de configuración para ejecutar el sitio web. Simplemente ejecútalo ejecutando el archivo `run.py`

# Demostración del sitio web

## Pantalla de Inicio de Sesión
En primer lugar, cuando abrimos el sitio web se nos muestra la pantalla de inicio de sesión.
- Se nos presentan tres opciones:
 - Usar como Administrador
 - Usar como Vendedor
 - Usar como Cliente
 
 ![image](https://user-images.githubusercontent.com/76804249/189930307-1b589e67-6929-42bd-8f95-26791a563861.png)

- A cada rol se le da la opción de Registrarse o Iniciar Sesión.

![image](https://user-images.githubusercontent.com/76804249/189930533-d9417030-12ad-4fdb-b8cb-cbc4b78153d8.png)

- Si el usuario elige iniciar sesión, mostramos el formulario de autenticación.

![image](https://user-images.githubusercontent.com/76804249/189930682-974ad142-c7c0-4bb3-b0b4-297e8048315e.png)

- Si la contraseña ingresada es incorrecta, mostramos el error; de lo contrario, iniciamos la sesión del usuario.

![image](https://user-images.githubusercontent.com/76804249/189930896-cb75eb5f-fa21-4806-ab96-5387abed6f79.png)

- Si el usuario no está registrado previamente, le pedimos los datos relevantes.

![image](https://user-images.githubusercontent.com/76804249/189931179-d0c77367-7732-4ec8-a270-895897884cb0.png)

## Pantalla de Compras
- Una vez que el usuario ha iniciado sesión con éxito, le mostramos la lista de productos.

![image](https://user-images.githubusercontent.com/76804249/189931991-7129528d-059b-4705-b36d-c0d7760f40e5.png)

- Tiene la opción de agregar el producto al carrito. Le damos una confirmación una vez agregado un producto con éxito.

![image](https://user-images.githubusercontent.com/76804249/189932723-824e8773-a96c-46f2-aebc-8fc5bb54e558.png)

- Luego puede ir al carrito y también aplicar un código de cupón.

![image](https://user-images.githubusercontent.com/76804249/189932935-66877493-52aa-4f86-91a0-8761e3af526a.png)

- A continuación, se muestra el precio incluyendo el descuento y se solicitan el pago y la dirección.

![image](https://user-images.githubusercontent.com/76804249/189933944-768e09ba-e38e-4cc1-a4f9-de2378fbce53.png)

- Luego le mostramos al usuario que el pedido se ha realizado con éxito.

![image](https://user-images.githubusercontent.com/76804249/189934185-e49aeae8-6b72-42b2-b92e-86e273146d43.png)

- Si iniciamos sesión como vendedor, podemos agregar productos al inventario.

![image](https://user-images.githubusercontent.com/76804249/189934713-7e24517d-8ac5-4497-b457-131eb59b256b.png)

- Si iniciamos sesión como Administrador del sitio web, podemos hacer múltiples cosas como se muestra:

![image](https://user-images.githubusercontent.com/76804249/189935135-bddd315f-13c5-4816-947d-738a44108e5a.png)

- Por ejemplo, agregar una nueva oferta:

![image](https://user-images.githubusercontent.com/76804249/189935575-259c4d78-50a2-4d58-9f5f-adb282dd0a03.png)


# Descripción Completa del Proyecto

## Alcance del Proyecto
Nuestro proyecto se ocupa de la creación y gestión de una tienda minorista en línea. En este proyecto nuestro objetivo principal es hacer un sistema de este tipo que ayude en el funcionamiento del sistema minorista en línea entre las partes interesadas involucradas. El alcance de nuestro proyecto se dirige principalmente a reducir la brecha entre las personas involucradas, como el vendedor, el cliente, la persona que lo administra y los repartidores. Tendríamos diferentes personas para desempeñar diferentes roles.
Aquí el Administrador, el Cliente y el Vendedor podrán iniciar sesión en una página.
Específicamente, primero tomamos al Administrador, quien manejaría muchas solicitudes y aseguraría el correcto funcionamiento entre las personas ajenas a la organización involucrada en el sistema. Tendría todos sus datos donde contaría con un nombre, ID y una contraseña. Podrá agregar vendedores que ofrezcan productos en el mercado y agregar esos productos al carrito con sus atributos. También podrá ver el producto. El Administrador también puede agregar un repartidor para entregar productos y tiene acceso para agregar ofertas para diferentes pedidos según su elegibilidad.
De manera similar, un vendedor que tenga su nombre, lugar de operación, contraseña, correo electrónico y número de teléfono podrá vender los productos fácilmente.
El producto vendido también tendría varios atributos donde el administrador y el cliente podrían ver su precio, nombre, marca, medida, unidad y también tendría un ID.
A continuación, tendríamos a un cliente que tendría nombre, contraseña, correo electrónico, número de teléfono móvil y también un ID, quien tendría la libertad de dar sus comentarios (feedback) sobre el producto y está asociado con la categoría y selecciona la categoría. El cliente ahora tiene el poder de dar una calificación al repartidor correspondiente a un pedido.
La Retroalimentación (Feedback) tendría un cuerpo para escribir los detalles, así como un ID para almacenarla. Contendría la fecha para ser agregada y también la puntuación para medirla.
Tendríamos Categorías que contienen el ID y el nombre para diferenciar, y los productos también se agregarían a un carrito que tiene el costo total y el valor agregado con su ID.
Finalmente, el carrito genera los pedidos para que finalmente se pueda proceder a la compra, donde el pedido tendría su ID, la dirección a la que se entrega, el método de pago y el monto a pagar. Tendría la fecha del pedido y también su hora. El carrito también tendría un valor final como atributo, el cual está presente después de aplicarle una oferta. Ahora las ofertas también se pueden aplicar en el carrito. La sección de pedidos también se asignaría a un repartidor en particular.
También tendríamos una sección de ofertas que se utiliza principalmente para aplicar descuentos especiales a todos los productos agregados. La oferta contendría un código de promoción, un ID de oferta, un descuento máximo, un valor mínimo y también un porcentaje de descuento.
Por último, tenemos un repartidor que realiza diferentes pedidos a lo largo del proceso. El repartidor tendría su contraseña, correo electrónico, número de teléfono, así como su calificación promedio. Tendría un ID y también un nombre con nombre de pila y apellido. Estaría asignado a un pedido.
En resumen, una persona podrá vender sus productos al cliente, donde el proceso será administrado por el administrador y el pedido será realizado por el repartidor. Contaría con todas las características agregadas para hacer el proceso más eficiente y fluido.
También hemos incluido Git para el control de versiones para garantizar que todos los miembros del equipo tengan la última versión de la base de datos con ellos. Actualizamos regularmente los dumps de la base de datos en Github.
Nuestro alcance final reside en identificar los productos, usuarios, administrador, pedidos, vendedores y repartidores, y mantener un ciclo e interacción adecuados entre todos.

## Partes Interesadas (Stakeholders) del Proyecto
Hay múltiples partes interesadas en este proyecto; el proyecto se centra principalmente en clientes y vendedores, junto con los cuales también tenemos al administrador y al repartidor como dos partes interesadas más. Los clientes son partes interesadas importantes que realizan operaciones como ver productos por categoría, agregar productos al carrito, realizar pedidos y dar comentarios sobre los productos. También pueden agregar una calificación al repartidor correspondiente a un pedido en particular.
Nuestra otra parte interesada, el vendedor, vende varios productos que compran los clientes.
Otra parte interesada aquí es el administrador, quien mantiene y agrega datos a nuestra base de datos para la tienda minorista en línea, como agregar productos y vendedores, además de poder ver los pedidos que los clientes han realizado para procesarlos. El Administrador también agrega al repartidor, mientras que el repartidor siempre es asignado a un pedido cuando este se realiza.

## Supuestos en el Proyecto
Hemos tomado las siguientes suposiciones en nuestro proyecto:
1. En primer lugar, hemos asumido que todos los pedidos pasarán por el carrito y cada pedido tendrá un carrito único con un ID de carrito único y estará asociado a un solo cliente. Además, cada cliente tendrá un solo carrito a la vez para realizar un pedido.
2. Solo un cliente puede agregar comentarios a un producto otorgando una reseña y una calificación a los productos.
3. Cada producto pertenecerá a una categoría única y no hay categorías que no tengan ningún producto.
4. El cliente también puede ver el producto directamente y puede verlo seleccionando esa categoría en particular.
5. Puede haber múltiples administradores y cada uno de ellos tiene el poder de agregar productos, categorías y vendedores.
6. Solo los administradores pueden ver los detalles de todos los pedidos realizados por diferentes clientes, mientras que un cliente solo puede ver su propio pedido.
7. Cada producto puede ser vendido por cualquiera de los múltiples vendedores y cada vendedor puede vender múltiples productos.
8. El vendedor solo puede saber la cantidad de productos de cada tipo que ha vendido.
9. También hemos asumido que cada carrito está asociado a un solo pedido y cada pedido está asociado a un solo carrito.
10. Se asume en este proyecto que todos los productos se venden al precio de venta sugerido (MRP) y no hay opción de descuento, código de cupón o reembolso. SUPOSICIÓN ELIMINADA.
11. Nos hemos asegurado de que las ofertas se realicen de acuerdo con un precio mínimo. Tendrían un descuento máximo y tendrían un porcentaje de descuento.
12. Un carrito solo puede tener una única oferta. Pero se puede hacer una sola oferta a múltiples carritos.
13. Solo un administrador puede agregar múltiples ofertas.
14. Solo un administrador puede agregar múltiples repartidores.
15. Se puede asignar un solo repartidor a múltiples pedidos.
16. Múltiples clientes pueden otorgar un valor de calificación particular a múltiples repartidores correspondientes a múltiples pedidos.
17. Un cliente solo puede agregar una calificación correspondiente a su propio pedido.

## Permisos (Grants) en el Proyecto
1 PERMISO PARA ADMINISTRADOR
grant select,insert,update,alter
on category
to 'Admin1';
grant select,insert,update,alter
on delivery_boy
to 'Admin1';
grant select,insert,update,alter
on offer
to 'Admin1';
grant select,insert,update,alter
on product
to 'Admin1';
grant select,insert,update,alter
on seller
to 'Admin1';
grant select
on orders
to 'Admin1';
grant select
on customer
to 'Admin1';
EXPLICACIÓN: Este es el permiso que se ha creado para el Administrador. El nombre de usuario del Administrador es “Admin1”, como se muestra en la consulta SQL anterior.
Como se vio anteriormente en este permiso, le hemos dado al administrador, que es “Admin1”, el privilegio de seleccionar, actualizar, insertar y alterar la entidad categoría según su elección.
De manera similar, el administrador tiene el privilegio de seleccionar, actualizar, insertar y alterar las entidades repartidor (delivery_boy), oferta (offer), producto (product) y vendedor (seller) según su elección.
En pedidos (orders), el administrador tiene el privilegio de solo seleccionar los pedidos otorgados por el cliente.
El Administrador tiene el privilegio de solo seleccionar un cliente también.

2 PERMISO PARA VENDEDOR
grant select,insert,update
on product
to 'Seller1','Seller2';
grant select
on orders
to 'Seller1','Seller2';
grant select
on offer
to 'Seller1','Seller2';
grant select
on sells
to 'Seller1','Seller2';
grant select
on category
to 'Seller1','Seller2';
EXPLICACIÓN: Este es el permiso que se ha creado para dos vendedores. Hay dos nombres de usuario para los dos vendedores, que son “Seller1” y “Seller2” respectivamente.
Como se vio anteriormente en este permiso, les hemos dado a ambos vendedores el privilegio de seleccionar, actualizar e insertar en la entidad producto según su elección.
Por el contrario, “Seller1” y “Seller2” tienen el privilegio de solo seleccionar las entidades pedidos (orders), oferta (offer) y categoría (category) como se indica en la base de datos.
Ambos vendedores también pueden seleccionar la tabla de relación vende (sells) presente en nuestra base de datos.

3 PERMISO PARA REPARTIDOR
grant select
on product
to 'Delivery_boy1','Delivery_boy2';
grant select
on orders
to 'Delivery_boy1','Delivery_boy2';
grant select
on offer
to 'Delivery_boy1','Delivery_boy2';
grant select
on product_feedback
to 'Delivery_boy1','Delivery_boy2';
grant select
on rates_order_delivery
to 'Delivery_boy1','Delivery_boy2';
EXPLICACIÓN: Este es el permiso que se ha creado para dos repartidores. Hay dos nombres de usuario para dos repartidores, que son “Delivery_boy1” y “Delivery_boy2” respectivamente.
Como se vio anteriormente en este permiso, les hemos dado a ambos repartidores el privilegio de SOLO seleccionar retroalimentación de productos (product_feedback), oferta (offer), pedidos (orders) y productos (product).
Ambos repartidores también pueden seleccionar la tabla de relación califica_pedido_entrega (rates_order_delivery) presente en nuestra base de datos.

## Entidades con su Clave Primaria
Hay numerosas entidades en el proyecto y a continuación se muestran sus claves:
Cliente (Customer): Es la persona principal involucrada en la compra de los productos que puede seleccionar la categoría y también brinda comentarios sobre los productos. También está asociado con el carrito para realizar los pedidos. El Cliente tiene un nombre, un correo electrónico, un número de teléfono y también se le ha asignado una contraseña. El cliente puede otorgar un valor de calificación a un repartidor correspondiente a un pedido en particular. Clave Foránea: N/A, CLAVE PRIMARIA: Customer_ID
Producto (Product): Este es el elemento que agrega el administrador, vende el vendedor y finalmente selecciona el cliente a través del usuario. Tendría el nombre, el ID y el precio. También tendría la marca, la unidad y la medida. Está asociado con el carrito y tiene una categoría. Clave Foránea: Category_ID, CLAVE PRIMARIA: Product_ID
Administrador (Admin): Es el trabajo del administrador agregar los productos y a la persona que los vende. El Administrador también puede ver cuáles son los pedidos. El Administrador puede agregar ofertas así como repartidores. El Administrador tiene un nombre, ID y una contraseña. Clave Foránea: Category_ID, CLAVE PRIMARIA: Admin_ID
Categoría (Category): Es básicamente la sección a la que pertenece el producto. Tendría el nombre de la categoría así como el ID de la categoría. El Administrador también puede ver cuáles son los pedidos. Tendría el nombre así como el ID. Clave Foránea: N/A, CLAVE PRIMARIA: Category_ID
Vendedor (Seller): La persona involucrada en la venta de los productos en la tienda. El vendedor es agregado por el administrador. El vendedor tendría su nombre y un ID. Se han almacenado los datos de contacto del vendedor y también su lugar de operación. También se le ha asignado una contraseña. Clave Foránea: Admin_ID, CLAVE PRIMARIA: Seller_ID.
Comentarios del Producto [ENTIDAD DÉBIL] (Product Feedback): Es la reseña y comentario otorgado por el cliente. Cada producto tendría comentarios. La Retroalimentación tendría un ID. También contendría la fecha en que se agrega. El producto también contendría la calificación y el cuerpo para determinar cuál es básicamente nuestra reseña. Clave Foránea: N/A, CLAVE PRIMARIA: Review_ID ∪ Product_ID
Pedidos (Orders): Esta es una de las entidades principales donde se realiza el pedido principal. Aquí los productos que se confirman finalmente se colocan en el sistema. Aquí el carrito finalmente realizará los pedidos. El pedido contendría el ID, la dirección de donde proviene. También tendría la hora y la fecha de su entrega. Uno también tendría la opción de elegir el método de pago y su monto. El pedido se asignaría a un repartidor mientras que, con respecto a un pedido en particular, a un repartidor se le otorgaría una calificación. Clave Foránea: Cart_ID, CLAVE PRIMARIA: Order_ID.
Carrito (Cart): Aquí se almacenan todos los pedidos del cliente. El carrito generará los pedidos. El carrito tendría el ID, la cantidad total de productos, así como las unidades totales que tiene cada producto. El carrito también tendría el monto final como atributo después de aplicar una oferta en particular. La oferta también se aplicaría al carrito. Clave Foránea: N/A, CLAVE PRIMARIA: Admin_ID
Oferta (Offer): Estas serán las ofertas que se aplicarán en función de cierta condición. Puede basarse en un precio mínimo aplicado al pedido. Estas ofertas otorgarán a los usuarios cierta cantidad, reduciendo así el costo del carrito. La oferta se aplicará únicamente al carrito. La oferta también tendrá un código de promoción. Entonces los atributos serían código de promoción, ID de oferta, descuento máximo, porcentaje de descuento y un valor mínimo de pedido. Clave Foránea: Admin_ID, CLAVE PRIMARIA: Offer_ID
Repartidor (Delivery_boy): Esta es la persona que entregará los pedidos al cliente. Sería agregado por el administrador y también estaría sujeto a una calificación por parte del cliente con respecto a un pedido en particular. Se le asignaría a un pedido. El repartidor tendría un nombre y un apellido. En forma de contacto, el repartidor tendría una dirección de correo electrónico y un número de teléfono móvil. Se le asignaría un ID y se le daría una calificación promedio y una contraseña. Clave Foránea: Admin_ID, CLAVE PRIMARIA: Delivery_Boy_ID

## RELACIONES ESTABLECIDAS, PARTICIPACIÓN DE ENTIDADES Y TIPOS DE RELACIÓN
Hemos construido muchas relaciones entre entidades aquí y a continuación se presenta una breve descripción de cada relación junto con la participación y el tipo:
1. cliente selecciona categoría: Aquí la relación entre cliente y categoría es de M a N, ya que cada cliente puede seleccionar múltiples categorías y cada categoría puede ser seleccionada por múltiples clientes. Aquí tanto el cliente como la categoría tienen una participación parcial, ya que no es necesario que cada cliente seleccione alguna categoría y tampoco es necesario que cada categoría sea seleccionada por algún cliente, por lo que la participación es parcial.
2. cliente da comentarios_del_producto: Aquí la relación entre cliente y comentarios_del_producto es de 1 a N, ya que sabemos que un cliente puede dar comentarios sobre varios productos, pero sabemos que un solo comentario de producto puede ser otorgado por un solo cliente. Aquí el cliente tiene una participación parcial ya que no es necesario que todos los clientes den comentarios sobre los productos, pero es necesario que cada comentario sea dado por algún cliente, por lo que los comentarios del producto tienen una participación completa. Aquí nuestro comentario de producto es una entidad débil y el tipo de relación es entre la entidad débil y la fuerte, por lo que era necesario que la entidad débil tuviera una participación completa.
3. categoría tiene producto: Aquí la relación entre categoría y producto es de 1 a N ya que cada categoría tiene múltiples productos, pero cada producto pertenece a una sola categoría. Aquí hay una participación completa de ambas partes (categoría y producto), ya que cada producto pertenece a alguna categoría y también aquí hemos asumido que cada categoría tiene al menos un producto.
4. producto tiene comentarios del producto: Aquí la relación entre producto y comentarios del producto es de 1 a N ya que cada producto tiene múltiples comentarios, pero un comentario del producto pertenece a un solo producto. Aquí hay una participación parcial por parte del producto ya que no todos los productos tienen comentarios, pero hay una participación completa por parte de los comentarios del producto ya que cada comentario está asociado con algún producto.
5. vendedor vende producto: Aquí la relación entre vendedor y producto es de M a N ya que cada producto puede ser vendido por múltiples vendedores y también cada vendedor puede vender múltiples productos. Aquí hay una participación completa tanto del vendedor como del producto porque cada vendedor vende algún producto y cada producto es vendido por algún vendedor.
6. administrador agrega vendedor: Aquí la relación entre administrador y vendedor es de 1 a N. Un administrador puede agregar múltiples vendedores, pero un vendedor solo puede ser agregado por un administrador. Aquí hay una participación parcial del administrador porque hemos asumido que no todos los administradores agregan vendedores; también hay una participación completa del vendedor ya que cada vendedor es agregado por algún administrador.
7. administrador agrega producto: Aquí la relación entre administrador y producto es de 1 a N. Un administrador puede agregar múltiples productos, pero un producto es agregado por un solo administrador. Hay una participación completa del producto porque cada producto es agregado por algún administrador, pero hay una participación parcial del administrador porque no todos los administradores agregan productos.
8. carrito realiza pedido: Aquí la relación entre carrito y pedido es de 1 a 1. Hemos asumido que un solo carrito puede realizar un solo pedido y un carrito realiza solo un pedido. Aquí hay una participación parcial del carrito porque no todos los carritos realizan un pedido, ya que algunos clientes pueden dejar algunos artículos en el carrito y no realizar un pedido, pero hay una participación completa del pedido porque cada pedido ha sido realizado por algún carrito.
9. administrador visualiza pedidos: Aquí la relación entre administrador y pedido es de M a N. Es de M a N ya que cada pedido puede ser visto por múltiples administradores y cada administrador puede ver múltiples pedidos. Aquí hay una participación parcial tanto del administrador como de los pedidos, ya que no todos los administradores ven algún pedido ni todos los pedidos son vistos por algún administrador.
10. cliente está asociado con producto y carrito: Esta es una relación ternaria en nuestra tienda minorista en línea.
Hablando de estas una por una, hemos tomado algunas suposiciones aquí:
 1. Entre cliente y carrito la relación es de uno a uno, tal como hemos asumido e implementado de tal manera que un cliente tendrá solo un carrito y un carrito estará relacionado con un solo cliente; aquí hay una participación parcial del cliente, ya que hemos asumido que no todos los clientes tienen un carrito, y hay una participación completa del carrito, ya que cada carrito está asociado con algún cliente.
 2. Entre producto y carrito la relación es de N a 1, ya que hemos asumido que un producto se puede agregar a un solo carrito a la vez para un usuario y un carrito puede tener múltiples productos. Hay una participación parcial del producto, ya que es posible que no todos los productos se agreguen al carrito, pero hay una participación completa del carrito, ya que hay 1 carrito único para un usuario, por lo que siempre tendrá un producto y participará.
 3. Entre cliente y producto la relación es de 1 a N, ya que hemos asumido que una persona puede agregar múltiples productos al carrito, pero un producto puede ser agregado al carrito por una sola persona a la vez. Hay una participación parcial tanto del cliente como del producto, ya que no todos los clientes agregan productos al carrito y no todos los productos son agregados al carrito por un cliente según nuestra implementación.
11. Oferta se Aplica a un Carrito:
Aquí la relación entre oferta y carrito es de 1 a N. Hemos asumido que un pedido se puede aplicar a múltiples carritos únicamente y solo 1 carrito puede tener solo 1 oferta. Aquí hay una participación parcial del carrito porque no todos los carritos tendrían una oferta, ya que es posible que no se aplique alguna oferta a un carrito y, por lo tanto, queden algunas ofertas sin aplicar, y hay una participación parcial de la oferta porque no todas las ofertas se pueden aplicar a los carritos, ya que no es necesario que se realice la oferta.
12. Administrador agrega oferta: Aquí la relación entre administrador u oferta es de 1 a N. Un administrador puede agregar múltiples ofertas, pero una oferta es agregada por un solo administrador. Hay una participación completa del producto/oferta porque cada oferta es agregada por algún administrador, pero hay una participación parcial del administrador porque no todos los administradores agregan ofertas.
13. Administrador agrega repartidores: Aquí la relación entre administrador y repartidor es de 1 a N. Un administrador puede agregar múltiples repartidores, pero un repartidor es agregado por un solo administrador. Hay una participación completa del repartidor porque cada repartidor es agregado por algún administrador, pero hay una participación parcial del administrador porque no todos los administradores agregan repartidores.
14. repartidor es asignado a pedidos: Aquí la relación entre repartidor y pedido es de 1 a N. Se puede asignar un repartidor a múltiples pedidos, pero se puede asignar un pedido a un solo repartidor. Hay una participación completa del pedido porque cada pedido se asigna a algún repartidor, pero hay una participación parcial del repartidor porque no todos los repartidores están asignados a un pedido.
15. El cliente califica la entrega del pedido con respecto al pedido y al repartidor: Esta es otra relación ternaria en nuestra tienda minorista en línea.
Hablando de estas una por una, hemos tomado algunas suposiciones aquí:
 1. Entre cliente y repartidor la relación es de N a 1, tal como hemos asumido e implementado de manera que M clientes pueden dar múltiples calificaciones a 1 repartidor con respecto a múltiples pedidos; aquí hay una participación parcial del cliente, ya que hemos asumido que no todos los clientes darán una calificación al repartidor, y hay una participación parcial del repartidor, ya que no todos los repartidores serán calificados por algún cliente.
 2. Entre repartidor y pedido la relación es de 1 a N, ya que hemos asumido que múltiples clientes pueden calificar a 1 repartidor con respecto a múltiples pedidos. Hay una participación parcial del repartidor, ya que no todos los repartidores pueden asignarse a un pedido, y hay una participación parcial del pedido, ya que no es necesario que cada pedido se asigne a un repartidor.
 3. Entre cliente y pedido la relación es de M a N, ya que hemos asumido que múltiples clientes pueden calificar múltiples pedidos (digamos N) con respecto a un repartidor en particular. Hay una participación parcial tanto del cliente como del pedido, ya que no todos los clientes agregan calificaciones con respecto al pedido y no todos los pedidos son calificados por un cliente según nuestra implementación.

## Conversión del Modelo E-R a Esquemas Relacionales
Convertimos el diagrama E-R en esquemas de relación de la siguiente manera, siguiendo las reglas relacionadas con la inclusión de claves foráneas donde sea necesario y creando tablas adicionales en el esquema para relaciones de M a N y también para relaciones con atributos. El esquema que creamos es el siguiente:

product(Product_ID, Name, Price, Brand, Measurement, Unit, Admin_ID, Category_ID)
customer(Customer_ID, First_Name, Last_Name, Email, Mobile_No, Password)
category(Category_ID, Category_Name)
admin(Admin_ID, First_Name, Last_Name, Admin_Password)
seller(Seller_ID, First_Name, Last_Name, Email, Phone_Number, Password, Place_Of_Operation, Admin_ID)
cart(Cart_ID, Total_Value, Total_Count, Final_Amount, Offer_ID)
orders(Order_ID, Mode, Amount, Order_Time, State, City, House_Flat_No, Pincode, Cart_ID, Date, Delivery_Boy_ID)
product_feedback(Review_ID, Rating, Review_Body, Product_ID, Customer_ID, Review_Date)
sells(Seller_ID, Product_ID, No_of_Product_Sold)
admin_views(Admin_ID, Order_ID, No_Of_Orders_Viewed)
selects(Customer_ID, Category_ID)
associated_With(Customer_ID, Cart_ID, Product_ID)
delivery_boy(Delivery_Boy_ID, First_Name, Last_Name, Password, Mobile_No, Email, Average_Rating, Admin_ID)
rates_order_delivery(Order_ID, Delivery_Boy_ID, Customer_ID, Rating_Given)
offer(Offer_ID, Promo_Code, Percentage_Discount, Min_OrderValue, Max_Discount, Admin_ID)
