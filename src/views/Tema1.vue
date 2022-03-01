<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5

    .titulo-principal.color-acento-contenido.mb-0(data-aos="flip-up")
      .titulo-principal__numero
        span 1
      h1 #[i Hibernate]
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-0
        .row
          .col-lg-5
            img(src="@/assets/curso/tema1/img1.png").m-auto
          .col-lg-7
            .row
              .col-12
                p.mt-5.mb-4 Hibernate es software libre con licencia GNU LGPL que presta servicios de ORM para JAVA, es decir, es plugin que puede ser integrado al IDE de desarrollo en JAVA que facilita el proceso de mapeo de tablas en una base de datos relacional a objetos JAVA mediante el uso de archivos declarativos en formato XML o anotaciones.
                .row.mb-4.bg-color4.justify-content-end
                  .col-12
                    img(src="@/assets/curso/tema1/img2.svg" style="width: 50px; margin-left:40px")
                  .col-10
                    .p-4
                      p.text-white #[i Hibernate] utiliza JDBC para todos los procesos de comunicación con la base de datos funcionando como una capa adicional de abstracción de las funcionalidades del JDBC. En una aplicación JAVA podremos delegar la mayoría de las operaciones de bases de datos al #[i framework] de #[i Hibernate] pero en segundo plano todo estará pasando por el API de JDBC.
                      .row.align-items-center
                        .col-10.d-inline
                          p.text-white.text-end.mb-0 #[b Martinez (2015)]
                        img(src="@/assets/curso/tema1/img3.svg" style="width: 40px")
                p Así que cuando estamos configurando #[i Hibernate] para conectarse a una base de datos lo que realmente pasa es que se configura #[i Hibernate] para el Uso del JDBC y es este quien realiza las operaciones.  A continuación se presenta el esquema general del funcionamiento:
    img(src="@/assets/curso/tema1/img4.svg" style="width: 1100px").m-auto.mb-5(data-aos="slide-right")
    p.mb-5 Para el desarrollo de una aplicación JAVA que usa el entorno de desarrollo de #[i Eclipse] es necesario descargar todas las librerías requeridas por el #[i framework] de #[i Hibernate] las cuales puede encontrar en la página oficial del ORM #[span.text-deco1.text-white #[a(href="https://hibernate.org/orm/" target="blank") https://hibernate.org/orm/]]. Una vez descargado el paquete este se debe descomprimir y podrá encontrar los archivos jar necesarios en la ubicación /lib/required los cuales deberá anexar al proyecto JAVA.
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-0
        .row
          .col-lg-7
            .row.mt-3
              .col-12.mt-5.mb-4.bg-color5
                .p-4
                  p.mb-0 Debido a que #[i Hibernate] utiliza el #[i Driver] JDBC necesitará también descargar el #[i Driver] correspondiente a la base de datos a acceder desde su página oficial. Para el caso de MySQL podrá encontrar el #[i Driver] en: #[span.text-deco1.text-white #[a(href="https://dev.mysql.com/downloads/connector/j/" target="blank") https://dev.mysql.com/downloads/connector/j/]].
            .row
              .col-12.mb-4
                p.ms-0.ms-lg-5 En el siguiente video se muestra un ejemplo de alistamiento de una aplicación JAVA en IDE de #[i Eclipse] para trabajar con #[i Hibernate] y una base de datos MySQL.
            .tarjeta.color-primario.p-3.mb-5.ms-0.ms-lg-5
              .row.justify-content-around.align-items-center
                .col-3.col-sm-2.col-lg-1
                  img(src="@/assets/curso/tema1/img5.svg")
                .col
                  .row.justify-content-between.align-items-center
                    .col.mb-3.mb-sm-0
                      h3.mb-1.text-white Alistamiento #[i Hibernate]
                      p.text-small.text-white Estimado aprendiz, para profundizar sobre el tema puede consultar el siguiente video. 
                    .col-sm-auto
                      a.boton.color-acento-contenido.texto-blanco(href="https://www.youtube.com/watch?v=wUV2JemOo9k" target="_blank")
                        span(style="color:#000000 !important") Ver
                        i.fas.fa-file-download(style="color:#000000 !important")
          .col-lg-5
            img(src="@/assets/curso/tema1/img2.png").m-auto
        .row
          .col-12
            br
            br
    .row.justify-content-center
      .col-10.text-deco2
        .cajon.color-primario.p-4
          p.mb-0 Teniendo en cuenta que #[i Hibernate] debe usar el #[i Driver] JDBC para la ejecución de las instrucciones en la base de datos se debe construir un archivo de configuración en formato XML donde se especifique la Url del JDBC y las credenciales de acceso a la base de datos. En la siguiente figura se presenta el esquema general de funcionamiento en el proceso de configuración:
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white #[i Hibernate] Archivo de configuración
    img(src="@/assets/curso/tema1/img6.svg" style="width: 1000px").m-auto.mb-5(data-aos="slide-left")
    img(src="@/assets/curso/tema1/img3.png" style="width: 1300px").m-auto
    .row.justify-content-center
      .col-10.bg-color8
        .p-4
          p.mb-0 Este archivo de configuración define un conjunto de propiedades que serán utilizadas para crear las sesiones mediante las cuales se inicia un conjunto de transacciones u operaciones sobre la base de datos, entre las propiedades más importantes se encuentran las siguientes:
    .row.bg-color9
      .col-12.px-5
        .row.justify-content-center
          .col-lg-10
            .tabla-a.color-acento-botones.mb-5 
              table
                thead
                  tr
                    th(width="30%") Propiedad
                    th Definición
                tbody
                  tr(style="background-color: #FFFFFF")
                    td connection.driver.class
                    td Parte de la configuración del JDBC donde se define el #[i driver] a usar.
                  tr(style="background-color: #E8E8E8")
                    td connection.url
                    td Parte de la configuración del JDBC donde se define la url de la base de datos a utilizar (protocolo: url base de datos: puerto / nombre DB).
                  tr(style="background-color: #FFFFFF")
                    td connection.username
                    td Parte de la configuración del JDBC donde se define el usuario de la base de datos a utilizar en la conexión.
                  tr(style="background-color: #E8E8E8")
                    td connection.password
                    td Parte de la configuración del JDBC donde se define el #[i password] del usuario de la base de datos a utilizar en la conexión.
                  tr(style="background-color: #FFFFFF")
                    td connection.pool_size
                    td Número de conexiones simultáneas al JDBC.
                  tr(style="background-color: #E8E8E8")
                    td dialect
                    td Aunque SQL es un estándar, cada motor de bases de datos tiene una implementación particular. En esta propiedad se especifica el dialecto a utilizar por #[i Hibernate].
                  tr(style="background-color: #FFFFFF")
                    td show_sql
                    td Esta propiedad permite ver en la salida estándar las sentencias SQL que ejecuta en #[i background Hibernate] lo cual sirve mucho para entender lo que está sucediendo en entornos de desarrollo.
                  tr(style="background-color: #E8E8E8")
                    td current_session_context_class
                    td Especifica el contexto de la sesión actual, por defecto se puede asignar #[i thread].
        p.mb-5 Es importante tener en cuenta que este archivo de configuración de #[i Hibernate] debe estar ubicado en la raíz de la carpeta src del proyecto de forma que pueda ser utilizado por #[i Hibernate] en cualquier contexto de la aplicación. A continuación, se muestra cómo debe verse un archivo de configuración de #[i Hibernate] completo donde se establece una conexión con una base de datos MySQL en un servidor que se está ejecutando en la máquina local en #[i localhost] y puerto 3306 con el usuario #[i root] y contraseña 12345:
        .row.mb-5
          .col-12.bg-color11
            img(src="@/assets/curso/tema1/img8.svg")
          .col-12.bg-color10
            .p-4
              p.mb-0 #[span.text-white &lt;!]#[span.text-deco3 DOCTYPE hibernate-configuration] #[span.text-white PUBLIC]
              p.mb-0.text-white(style="margin-left: 20px") “-//Hibernate/Hibernate Configuration DTD 3.0//EN”
              p.text-white(style="margin-left: 20px") “http://www.hibernate.org/dtd/hibernate-configuration-3.0.dtd”&gt;
              p #[span.text-white &lt;]#[span.text-deco3 hibernate-configuration]#[span.text-white &gt;]
              p(style="margin-left: 20px") #[span.text-white &lt;]#[span.text-deco3 session-factory]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-deco4 &lt;!-- JDBC Database connection settings --&gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 "connection.driver_class"]#[span.text-white &gt;com.mysql.cj.jdbc.Driver&lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 "connection.url"]#[span.text-white &gt;]#[span.text-deco7 jdbc:mysql://localhost:3306/prueba?useSSL=false&serverTimezone=UTC]#[span.text-white &lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 "connection.username"]#[span.text-white &gt;]#[span.text-deco7 root]#[span.text-white &lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 "connection.password"]#[span.text-white &gt;]#[span.text-deco7 12345]#[span.text-white &lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-deco4 &lt;!-- JDBC connection pool settings … using built-in test pool --&gt;]
              p(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 “connection.pool_size”]#[span.text-white &gt;1&lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-deco4 &lt;!-- Select our SQL dialect --&gt;]
              p(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 “dialect”]#[span.text-white &gt;org.hibernate.dialect.MySQLDialect&lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-deco4 &lt;!-- Echo the SQL to stdout --&gt;]
              p(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 “show_sql”]#[span.text-white &gt;true&lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p.mb-0(style="margin-left: 40px") #[span.text-deco4 &lt;!-- Set the current session context --&gt;]
              p(style="margin-left: 40px") #[span.text-white &lt;]#[span.text-deco3 property] #[span.text-deco5 name]#[span.text-white =]#[span.text-deco6 “current_session_context_class”]#[span.text-white &gt;thread&lt;/]#[span.text-deco8 property]#[span.text-white &gt;]
              p(style="margin-left: 20px") #[span.text-white &lt;/]#[span.text-deco3 session-factory]#[span.text-white &gt;]
              p #[span.text-white &lt;/]#[span.text-deco3 hibernate-configuration]#[span.text-white &gt;]
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-0
        .row
          .col-lg-5
            img(src="@/assets/curso/tema1/img2.png").m-auto
          .col-lg-7
            .row.mt-3
              .col-12.mt-2.mt-lg-5.mb-4.bg-color12
                .p-4
                  p.mb-0 Se invita a revisar en los anexos el archivo de configuración mostrado anteriormente para que pueda ser descargado y utilizado en la construcción de su proyecto, teniendo en cuenta que debe editar las propiedades de acuerdo con sus necesidades.
            .row
              .col-12.mb-4
                p.me-0.me-md-4 Luego de esto se requiere definir todas las #[i Entity Classes] que serán utilizadas por #[i Hibernate] para realizar el proceso de mapeo hacia una base de datos relacional y viceversa. Una #[i Entity Class] básicamente es una clase #[i Java] tradicional que tiene las mismas características definidas una tabla de la base de datos, es decir, es una imagen de la tabla (ver siguiente figura) pero desde la perspectiva de la programación orientada a objetos que adicionalmente tiene unas anotaciones especiales que le permiten a #[i Hibernate] realizar el trabajo adecuado.
    img(src="@/assets/curso/tema1/img9.svg" style="width: 1300px").m-auto.mb-5(data-aos="slide-right")
    .cajon.color-primario.p-4.mb-5
      p.mb-0 Las anotaciones pueden ser utilizadas al importar la librería de persistencia de JAVA javax.persistence.*, entre las más utilizadas encontramos:
    .row.bg-color9
      .col-12.px-5
        .row.justify-content-center
          .col-lg-10
            .tabla-a.color-acento-botones.mb-5 
              table
                thead
                  tr
                    th(width="30%") Anotación
                    th Significado
                tbody
                  tr(style="background-color: #FFFFFF")
                    td @Entity
                    td Especifica que la clase definida en una #[i Entity Class].
                  tr(style="background-color: #E8E8E8")
                    td @Table(name = “ ”)
                    td Permite especificar que la clase será mapeada con una tabla en la base de datos especificada en la propiedad #[i name].
                  tr(style="background-color: #FFFFFF")
                    td @Column(name = “ ”)
                    td Permite especificar que el atributo por ser definido será mapeado con una columna especificada por la propiedad #[i name]. Cuando el nombre del atributo coincide con el nombre de la columna en la tabla se puede omitir la especificación de la propiedad #[i name] y solo dejar la anotación @Column.
                  tr(style="background-color: #E8E8E8")
                    td @Id
                    td Permite especificar que el atributo a definir corresponde con el identificador primario a ser mapeado en la tabla.
        img(src="@/assets/curso/tema1/img10.svg" style="width: 1000px").m-auto.mb-5(data-aos="slide-left")
        p.mb-5 A continuación, se muestra un corto video donde se agrega el archivo de configuración de #[i Hibernate] al proyecto y se crea la clase #[i Entity] para la gestión de una tabla en una base de datos MySQL.
        figure.mb-5
          .video
            iframe(width="560" height="315" src="https://www.youtube.com/embed/fKlKfb5ftAM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    #t_1_1
    .titulo-segundo.color-secundario
      h2 1.1 Operaciones básicas
    .row.bg-color3.mb-4
      .col-12.px-5.px-lg-0
        .row
          .col-lg-5
            img(src="@/assets/curso/tema1/img4.png").m-auto
          .col-lg-7
            .row.mt-3
              .col-12.mt-2.mt-lg-4.mb-4.bg-color12
                .p-4
                  p.mb-0 Una vez se tienen registradas todas dependencias, los archivos de configuración de #[i Hibernate] y las respectivas clases de entidad se puede utilizar las facilidades ofrecidas por #[i Hibernate] para la manipulación de la base de datos de forma transparente por medio de los procesos de mapeo que ofrece este #[i framework].
              .col-12.pe-1.pe-lg-5
                p.mb-4 Hibernate utiliza principalmente dos clases que debemos utilizar, las cuales se describen a continuación:
                .tabla-a.color-acento-botones.mb-4.mb-lg-0
                  table
                    thead
                      tr
                        th(width="30%") Class
                        th Descripción
                    tbody
                      tr(style="background-color: #FFFFFF")
                        td #[i SessionFactory]
                        td Esta clase lee el archivo de configuración de #[i Hibernate] y crea los objetos de sesión. Por ser una clase que genera objetos pesados por los procesos de los que es responsable solo debo crearlo una vez por toda la aplicación.
                      tr(style="background-color: #E8E8E8")
                        td #[i Session]
                        td Esta clase envuelve todo lo correspondiente a una conexión JDBC y es el tipo de objeto que será usado para guardar o recibir objetos desde y hacia la base de datos. Es instanciado a partir de una clase #[i SessionFactory]. Los objetos creados de este tipo son más livianos por lo que pueden ser creados y desechados tantas veces como se necesite dentro de la aplicación.
    .row.bg-color9
      .col-12.px-5
        .cajon.color-primario.p-4.mb-5
          p.mb-0 En el siguiente fragmento de código se muestra un esqueleto de como es el proceso de definición de los objetos #[i SessionFactory] y #[i Session] para poder hacer la manipulación de la base de datos.
        .row.mb-5
          .col-lg-8
            .row
              .col-12.bg-color11
                img(src="@/assets/curso/tema1/img8.svg")
              .col-12.bg-color10
                .p-4
                  p.mb-0 #[span.text-deco9 // creación del session factory]
                  p.mb-0 #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                  p.mb-0(style="margin-left:20px") #[span.text-deco13 .configure(#[span.text-deco14 “hibernate.cfg.xml”])]
                  p.mb-0(style="margin-left:20px") #[span.text-deco13 .addAnnotatedClass(#[span.text-deco11 Usuario.class])]
                  p(style="margin-left:20px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                  p.mb-0 #[span.text-deco9 // creación de la session a partir del Session factory]
                  p #[span.text-deco10 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                  p #[span.text-deco12 try]#[span.text-white {]
                  p(style="margin-left:20px") #[span.text-deco9 // Ahora se puede usar el objeto session para la manipulación de la BD]
                  p.mb-0 #[span.text-white }]
                  p #[span.text-deco12 finally]#[span.text-white {]
                  p.mb-0(style="margin-left:20px") #[span.text-deco9 // Se cierra el objeto session factory una vez se deja de utilizar]
                  p(style="margin-left:20px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                  p.mb-0 #[span.text-white }]
          .col-lg-4
            img(src="@/assets/curso/tema1/img11.svg" style="width: 310px").m-auto(data-aos="slide-left")
        p.mb-5 Note que en el código anterior para creación del objeto #[i SessionFactory] se indica el nombre del archivo de configuración de Hibernate en método #[i configure()], si este parámetro no se incluyera #[i Hibernate] buscará en el directorio raíz del proyecto un archivo que contenga el nombre por defecto de este tipo de archivos de configuración el cual es hibernate.cfg.xml. También note que en el método #[i addAnnotatedClass()] se indica la clase de entidad a ser utilizada.
        AcordionA.mb-5(tipo="a" clase-tarjeta="tarjeta tarjeta--azul").mb-5
          .row(titulo="Método <i>Save</i>")
            .col-12
              p.mb-4 El método #[i save()] del objeto #[i Session] permite hacer el proceso de inserción de un nuevo registro en la base de datos enviando como parámetro un objeto de tipo entidad con sus valores. La forma correcta de hacer un proceso de inserción de un nuevo registro de una base de datos con un objeto de tipo sesión incluye los siguientes pasos:
              .row.mb-4
                .col-6.col-lg-3
                  img(src="@/assets/curso/tema1/img12.svg").m-auto
                .col-6.col-lg-3
                  img(src="@/assets/curso/tema1/img13.svg").m-auto
                .col-6.col-lg-3
                  img(src="@/assets/curso/tema1/img14.svg").m-auto
                .col-6.col-lg-3
                  img(src="@/assets/curso/tema1/img15.svg").m-auto
              .row.justify-content-center
                .col-lg-10
                  .row
                    .col-12.bg-color11
                      img(src="@/assets/curso/tema1/img8.svg")
                    .col-12.bg-color10
                      .p-4
                        p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                        P.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                        P.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                        P.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                        P #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                        p #[span.text-deco8 public class] #[span.text-deco9 CreateUserDemo] #[span.text-white {]
                        p.mb-0(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco9 void] #[span.text-deco13 main(]#[span.text-deco11 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                        p.mb-0(style="margin-left:40px") #[span.text-deco9 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                        p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                        p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                        p(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                        p(style="margin-left:40px") #[span.text-deco9 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                        p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                        p.mb-0(style="margin-left:60px") #[span.text-deco9 System.out]#[span.text-deco13 .println(]#[span.text-deco14 "Creando un usuarios..."]#[span.text-deco13 )]#[span.text-white ;]
                        p.mb-4(style="margin-left:60px") #[span.text-deco7 Usuario usuario1 = new Usuario("Francisco","FFFFF#");]
                        p.mb-0(style="margin-left:60px") #[span.text-deco7 session.beginTransaction();]
                        p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Guardando los nuevos usuarios …”]#[span.text-deco13 )]#[span.text-white ;]
                        p.mb-0(style="margin-left:60px") #[span.text-deco7 session.save(usuario1);]
                        p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “El usuario se almaceno con el ID:”]#[span.text-white +]#[span.text-deco9 usuario1]#[span.text-deco13 .getUserId())]#[span.text-white ;]
                        p.mb-0(style="margin-left:60px") #[span.text-deco7 session.getTransaction().commit();]
                        p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Proceso finalizado”]#[span.text-deco13 )]#[span.text-white ;]
                        p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                        p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                        p(style="margin-left:40px") #[span.text-white }]
                        p(style="margin-left:20px") #[span.text-white }]
                        p #[span.text-white }]
          div(titulo="Método <i>Get</i>")
            .row
              .col-12
                p.mb-5  El método #[i get()] del objeto #[i session] permite obtener un registro de la base de datos por medio de una consulta por su llave primaria. Este método recibe como parámetro la clase de entidad que será utilizada para hacer el mapeo del registro en la respuesta y un segundo parámetro que corresponde al valor a ser buscado en la llave primaria de la tabla. Este método ofrece como resultado un objeto de la clase de entidad especificado en la invocación del método. La forma correcta de hacer un proceso de consulta de un registro particular por medio de su llave primaria y un objeto de tipo session incluye los siguientes pasos:
                .row.align-items-center.justify-content-center
                  .col-lg-5.mb-5.mb-lg-0
                    img(src="@/assets/curso/tema1/img16.svg" style="width: 450px").m-auto
                  .col-lg-6
                    .tarjeta-avatar-b.mb-5
                      .tarjeta-avatar-b__img
                        img(src='@/assets/curso/tema1/img17.svg' alt='AvatarTop')
                      .tarjeta.tarjeta--blanca
                        .p-4
                          br
                          p.mb-0 Iniciar una transacción por medio del método #[i beginTransaction()]
                          br
                    .tarjeta-avatar-b.mb-5
                      .tarjeta-avatar-b__img
                        img(src='@/assets/curso/tema1/img18.svg' alt='AvatarTop')
                      .tarjeta.tarjeta--blanca
                        .p-4
                          p.mb-0 Invocar el método #[i get()] de la sesión enviando como parámetro la clase de tipo entidad para hacer mapeo y el valor de la llave primaria a buscar. La invocación de este método requiere de un objeto compatible que reciba el resultado.
                    .tarjeta-avatar-b.mb-5
                      .tarjeta-avatar-b__img
                        img(src='@/assets/curso/tema1/img19.svg' alt='AvatarTop')
                      .tarjeta.tarjeta--blanca
                        .p-4
                          br
                          p.mb-0 Confirmar la transacción realizada por medio del método #[i getTransaction().commit()]
                          br
                .row.justify-content-center
                  .col-lg-10
                    .row
                      .col-12.bg-color11
                        img(src="@/assets/curso/tema1/img8.svg")
                      .col-12.bg-color10
                        .p-4
                          p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                          p #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                          p #[span.text-deco8 public class] #[span.text-deco10 CreateUserDemo] #[span.text-white {]
                          p(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco10 void] #[span.text-deco13 main(]#[span.text-deco10 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                          p.mb-0(style="margin-left:40px") #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                          p(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-deco10 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]      
                          p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                          p.mb-0(style="margin-left:60px") #[span.text-deco7 session.beginTransaction();]
                          p(style="margin-left:60px") #[span.text-deco9 //consulta de un usuario cuya pk tiene el valor de 16]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Consulta de un usuario”]#[span.text-deco13 )]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco10 Usuario] #[span.text-deco11 resultado] #[span.text-white =] #[span.text-deco11 session]#[span.text-deco13 .get(]#[span.text-deco10 Usuario.class]#[span.text-white ,] #[span.text-deco15 16]#[span.text-deco13 )]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Resultado= “]#[span.text-white +resultado]#[span.text-deco13 )]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .getTransaction().commit()]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Proceso finalizado”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-white }]
                          p(style="margin-left:20px") #[span.text-white }]
                          p #[span.text-white }]
          div(titulo="Método <i>CreateQuery</i>")
            .row
              .col-12
                .row.mb-4.align-items-center.justify-content-center
                  .col-lg-6.mb-4.mb-lg-0
                    img(src="@/assets/curso/tema1/img5.png").m-auto
                  .col-lg-6
                    p #[i Hibernate] permite el proceso de creación de consultas usando HQL, el cual es una versión especial de #[i Hibernate] para establecer consultas SQL pero es orientado a objetos y comprende nociones propias del paradigma orientado a objetos como la herencia, el polimorfismo y las asociaciones. Es importante tener en cuenta que aunque las palabras reservadas y sentencias de SQL no son sensibles a mayúsculas los nombres de las clases y sus atributos usados en HQL si lo son.
                    .cajon.color-primario.p-4.bg-color13
                      p.mb-0 Para el caso en el que se requiera realizar consultas más avanzadas se puede utilizar la potencia de HQL para establecer las características de los registros a ser consultados, como este tipo de consulta puede producir como resultado más de un registro proveniente de la base de datos es necesario usar el método #[i getResultList()], para poder mapear la respuesta a una lista de objetos JAVA.
                p.mb-5 En la siguiente tabla se muestra algunas de las cláusulas HQL más comúnmente utilizadas, tengo en cuenta que en HQL se hace referencia a las clases de entidad JAVA con sus atributos los cuales son sensibles a mayúsculas y estas sentencias son mapeadas a su equivalente estructura en la base de datos usando los nombres de tablas y atributos los cuales ya no son sensibles a mayúsculas:
                .row.justify-content-center.mb-5
                  .col-lg-8
                    .tabla-a.color-acento-botones
                      table
                        thead
                          tr
                            th(width="30%") Sentencia HQL
                            th Equivalente en SQL
                        tbody
                          tr(style="background-color: #FFFFFF")
                            td from #[span.text-deco16 Usuario]
                            td SELECT * FROM #[span.text-deco17 usuario]
                          tr(style="background-color: #E8E8E8")
                            td from #[span.text-deco16 Usuario] u where u#[span.text-deco16 .userName] = ‘Raul’
                            td
                              p.mb-0 SELECT * FROM #[span.text-deco17 usuario] U 
                              p WHERE u.username = ‘Raul’
                          tr(style="background-color: #FFFFFF")
                            td from #[span.text-deco16 DomesticCat] cat
                            td SELECT * FROM #[span.text-deco17 domesticCat] Cat
                          tr(style="background-color: #E8E8E8")
                            td order by cat#[span.text-deco16 .name] asc
                            td ORDER BY Cat#[span.text-deco17 .name] ASC
                          tr(style="background-color: #FFFFFF")
                            td order by cat#[span.text-deco16 .name] asc
                            td ORDER BY Cat#[span.text-deco17 .name] ASC
                          tr(style="background-color: #E8E8E8")
                            td
                              p.mb-0 from #[span.text-deco16 Cat] as cat
                              p inner join Cat#[span.text-deco17 .mate] as mate
                            td
                              p.mb-0 SELECT * FROM #[span.text-deco17 cat] cat
                              p INNER JOIN #[span.text-deco17 cat_mate] mate ON Cat#[span.text-deco17 .id] = mate#[span.text-deco17 .id]
                p Para más información sobre las características y particularidades del lenguaje de consulta de #[i Hibernate] HQL se invita a consultar en los anexos la guía oficial de este lenguaje.
                p.mb-5 A continuación, se muestran diferentes ejemplos haciendo uso de consultas por medio de HQL:
                .row.justify-content-center
                  .col-lg-10
                    .row
                      .col-12.bg-color11
                        img(src="@/assets/curso/tema1/img8.svg")
                      .col-12.bg-color10
                        .p-4
                          p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                          p #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                          p #[span.text-deco8 public class] #[span.text-deco10 CreateUserDemo] #[span.text-white {]
                          p.mb-0(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco10 void] #[span.text-deco13 main(]#[span.text-deco10 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                          p.mb-0(style="margin-left:40px") #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-deco10 Session] #[span.text-deco11 sesion] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 sesion]#[span.text-deco13 .beginTransaction()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Consultar todos los usuarios de la tabla Usuarios]
                          p.mb-0(style="margin-left:60px") #[span.text-deco10 List]#[span.text-white &lt;]#[span.text-deco10 Usuario]#[span.text-white &gt;] #[span.text-deco11 usuariosRegistrados] #[span.text-white =]  #[span.text-deco11 sesion]#[span.text-deco13 .createQuery(]#[span.text-deco14 “from Usuario”]#[span.text-deco13 )]#[span.text-deco13 .list()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nUsuarios registrados”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco12 for(]#[span.text-deco10 Usuario] #[span.text-deco11 u]#[span.text-white : usuariosRegistrados]#[span.text-deco12 )] #[span.text-white {]
                          p.mb-0(style="margin-left:80px") #[span.text-deco11 System.out]#[span.text-deco13 .println(#[span.text-white u])]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-white }]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Consultar todos los usuarios cuyo username es igual a Raul]
                          p.mb-0(style="margin-left:60px") #[span.text-white usuariosRegistrados =] #[span.text-deco11 sesion]#[span.text-deco13 .createQuery(]#[span.text-deco14 “from Usuario u where u.userName = ‘Raul’”]#[span.text-deco13 )]#[span.text-deco13 .getResultList()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nUsuarios registrados con username = Raul”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco12 for(]#[span.text-deco10 Usuario] #[span.text-deco11 u]#[span.text-white : usuariosRegistrados]#[span.text-deco12 )] #[span.text-white {]
                          p.mb-0(style="margin-left:80px") #[span.text-deco11 System.out]#[span.text-deco13 .println(#[span.text-white u])]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-white }]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Consultar todos los usuarios cuyo username es igual a Francisco o su password es 12345]
                          p.mb-0(style="margin-left:60px") #[span.text-white usuariosRegistrados =] #[span.text-deco11 sesion]#[span.text-deco13 .createQuery(]#[span.text-deco14 “from Usuario u where u.userName = ‘Francisco’ OR u.userPassword = ‘12345’”]#[span.text-deco13 )]#[span.text-deco13 .getResultList()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nUsuarios registrados con userName = Francisco o userPassword = 12345”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco12 for(]#[span.text-deco10 Usuario] #[span.text-deco11 u]#[span.text-white : usuariosRegistrados]#[span.text-deco12 )] #[span.text-white {]
                          p.mb-0(style="margin-left:80px") #[span.text-deco11 System.out]#[span.text-deco13 .println(#[span.text-white u])];
                          p.mb-0(style="margin-left:60px") #[span.text-white }]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Consultar todos los usuarios cuyo username inicia por la letra S]
                          p.mb-0(style="margin-left:60px") #[span.text-white usuariosRegistrados =] #[span.text-deco11 sesion]#[span.text-deco13 .createQuery(]#[span.text-deco14 “from Usuario u where u.userName LIKE ‘S%’”]#[span.text-deco13 ).getResultList()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nUsuarios registrados con userName que inicia con la letra S”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco12 for(]#[span.text-deco10 Usuario] #[span.text-deco11 u]#[span.text-white : usuariosRegistrados]#[span.text-deco12 )] #[span.text-white {]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(#[span.text-white u])]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-white }]
                          p(style="margin-left:60px") #[span.text-deco11 sesion]#[span.text-deco13 .getTransaction().commit()]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Proceso finalizado”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-white }]
                          p(style="margin-left:20px") #[span.text-white }]
                          p #[span.text-white }]
          div(titulo="Actualizaciones")
            .row
              .col-12
                p.mb-5 El proceso de actualización es muy similar al proceso de consulta ya que se puede hacer uso directo de los objetos obtenidos de las clases de entidad por medio de los métodos modificadores de sus atributos (Metodos #[i set()]) y confirmar las transacciones realizadas o también se puede hacer uso de #[i createQuery()] el cual permite enviar consultas HQL un poco más elaboradas pero asociándolo con el método #[i executeUpdate()] para que se reflejen los cambios en la base de datos una vez se confirma la transacción.
                .row.justify-content-center
                  .col-lg-10.mb-5
                    .row
                      .col-12.bg-color11
                        img(src="@/assets/curso/tema1/img8.svg")
                      .col-12.bg-color10
                        .p-4
                          p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                          p #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                          p #[span.text-deco8 public class] #[span.text-deco10 CreateUserDemo] #[span.text-white {]
                          p.mb-0(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco10 void] #[span.text-deco13 main(]#[span.text-deco10 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                          p.mb-0(style="margin-left:40px") #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                          p(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-deco10 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 sesion]#[span.text-deco13 .beginTransaction()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Actualizando el usuario de llave primaria igual a 6]
                          p.mb-0(style="margin-left:60px") #[span.text-deco10 Usuario] #[span.text-deco11 consultaUsuario] #[span.text-white =] #[span.text-deco11 session]#[span.text-deco13 .get(]#[span.text-deco11 Usuario.class]#[span.text-white ,] #[span.text-deco15 6]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 consultaUsuario]#[span.text-deco13 .setUserName(#[span.text-deco15 “Nuevo Raul”])]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nUsuario  “]#[span.text-white +]#[span.text-deco11 consultaUsuario]#[span.text-deco13 .getUserId()]#[span.text-white +] #[span.text-deco14 “ Actualizado!”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .getTransaction().commit()]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(#[span.text-deco14 “Proceso finalizado”])]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-white }]
                          p(style="margin-left:20px") #[span.text-white }]
                          p #[span.text-white }]
                  .col-lg-10
                    .row
                      .col-12.bg-color11
                        img(src="@/assets/curso/tema1/img8.svg")
                      .col-12.bg-color10
                        .p-4
                          p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                          p #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                          p #[span.text-deco8 public class] #[span.text-deco10 CreateUserDemo] #[span.text-white {]
                          p.mb-0(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco10 void] #[span.text-deco13 main(]#[span.text-deco10 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                          p.mb-0(style="margin-left:40px") #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                          p(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-deco10 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 sesion]#[span.text-deco13 .beginTransaction()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Actualizando el password Z@e34 a todos los usuario cuyo password actual sea 678]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nActualizando varios usuarios …”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .createQuery(]#[span.text-deco14 “update Usuario u set u.userPassword = ‘Z@e34’ where u.userPassword = ‘678’”]#[span.text-deco13 )]
                          p(style="margin-left:60px") #[Span.text-deco13 .executeUpdate()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .getTransaction().commit()]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Proceso finalizado”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-white }]
                          p(style="margin-left:20px") #[span.text-white }]
                          p #[span.text-white }]
          div(titulo="Método <i>Delete</i>")
            .row
              .col-12
                .row.justify-content-center
                  .col-lg-10
                    .cajon.color-primario.p-4.mb-5
                      p.mb-0 El método #[i delete()] del objeto session permite eliminar un registro de la base de datos por medio de un objeto recibido como parámetro para identificar el registro de la tabla a eliminar. La forma correcta de hacer un proceso de eliminación de un registro particular incluye los siguientes pasos:
                  .col-lg-10.mb-4.mb-lg-0
                    .row
                      .col-lg-7
                        .tarjeta-avatar-b.mb-4
                          .tarjeta-avatar-b__img
                            img(src='@/assets/curso/tema1/img17.svg' alt='AvatarTop')
                          .tarjeta.tarjeta--blanca
                            .p-4
                              br
                              p.mb-0 Iniciar una transacción por medio del método #[i beginTransaction()]
                              br
                        .tarjeta-avatar-b.mb-4
                          .tarjeta-avatar-b__img
                            img(src='@/assets/curso/tema1/img18.svg' alt='AvatarTop')
                          .tarjeta.tarjeta--blanca
                            .p-4
                              br
                              p.mb-0 Utilizar un mecanismo para obtener una instancia de la clase entidad con el objeto que referencia del registro a eliminar ya sea por medio del método #[i get()] o #[i CreateQuery].
                              br
                        .tarjeta-avatar-b.mb-4
                          .tarjeta-avatar-b__img
                            img(src='@/assets/curso/tema1/img20.svg' alt='AvatarTop')
                          .tarjeta.tarjeta--blanca
                            .p-4
                              br
                              p.mb-0 Invocar el método #[i delete()] del objeto de #[i session] pasando como parámetro el objeto que referencia el registro a eliminar.
                              br
                        .tarjeta-avatar-b.mb-4
                          .tarjeta-avatar-b__img
                            img(src='@/assets/curso/tema1/img19.svg' alt='AvatarTop')
                          .tarjeta.tarjeta--blanca
                            .p-4
                              br
                              p.mb-0 Confirmar la transacción realizada por medio del método #[i getTransaction().commit()]
                              br
                      .col-lg-5
                        img(src="@/assets/curso/tema1/img6.png" style="width: 450px").m-auto
                  .col-lg-10.mb-5
                    .row
                      .col-12.bg-color11
                        img(src="@/assets/curso/tema1/img8.svg")
                      .col-12.bg-color10
                        .p-4
                          p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                          p #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                          p #[span.text-deco8 public class] #[span.text-deco10 CreateUserDemo] #[span.text-white {]
                          p.mb-0(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco10 void] #[span.text-deco13 main(]#[span.text-deco10 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                          p.mb-0(style="margin-left:40px") #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                          p(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-deco10 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 sesion]#[span.text-deco13 .beginTransaction()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Eliminando el usuario cuyo id es 9]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Eliminacion de un usuario”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco10 Usuario] #[span.text-deco11 usuarioDelete] #[span.text-white =] #[span.text-deco11 session]#[span.text-deco13 .get(]#[span.text-deco11 Usuario.class]#[span.text-white ,] #[span.text-deco15 9]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .delete(]#[span.text-deco15 usuarioDelete]#[span.text-deco13 )]#[span.text-white ;]
                          p(style="margin-left:80px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “\nUsuario “]#[span.text-white +]#[span.text-deco11 usuarioDelete]#[span.text-deco13 .getUserName()]#[span.text-white +]#[span.text-deco14 ” eliminado”]#[span.text-deco13 )]#[pan.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .getTransaction().commit()]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Proceso finalizado”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-white }]
                          p(style="margin-left:20px") #[span.text-white }]
                          p #[span.text-white }]
                  .col-lg-10
                    .row
                      .col-12.bg-color11
                        img(src="@/assets/curso/tema1/img8.svg")
                      .col-12.bg-color10
                        .p-4
                          p.mb-0 #[span.text-deco8 import] #[span.text-white java.util.List;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.Session;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.SessionFactory;]
                          p.mb-0 #[span.text-deco8 import] #[span.text-white org.hibernate.cfg.Configuration;]
                          p #[span.text-deco8 import] #[span.text-white com.jonathan.hibernate.demo.entity.Usuario;]
                          p #[span.text-deco8 public class] #[span.text-deco10 CreateUserDemo] #[span.text-white {]
                          p.mb-0(style="margin-left:20px") #[span.text-deco8 public static] #[span.text-deco10 void] #[span.text-deco13 main(]#[span.text-deco10 String[]] #[span.text-deco11 args]#[span.text-deco13 )] #[span.text-white {]
                          p.mb-0(style="margin-left:40px") #[span.text-deco10 SessionFactory] #[span.text-deco11 factory] #[span.text-white =] #[span.text-deco12 new] #[span.text-deco13 Configuration()]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .configure(]#[span.text-deco14 “hibernate.cfg.xml”]#[span.text-deco13 )]
                          p.mb-0(style="margin-left:60px") #[span.text-deco13 .addAnnotatedClass(]#[span.text-deco11 Usuario.class]#[span.text-deco13 )]
                          p(style="margin-left:60px") #[span.text-deco13 .buildSessionFactory()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-deco10 Session] #[span.text-deco11 session] #[span.text-white =] #[span.text-deco11 factory]#[span.text-deco13 .getCurrentSession()]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-deco12 try] #[span.text-white {]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 sesion]#[span.text-deco13 .beginTransaction()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco9 //Eliminando todos los usuarios cuyo id es 8]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 "\nEliminando el usuario 8 ..."]#[span.text-deco13 )]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .createQuery(]#[span.text-deco14 "delete from Usuario u where u.userId = 8"]#[span.text-deco13 )]#[span.text-deco13 .executeUpdate()]#[span.text-white ;]
                          p.mb-0(style="margin-left:60px") #[span.text-deco11 session]#[span.text-deco13 .getTransaction().commit()]#[span.text-white ;]
                          p(style="margin-left:60px") #[span.text-deco11 System.out]#[span.text-deco13 .println(]#[span.text-deco14 “Proceso finalizado”]#[span.text-deco13 )]#[span.text-white ;]
                          p.mb-0(style="margin-left:40px") #[span.text-white }]#[span.text-deco12 finally] #[span.text-white {]
                          p(style="margin-left:60px") #[span.text-deco11 factory]#[span.text-deco13 .close()]#[span.text-white ;]
                          p(style="margin-left:40px") #[span.text-white }]
                          p(style="margin-left:20px") #[span.text-white }]
                          p #[span.text-white }]
    .row.bg-color3
      .col-12.px-5
        .row
          .col-lg-5
            img(src="@/assets/curso/tema1/img7.png" style="width: 470px").m-auto
          .col-lg-6
            .row.my-4
              .col-12.bg-color2
                .p-4
                  p.mb-0 A continuación, se muestran  video de clases practicando cada una de las operaciones básicas necesarias para la realización de un CRUD en una tabla de la base de datos.
            .tarjeta.color-primario.p-3.mb-4.ms-0.ms-lg-5
              .row.justify-content-around.align-items-center
                .col-3.col-sm-2.col-lg-2
                  img(src="@/assets/curso/tema1/img21.svg")
                .col
                  .row.justify-content-between.align-items-center
                    .col.mb-3.mb-sm-0
                      h3.mb-1.text-white Método #[i save]
                      p.text-small.text-white Estimado aprendiz, para profundizar sobre el tema puede consultar el siguiente video.
                    .col-sm-auto
                      a.boton.color-acento-contenido.texto-blanco(href="https://www.youtube.com/watch?v=_vElkMY1nOg" target="_blank")
                        span(style="color:#000000 !important") Ver video
            .tarjeta.color-primario.p-3.mb-4.ms-0.ms-lg-5
              .row.justify-content-around.align-items-center
                .col-3.col-sm-2.col-lg-2
                  img(src="@/assets/curso/tema1/img21.svg")
                .col
                  .row.justify-content-between.align-items-center
                    .col.mb-3.mb-sm-0
                      h3.mb-1.text-white Consultas
                      p.text-small.text-white Estimado aprendiz, para profundizar sobre el tema puede consultar el siguiente video.
                    .col-sm-auto
                      a.boton.color-acento-contenido.texto-blanco(href="https://www.youtube.com/watch?v=JgiGWa_cPA8" target="_blank")
                        span(style="color:#000000 !important") Ver video
            .tarjeta.color-primario.p-3.ms-0.ms-lg-5
              .row.justify-content-around.align-items-center
                .col-3.col-sm-2.col-lg-2
                  img(src="@/assets/curso/tema1/img21.svg")
                .col
                  .row.justify-content-between.align-items-center
                    .col.mb-3.mb-sm-0
                      h3.mb-1.text-white #[i Update] y #[i Delete]
                      p.text-small.text-white Estimado aprendiz, para profundizar sobre el tema puede consultar el siguiente video.
                    .col-sm-auto
                      a.boton.color-acento-contenido.texto-blanco(href="https://www.youtube.com/watch?v=QiL6l9qMVWE" target="_blank")
                        span(style="color:#000000 !important") Ver video
    separador
    #t_1_2
    .titulo-segundo.color-secundario
      h2 1.2	Asociaciones
    .row.bg-color3.mb-5
      .col-12.px-5
        .row
          .col-lg-7.mb-4.mb-lg-0
            p.mt-4 Normalmente al desarrollar una aplicación que gestione una base de datos, se requiere mucho más que una única tabla para hacer la gestión de la información en la base de datos, por lo que es común tener modelos de datos con múltiples tablas relacionadas con asociaciones de diferentes tipos y diferentes cardinalidades. Por lo cual es importante establecer en las clases de entidad este tipo de relaciones para que el proceso de mapeo sea coherente. Los tipos de asociaciones más comúnmente utilizadas son las que expresan relaciones uno a uno, relaciones uno a muchos, relaciones mucho a uno y relaciones muchos a muchos.
            .cajon.color-primario.p-4.bg-color14
              p.mb-0 Para mostrar cada uno de estos casos utilizaremos como referencia el siguiente modelo de datos que ya fue mapeado de forma individualizada y a medida que se agrega una asociación de diferente tipo se establecerán los cambios que debería estar presentes, y que se presenta en la siguiente figura:
          .col-lg-5
            img(src="@/assets/curso/tema1/img8.png" style="width: 570px").m-auto
    .row.justify-content-center.mb-5
      .col-lg-11.bg-color15#menu1
        img(src="@/assets/curso/tema1/img22.svg" style="width: 1200px").m-auto(data-aos="slide-right")
    .row.justify-content-evenly
      .col-5.col-lg-4.mb-3.mb-lg-0
        a(href="#1A")
          figure.efect1
            img(src="@/assets/curso/tema1/img23.svg", style="width:300px").m-auto
      .col-5.col-lg-4.mb-3.mb-lg-0
        a(href="#2A")
          figure.efect1
            img(src="@/assets/curso/tema1/img24.svg", style="width:300px").m-auto
      .col-5.col-lg-3
        a(href="#3A")
          figure.efect1
            img(src="@/assets/curso/tema1/img25.svg", style="width:300px").m-auto
    hr
    #1A
    br
    .row.py-5.align-items-center.justify-content-between
      .col-6.col-lg-4
        h3.text-white.mb-0.text-deco1 #[b Relaciones #[i OneToOne]]
      .col-2
        a(href="#menu1")
          figure.efect1
            img(src="@/assets/curso/tema1/img26.svg", style="width:50px").m-auto
    .row.bg-color3
      .col-12.px-5
        .row
          .col-lg-5
            img(src="@/assets/curso/tema1/img9.png" style="width: 470px").m-auto
          .col-lg-6
            p.mt-4 En este tipo de relaciones queremos expresar un vínculo en el que un ejemplar de una tabla tiene relación con un y solo un ejemplar de una segunda tabla. Desde el punto de vista de las bases de datos se creará una relación de integridad referencial vinculando una llave primaria con una llave foránea. Tomando como consideración el modelo de datos presentado anteriormente supongamos que se desea indicar que un usuario tiene asociado un recurso. Para resolver este nuevo requerimiento debemos modificar la clase de entidad de usuario para agregar un nuevo atributo que haga referencia al objeto recurso con el cual está relacionado y agregar la anotación correspondiente llamada @OneToOne de forma que Hibernate haga el mapeo correcto.  El esquema se presenta a continuación en la siguiente figura:
    .row.bg-color15
      .col-12
        .p-4
          img(src="@/assets/curso/tema1/img27.svg" style="width: 1200px").m-auto.my-5(data-aos="slide-left")
    .cajon.color-primario.p-4
      p.mb-0 Mientras que en la base de datos se debe agregar un nuevo campo foráneo en la tabla usuario que haga referencia a la llave primaria de la tabla recurso para poder establecer la relación, en las clases de tipo entidad bastará con especificar el nuevo atributo del tipo de objeto correspondiente que referencia agregando de la anotación de tipo @OneToOne. Si el campo nuevo requerido en la tabla usuario no existe el mapeador de #[i Hibernate] se encargará de agregarlo.
    hr
    #2A
    br
    .row.py-5.align-items-center.justify-content-between
      .col-9.col-lg-4
        h3.text-white.mb-0.text-deco1 #[b Relaciones #[i OneToMany] - #[i ManyToOne]]
      .col-2
        a(href="#menu1")
          figure.efect1
            img(src="@/assets/curso/tema1/img26.svg", style="width:50px").m-auto
    .row.bg-color3
      .col-12.px-5
        .p-4
          .row.align-items-center
            .col-12.tarjeta--blanca.mb-4
              p Las relaciones #[i OneToMany] tiene la particularidad de afectar cada una de las entidades vinculadas en la relación y es importante identificar el lugar que es una relación #[i OneToMany] y en qué lugar la relación es #[i ManyToOne].
            .col-lg-6
              p Recordando las reglas de transformación del modelo lógico de una base de datos relacional en este tipo de relaciones se indica que en la tabla del lado de la relación donde la cardinalidad máxima muchos (*) deberá ser transferido como un campo foráneo la llave primaria de la tabla donde la cardinalidad máxima es 1, como se aprecia en la siguiente figura:
            .col-lg-6
              img(src="@/assets/curso/tema1/img10.png" style="width: 490px").m-auto
    .row.bg-color15
      .col-12
        .p-4
          img(src="@/assets/curso/tema1/img28.svg" style="width: 1200px").m-auto.my-5(data-aos="slide-right")
    .cajon.color-primario.p-4
      .row.align-items-center
        .col-lg-4.mb-4.mb-lg-0
          img(src="@/assets/curso/tema1/img29.svg" style="width: 450px").m-auto
        .col-lg-8
          p.mb-0 Para el caso de las clases de entidad deberá especificarse en la clase donde la cardinalidad máxima es 1, un atributo del tipo lista de la clase de entidad con la que tiene un vínculo @OneToMany, este atributo será de tipo lista porque se está vinculando con varios. En el ejemplo, la entidad usuario se relaciona con varios recursos, es decir un usuario puede estar vinculado con múltiples recursos. Por otra parte, la clase de entidad donde la cardinalidad máxima es muchos deberá especificar un atributo de tipo objeto con la entidad vinculada agregándole la anotación @ManyToOne. En el ejemplo un recurso estará siempre vinculado con un único usuario. Es importante anexar en la entidad de cardinalidad @OneToMany el nombre del atributo en la entidad @ManyToOne que será usada para el mapeo de la asociación por parte de Hibernate. En el ejemplo se le indica en la entidad Usuario que la relación @OneToMany será mapeada usando el atributo user de la entidad @ManyToOne.
    hr
    #3A
    br
    .row.py-5.align-items-center.justify-content-between
      .col-6.col-lg-4
        h3.text-white.mb-0.text-deco1 #[b Relaciones #[i ManyToMany]]
      .col-2
        a(href="#menu1")
          figure.efect1
            img(src="@/assets/curso/tema1/img26.svg", style="width:50px").m-auto
    .row.bg-color3.mb-5
      .col-12.px-5
        .row
          .col-lg-5
            img(src="@/assets/curso/tema1/img11.png" style="width: 430px").m-auto
          .col-lg-7.mb-4.mb-lg-0
            p.mt-4 Las relaciones #[i ManyToMany] obligan a la construcción de una nueva entidad de mapeo en la cual se alojarán las respectivas llaves primarias de las entidades vinculadas por medio de la relación @ManyToMany. Para su correcta implementación deberán agregarse en cada una de las clases entidad un objeto de tipo lista de la entidad a la cual está relacionada etiquetada con la anotación @ManyToMany. Adicionalmente en una de las clases de entidad deberá especificar el objeto de mapeo del otro extremo que será utilizado por #[i Hibernate] para realizar la asociación.
            .cajon.color-primario.p-4.bg-color13
              p.mb-0 En el ejemplo siguiente, se establece una relación #[i ManyToMany] entre la clase Usuario y la clase Recurso por lo cual en cada una de ellas se agrega la correspondiente lista del tipo de entidad a la cual se asocian con la anotación @ManyToMany. En el caso de la clase Usuario se agrega el atributo de tipo lista de Recursos llamado recursos para indicar que un usuario puede estar vinculado con muchos recursos y por el lado de la clase Recursos se agrega una lista de tipo Usuario para indicar que un recurso puede estar vinculado con múltiples usuarios. Adicionalmente la relación entre usuario y recurso se mapea con el objeto #[i users] presente en la clase Recurso. La relación entre recurso y usuario no se mapea explícitamente por lo que generará la tabla intermedia recurso_usuario, lo cual cumple las reglas de transformación de un modelo lógico para una relación de muchos a muchos.
    .row.bg-color15
      .col-12
        .p-4
          img(src="@/assets/curso/tema1/img30.svg" style="width: 1200px").m-auto.mt-5(data-aos="slide-right")
    separador
    #t_1_3
    .titulo-segundo.color-secundario
      h2 1.3 Ciclo de vida
      p.my-5 Los objetos manipulados por Hibernate para el proceso de gestión de la persistencia pasa por cuatro estados diferentes, a continuación, se describe cada uno de ellos:
    .row.bg-color16.mb-5
      .col-12.px-5
        .row.align-items-center
          .col-lg-5
            img(src="@/assets/curso/tema1/img31.svg" style="width: 490px").m-auto
          .col-lg-7
            SlyderA
              .row.justify-content-center
                .col-8.bg-color17
                  .p-5
                    img(src="@/assets/curso/tema1/img32.svg" style="width: 100px").m-auto.mb-4
                    h4 Estado transitorio
                    p Corresponde al primer estado de un objeto de entidad y sucede cuando instanciamos y manipulamos el objeto de tipo entidad sin conectarlo por medio de la sesión a un registro de la base de datos. Así cualquier manipulación de este objeto no afecta la base de datos. En este estado un objeto de tipo entidad se comporta como cualquier otro objeto JAVA.
              .row.justify-content-center
                .col-8.bg-color17
                  .p-5
                    img(src="@/assets/curso/tema1/img33.svg" style="width: 100px").m-auto.mb-4
                    h4 Estado persistente
                    p Corresponde al estado que logra el objeto una vez se conecta con una sesión de Hibernate, lo cual ocurre cuando se invoca por ejemplo una operación de tipo #[i save()] o cuando el objeto fue producto de realizar un proceso de consulta a la base de datos por un método #[i get()]. Todos los cambios que se realizan sobre un objeto en estado persistente son observados por #[i Hibernate] y podrán eventualmente realizar modificaciones en la base de datos.
              .row.justify-content-center
                .col-8.bg-color17
                  .p-5
                    img(src="@/assets/curso/tema1/img34.svg" style="width: 100px").m-auto.mb-4
                    h4 Estado independiente
                    p A este estado pasan los objetos en estado persistentes una vez se realiza un cierre de sesión y en este momento son dejados de observar por #[i Hibernate] y cualquier cambio no será propagado en la base de datos. Un objeto independiente puede volver a ser persistente una vez se vuelva a abrir una nueva sesión y se use uno de los siguientes métodos #[i save()] o #[i merge()].
              .row.justify-content-center
                .col-8.bg-color17
                  .p-5
                    img(src="@/assets/curso/tema1/img35.svg" style="width: 100px").m-auto.mb-4
                    h4 Estado eliminado
                    p Es el último estado en el ciclo de vida de un objeto de tipo entidad y ocurre cuando el objeto en cuestión es eliminado de la base de datos por medio del método #[i delete()]. Cualquier cambio realizado sobre este objeto no afectará la base de datos.
    .cajon.color-primario.p-4.mb-5
      p.mb-0 A continuación, se muestra un resumen de los estados del ciclo de vida y sus transiciones completas con todos los posibles métodos.
    img(src="@/assets/curso/tema1/img36.svg" style="width: 1200px").m-auto

</template>

<script>
export default {
  name: 'Tema1',
  data: () => ({
    // variables de vue
  }),
  mounted() {
    this.$nextTick(() => {
      this.$aosRefresh()
    })
  },
  updated() {
    this.$aosRefresh()
  },
}
</script>

<style lang="sass"></style>
