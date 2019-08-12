#                            UNIVERSIDAD PUBLICA DE EL ALTO 
                              INGENIERIA DE SISTEMAS
NOMBRE: JIMENA PATZI SILLO  
CI: 8296537 LP  
DOCENTE: ING. MARIO TORREZ  
MATERIA: TECNOLOGIAS EMERGENTES II

                            SISTEMAS EMPRESARIALES
                                PRACTICA # 1
1.  Explique que son los sistemas empresariales

Un sistema distribuido es conjunto de computadoras 
independientes, interconectados a través de una red y que 
son capaces de colaborar con el fin de realizar una tarea.
Los sistemas distribuidos deben ser muy confiables, ya que si 
un componente del sistema se descompone otro componente 
debe ser capaz de reemplazarlo.       

2.  Describa cuales son las características más importantes de una aplicación empresarial
Las aplicaciones empresariales cuentas con las siguientes características:
•  Acceso a bases de datos, usualmente a bases de datos 
relacionales
•  Operaciones transaccionales, cumple con las propiedades 
ACID2
•  Escalables, permiten escalabilidad vertical y horizontal
•   Disponibles, idealmente prestan servicios de forma continua
•   Seguras, no todos los usuarios acceden con la misma 
funcionalidad
•   Permiten integración con otras tecnologías
•   Arquitectura multicapa
3.  Investigue y proponga cinco (5) instituciones que requerirían aplicaciones de misión critica
Justifique su respuesta
-  Alcaldía de la Ciudad de El Alto: Seria esencial una aplicación de misión crítica en la alcaldía de la ciudad de El Alto, ya que facilitaría mucho la comunicación entre todo el personal de trabajo en dicha institución, así agilizar el trabajo realizado.
-  Hospital “Los Andes”: La institución de salud requiere una aplicación de misión crítica para tener una comunicación interna y externa, para asi dar servicio a las personas.
-  Colegio “Fuerza Área Boliviana”: El colegio FAB requiere de una aplicación de misión crítica ya que sería fundamental para mejorar la forma de brindar información tanto a los estudiantes como a los profesores de dicha institución.
-   GADA 91 base área: Seria esencial la aplicación de misión critica para la institución GADA 91 ya que facilitaría mucho la intercomunicación entre todas personas de dicha institución.
-  Segip: El hecho de que se aplique la herramienta de la aplicación de misión critica en Segip sería muy útil para muchas personas que son beneficiadas con la institución, porque crecería la comunicación de información a toda la sociedad.
4.  Explique cuáles son las diferencias entre la escalabilidad horizontal y la escalabilidad vertical

La escalabilidad horizontal, se refiere a aumentar el número de componentes.
En cambio, la escalabilidad vertical, se refiere a actualizaciones de componentes existentes

5.  Que es un servidor Web y que es un servidor de aplicaciones

El Servidor web también llamado webserver, es el software que se encarga de despachar el contenido de un sitio web al usuario. 
Un servidor de aplicaciones es un dispositivo de software que proporcionan servicio de aplicación a las computadoras cliente, generalmente gestiona la mayor parte o en su totalidad de las funciones de la lógica de negocio y acceso a los datos de la aplicación

6.  Con un gráfico explique cómo funciona el protocolo HTTP

![clipboard](https://i.imgur.com/daOi5VQ.png)

HTTP corre sobre el protocolo TCP/IP, empleado para la transferencia de recursos que componen una web. 


7.  Explique los elementos importantes de REQUEST en HTTP
HTTP define un conjunto de métodos de petición para indicar la acción que se desea realizar para un recurso determinado. Aunque estos también pueden ser sustantivos, estos métodos de solicitud a veces son llamados HTTP verbs. Cada uno de ellos implementan una semántica diferente, pero algunas características similares son compartidas por un grupo de ellos: ej. un request method puede ser safe, idempotent, o cacheable.

GET: El método GET solicita una representación de un recurso específico. Las peticiones que usan el método GET sólo deben recuperar datos.

HEAD: El método HEAD pide una respuesta idéntica a la de una petición GET, pero sin el cuerpo de la respuesta.

POST: El método POST se utiliza para enviar una entidad a un recurso en específico, causando a menudo un cambio en el estado o efectos secundarios en el servidor.

PUT: El modo PUT reemplaza todas las representaciones actuales del recurso de destino con la carga útil de la petición.

DELETE: El método DELETE borra un recurso en específico.

CONNECT: El método CONNECT establece un túnel hacia el servidor identificado por el recurso.

OPTIONS: El método OPTIONS es utilizado para describir las opciones de comunicación para el recurso de destino.

TRACE: El método TRACE  realiza una prueba de bucle de retorno de mensaje a lo largo de la ruta al recurso de destino.

PATCH:El método PATCH  es utilizado para aplicar modificaciones parciales a un recurso. 

8.  Explique los elementos importantes de RESPONSE en HTTP

OK
La solicitud ha tenido éxito. El significado de un éxito varía dependiendo del método HTTP

GET: El recurso se ha obtenido y se transmite en el cuerpo del mensaje.

HEAD: Los encabezados de entidad están en el cuerpo del mensaje.

PUT o POST: El recurso que describe el resultado de la acción se transmite en el cuerpo del mensaje.

TRACE: El cuerpo del mensaje contiene el mensaje de solicitud recibido por el servidor.
 Created
 
La solicitud ha tenido éxito y se ha creado un nuevo recurso como resultado de ello. Ésta es típicamente la respuesta enviada después de una petición PUT.

Accepted
 
La solicitud se ha recibido, pero aún no se ha actuado. Es una petición "Sin compromiso", lo que significa que no hay manera en HTTP que permita enviar una respuesta asíncrona que indique el resultado del procesamiento de la solicitud. Está pensado para los casos en que otro proceso o servidor maneja la solicitud, o para el procesamiento por lotes.

 Non-Authoritative Information
 
La petición se ha completado con éxito, pero su contenido no se ha obtenido de la fuente originalmente solicitada, sino que se recoge de una copia local o de un tercero. Excepto esta condición, se debe preferir una respuesta de 200 OK en lugar de esta respuesta.

No Content

La petición se ha completado con éxito pero su respuesta no tiene ningún contenido, aunque los encabezados pueden ser útiles. El agente de usuario puede actualizar sus encabezados en caché para este recurso con los nuevos valores.

 Reset Content
 
La petición se ha completado con éxito, pero su respuesta no tiene contenidos y además, el agente de usuario tiene que inicializar la página desde la que se realizó la petición, este código es útil por ejemplo para páginas con formularios cuyo contenido debe borrarse después de que el usuario lo envíe.

 Partial Content
 
La petición servirá parcialmente el contenido solicitado. Esta característica es utilizada por herramientas de descarga como wget para continuar la transferencia de descargas anteriormente interrumpidas, o para dividir una descarga y procesar las partes simultáneamente.

Multi-Status (WebDAV)

Una respuesta Multi-Estado transmite información sobre varios recursos en situaciones en las que varios códigos de estado podrían ser apropiados. El cuerpo de la petición es un mensaje XML.

Multi-Status (WebDAV)

El listado de elementos DAV ya se notificó previamente, por lo que no se van a volver a listar.

IM Used (HTTP Delta encoding)

El servidor ha cumplido una petición GET para el recurso y la respuesta es una representación del resultado de una o más manipulaciones de instancia aplicadas a la instancia actual.

9.  Describa con un grafico de arquitectura Java EE

![clipboard](https://i.imgur.com/FQIL7sh.png)



10.  Explique cuáles son los contenedores, componentes y servicios de Java EE

Contendores: Un contenedor es un entorno de ejecución que provee al componente una serie de servicios, define los siguientes tipos de contenedores: 

  Contenedor Web: Maneja la ejecución de las paginas web, servlets y algunos componentes ejb para las aplicaciones Java EE.

  Contenedor EJB: Maneja la ejecución de los enterprise beans.

   Contenedor Web: Maneja la ejecución de las paginas web, servlets y algunos componentes ejb para las aplicaciones Java EE. 

  Contenedor de aplicación cliente: Maneja la ejecución de la aplicación cliente no necesita un servidor de aplicaciones.

  Contenedor Applet: Maneja la ejecución de applets, no necesita servidor de aplicaciones, consiste en un browser y el plugin web de java.

Componentes: Un componente es una unidad de software que forma parte de una aplicación, define los siguientes tipos de componentes:

  Componente cliente (cliente AWT, Swing, Appet y navegador web): Corriendo en la maquina del Cliente.

![clipboard](https://i.imgur.com/mjUJMvQ.png)


  Componente web (Servlet, JSP y JSF): Corriendo en el servidor Java EE.

![clipboard](https://i.imgur.com/WqmE3oO.png)



  Componente de negocio (EJB): Corriendo en el servidor Java EE.

![clipboard](https://i.imgur.com/2rSpw5h.png)



Servidores: Son los servidores que deben ofrecer los contendores JAVA E, son los siguientes:

  De directorio: para la indexación y búsqueda de componentes y recursos   

  De despliegue: para poder personalizar los componentes y recursos.

  De transaccionalidad: para poder ejecutar distintas acciones de una misma unidad transaccional.

  De seguridad: para poder autenticar y autorizar a los usuarios de la aplicación.

  De acceso a datos: para facilitar el acceso a Base de Datos.

  De conectividad: para poder acceder fácilmente a distintos EIS.

  De mensajería: para poder comunicarse con otros componentes, aplicación o EIS

11.  Investigue los métodos más utilizados de las clases HttpServlet, HttpServletRequest y HttpServletResponse, y para cada uno de los métodos muestre un ejemplo.

HTTPSERVLET: Todos los servlets implementan este interfaz directamente o extendiendo una clase que lo implemente como HttpServlet. Entre sus métodos están:
•  init(ServletConfig config): Es el método utilizado para crear una nueva instancia del servlet (análogo al constructor). Ver el ciclo de vida. Este método puede ser sobreescrito para realizar tareas como crear una conexión a una BD que se mantendrá mientras el servlet se mantenga cargado y puede ser utilizada por cada petición. ServletConfig contiene los parámetros de inicialización que entrega el servidor al servlet.

Ejemplo:

import javax.servlet.*;

public class UnServlet extends HttpServlet {

 public void init(ServletConfig config) throws ServletException {
 
    super.init(config);
  }
}
•  getServletConfig(): Retorna la configuración dada para la inicialización del servlet.

Ejemplo:

ServletConfig config = getServletConfig();

•  service(ServletRequest req, ServletResponse res): Este método es el que se llama cuando se recibe una petición de un cliente y en su implementación normal para HTTP verifica el tipo de solicitud GET, POST, etc. y la redirige a los métodos respectivos. En general no es necesario reimplementar este método.

•  destroy(): Este método es llamado por el servidor para indicar que el servlet será destruido. Es llamado sólo una vez y uno debe encargarse de esperar por posibles peticiones en curso.

HTTPSERVLETREQUEST: Cuenta con los diferentes métodos.

request.getParameter

Se utiliza para recoger parametros enviados por una peticion get o post.

Por ejemplo:

String variable = request.getParameter("datosget");

Este codigo tomaria el parametro datos get y lo guardaria en una varible de tipo string.

Si quisieramos guardar datos de otro tipo, tendríamos que utilizar una clase envolvente para indicar su tipo.
 
request.gerParameterValues

La funcion de este metodo es la misma que la del anterior, salvando la diferencia de que lo que recibe es un vector y no un solo parametro.
La forma de recogerlo seria:

String [] variables = request.getParameterValues("vector");

Cabe destacar, al igual que en el metodo anterior, que si queremos un vector de algo que no sean cadenas, deberemos utilizar clases envolventes.
 
request.getAttribute

Se utiliza para recoger atributos enviados con el metodo setAttribute. Es el metodo utilizado para recoger parametros de una sesion.

Ejemplo

String l = request.getAttribute("login")

 
request.getSession

Sirve para tomar la sesion del usuario y almacenarla en una variable de tipo HttpSession.

Ejemplo:

HttpSession repositorio = request.getSession();
 

HTTPSERVLETREPONSE: Cuenta con los siguientes métodos:

Response.AddHeader "Nombre", "Valor"

Este método permite añadir una nueva cabecera a la respuesta HTTP. Una vez que la cabecera ha sido creada, no es posible borrarla. El nombre dado a la nueva cabecera no puede contener ningun carácter de subrayado ( _ )
Se escribe:

<% 
Response.AddHeader "MiCabecera", "PRUEBA"
%>

Response.AppendToLog("String")

Mediante este método se puede añadir un string al registro que se genera con cada request en el fichero de logs del IIS.

Por ejemplo:

<%
Response.AppendToLog("Mi comentario")
%>

Y este sería el string añadido en un registro típico del fichero de logs del IIS:
125.125.125.125, - , 05/27/99, 9:50:00, W3SVC, PRUEBAS, 125.125.125.125, Mi comentario

Response.BinaryWrite(Data)

Escribe la salida HTTP en binario (no en modo string como lo hace Response.Write), y sin aplicar ninguna conversión de página de caracteres.

Supongamos que tenemos el siguiente formulario HTML con tres campos:

'---Fichero formulario.htm
<HTML><HEAD> <TITLE>Prueba1 ASP</TITLE> </HEAD>
<BODY>
<FORM ACTION="prueba2.asp" METHOD="POST">
Nombre:<INPUT TYPE="text" NAME="Nombre" VALUE="Juan" ><br>
Ciudad:<INPUT TYPE="text" NAME="Ciudad" VALUE="Guadalajara" ><br>
Postal:<INPUT TYPE="text" NAME="Postal" VALUE="12345"       ><br>
<INPUT TYPE="Submit" NAME="Boton" VALUE="Enviar">
</FORM>
</BODY>
</HTML>
Para poder ver el nombre de los campos y sus contenidos se escribe lo siguiente:
'---Fichero prueba2.asp

<% 
bytecount = Request.TotalBytes
binread = Request.BinaryRead(bytecount)
Response.BinaryWrite binread
%>

Y este sería el resultado:

Nombre=Juan&

Ciudad=Guadalajara&

Postal=12345&Boton=Enviar

Response.Clear

Este método se utiliza para vaciar (borrar) cualquier contenido del buffer de salida. No elimina las cabeceras HTTP, solamente el contenido que va entre los elementos <BODY> y </BODY> Si el buffer ya está vacío debido a que previamente se ha invocado 

Response.Buffer=False, se produce un error de ejecución. Recuerda que en la versión 2.0 de ASP el valor por defecto de Response.Buffer es False y en la versión 3.0 es True.

Se escribe:

<% 

Response.Clear 

%>

Response.End

Cuando se invoca este método el servidor detiene el proceso de la página ASP actual y envia al cliente el contenido del buffer de salida, siempre que Response.Buffer=True. El resto de instrucciones no se procesará. Recordar que en la versión 2.0 de ASP el valor por defecto de Response.Buffer es False y en la versión 3.0 es True.

Por ejemplo, si se escribe:

<% 

Response.Write "Primer string"  
Response.End  
Response.Write "Segundo string" 

%>

Sólo se obtiene en la respuesta:

Primer string 
Response.Flush  

Este método provoca el envio inmediato al cliente del contenido del buffer de salida, en lugar de hacerlo al concluir el proceso completo de la página, y continuando después con el resto de instrucciones normalmente. Si el buffer está vacío debido a que previamente se ha invocado Response.Buffer=False, se produce un error de ejecución. Recuerda que en la versión 2.0 de ASP el valor por defecto de Response.Buffer es False y en la versión 3.0 es True.

Se escribe:

<%   
Response.Flush   
%>
