<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    .titulo-principal.color-acento-contenido(data-aos="flip-up")
      .titulo-principal__numero
        span 2
      h1 #[i Spring]
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-0
        .row
          .col-lg-6
            img(src="@/assets/curso/tema2/img1.png").m-auto
          .col-lg-6
            .row
              .col-12
                .p-4
                  p.mb-4 Es un #[I Framework] de código abierto que facilita crear aplicaciones empresariales de alto rendimiento en JAVA, además de JAVA tiene soporte para los lenguajes #[i Groovy] y #[i Kotlin]. La estructura que lo compone es modular esta estructura cuenta con una flexibilidad para implementar una variedad de arquitecturas dependiendo de los requerimientos de las aplicaciones haciendo que la programación sea lo más hacedera posible, rápida y muy segura.
                  .row.mb-4.bg-color4.justify-content-end
                    .col-12
                      img(src="@/assets/curso/tema1/img2.svg" style="width: 50px; margin-left:40px")
                    .col-10
                      .p-2
                        p.text-white Historia: Rod Johnson creador de #[i Spring] se da cuenta que necesitan una herramienta para simplificar y facilitar la construcción de aplicaciones JEE utilizando EJB y escribe el libro expert #[i one-on-one] J2EE #[i Development] que es un conjunto de buenas prácticas para la creación de aplicaciones empresariales y en el año 2004 lanza primera versión 1.2.6 de #[i Spring], según el autor era el inicio de J2EE tradicional.
                        .row.align-items-center
                          .col-10.d-inline
                            p.text-white.text-end.mb-0 #[b Johnson, ( 2004)]
                          img(src="@/assets/curso/tema1/img3.svg" style="width: 40px")
                  p La siguiente figura muestra las Versiones de #[i Spring Framework]:
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Versiones de #[i Spring Framework]
    img(src="@/assets/curso/tema2/img2.png" style="width: 1000px").m-auto.mb-5(data-aos="slide-right")
    p.mb-5 Unas de las características principales de #[i Spring] son:
    .row
      .col-lg-6.mb-4.mb-lg-0
        LineaTiempoD.color-primario
          .row(numero="1" titulo="Flexibilidad")
            .col-12
              p Contiene un grupo flexible de librerías y extensiones de terceros de #[i Spring] facilitando a los desarrolladores construir aplicaciones fácilmente.
          .row(numero="2" titulo="Inyección de dependencia (DI)")
            .col-12
              p Ofrece un patrón que permite ayudar en el acoplamiento bajo, esto quiere decir que cuando existe dependencias entre las clases y se necesita crear un objeto de esta clase lo que hace #[i spring] es suministrar este objeto obteniendo beneficios en la modularidad, escalabilidad y dependencia de clases.
          .row(numero="3" titulo="POJOs (Plan <i>Old Java Objects</i>):")
            .col-12
              p Facilita un sencillo desarrollo por medio de los POJOs.
          .row(numero="4" titulo="ORM (<i>Object Relational Mapping</i>)")
            .col-12
              p Suministra un fácil acceso a datos por medio del ORM.
          .row(numero="5" titulo="Estructura y módulos")
            .col-12
              p #[i Spring] integra una variedad de módulos que se pueden integrar para el desarrollo de las aplicaciones.
      .col-lg-6
        img(src="@/assets/curso/tema2/img1.svg" style="width: 470px").m-auto(data-aos="slide-left")
    .row.bg-color16.mb-5
      .col-12.px-5
        .row.justify-content-center
          .col-12.mb-4.mt-3
            .p-4
              p.mb-0 La siguiente figura nos muestra lo que se puede crear con #[i Spring Framework]: Aplicaciones de consola, Aplicaciones de escritorio, Aplicaciones Web, Aplicaciones Móviles, Servicios SOAP, REST. #[i Spring] está orientado esencialmente al #[i backend].
          .col-10
            .row.justify-content-evenly.mb-0.mb-lg-4
              .col-11.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img2.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img3.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Microservicios
                      p.text-center Permite crear y ejecutar microservicios en producción a escala
              .col-11.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img4.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img5.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Nube
                      p.text-center Ejecución de servicios en la nube
              .col-11.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img6.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img7.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Aplicaciones #[i web]
                      p.text-center Creación rápida de aplicaciones #[i web]
            .row.justify-content-evenly
              .col-11.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img8.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img9.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center #[i Reactive]
                      p.text-center Permite la creación de proyectos reactivos basados en mensajes
              .col-11.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img10.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img11.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center #[i Servlets]
                      p.text-center Permite la ejecución de código impulsado por eventos se encarga del escalado y la seguridad del lado del servidor
              .col-11.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img12.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img13.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center #[i Batch]
                      p.text-center Aplicaciones de procesamiento de datos en lote
    #t_2_1
    .titulo-segundo.color-secundario
      h2 2.1 Introducción
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-0
        .row.align-items-center
          .col-lg-6
            img(src="@/assets/curso/tema2/img3.png").m-auto
          .col-lg-6
            .row
              .col-12.mt-5.bg-color12
                .p-4
                  p.mb-0 El #[i Framework Spring] básicamente con su inyección de dependencias se encarga de construir objetos y configurar todas las dependencias que estos necesiten. En #[i Spring] estos objetos que son creados son llamados #[i beans] que son anotaciones que son agregadas a las clases así: @component, @Service, @Repository etc. Uno de los principios principales de #[i Spring] es el de Inversión de Dependencia (DIP) el cual habla de que los módulos de alto nivel no deben depender de los de bajo nivel, lo que quiere decir es que hay que hacer más referencia a las abstracciones que a las implementaciones por lo que no se debe depender de una clase ni de una implementación en particular. La implementación de este principio es llamado Inversión de Control (IOc) que se encarga de desacoplar el código utilizando eventos, también es llamado como el principio de #[i Hollywood] “no nos llames; nosotros te llamaremos”, que consisten en una manera de programar donde la aplicación es quien interviene en cambio del código, para realizar la implementación del IOc se necesita un agente externo que recibe el nombre de contenedor quién es el encargado de verificar el flujo de la aplicación. Los IOc utilizan #[i Service locator], Eventos y los DI (Inyecciones de dependencias) enfocando el #[i Spring Framework] en la DI.
              .col-12.mt-2.mt-lg-5
                .p-4
                  p #[b Inyección de Dependencias]: es un patrón de diseño de #[i software], subtipo de inversión de control cuyo objetivo es tener un código fácil de mantener o desacoplado. Su función es determinar lo que los objetos necesitan.
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Principio inversión de control
    .row.bg-color15
      .col-12
        .p-4
          img(src="@/assets/curso/tema2/img15.svg" style="width: 800px").m-auto.mt-5(data-aos="slide-right")
    p.mb-5  A continuación, se muestra un ejemplo de código donde los objetos dependen entre sí:
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Acoplamiento hermético
    .row.align-items-center.mb-5
      .col-lg-4.mb-4.mb-lg-0
        img(src="@/assets/curso/tema2/img16.svg" style="width: 470px").m-auto
      .col-lg-4
        img(src="@/assets/curso/tema2/img17.svg" style="width: 200px").m-auto
        .cajon.color-primario.p-4.my-2
          p.mb-0 En el ejemplo anterior se muestra un código de una tienda de café que solicita cambiar el tipo de café y como se puede ver se realiza el cambio de café dentro de la propia clase controlando esta sus propias dependencias. La intención es obtener un acoplamiento suelto o desacoplamiento donde no exista una dependencia entre los objetos. En el siguiente ejemplo se puede ver cómo se realiza:
        img(src="@/assets/curso/tema2/img18.svg" style="width: 200px").m-auto
      .col-lg-4.mt-4.mt-lg-0
        img(src="@/assets/curso/tema2/img19.svg" style="width: 470px").m-auto
    img(src="@/assets/curso/tema2/img4.png" style="width: 1300px").m-auto
    .row.justify-content-center
      .col-10.bg-color8
        .p-4
          p.mb-0 En el código anterior se puede observar que se obtuvo el objeto desde el exterior y que el objeto puede ser cualquier tipo de café, sin necesidad de tocar la clase TiendaCafe.
    .row.align-items-center.mb-5
      .col-lg-6
        .row
          .col-12.my-4.bg-color14.tarjeta--azul
            .p-4
              p.mb-0 Resumiendo, la inversión de control es un patrón de programación para obtener un acoplamiento flexible logrando que los objetos independientes no sean responsables de sus dependencias sino que sean recibidas desde afuera; el contenedor de IOc recoge los metadatos que vienen de un archivo XML, o código JAVA, y recibe las indicaciones de los objetos que debe crearlos, enlazarlos, configurarlos y destruirlos por medio de POJOs (Objetos simples de Java) creando objetos por medio del proceso que recibe el nombre de #[i Spring Beans] y resultando objetos preparados para la inyección de dependencia.
        p La siguiente figura evidencia el funcionamiento de una vista abstracta de #[i Spring].
      .col-lg-6
        img(src="@/assets/curso/tema2/img5.png" style="width: 570px").m-auto
    .row.align-items-center.mb-5
      .col-lg-6.tarjeta--azul
        .p-4
          img(src="@/assets/curso/tema2/img20.svg" style="width: 570px").m-auto(data-aos="slide-right")
      .col-lg-6.mt-4.mt-lg-0
        p.mb-4 En el video se explican aspectos generales de la inyección de dependencias:
        .tarjeta.color-primario.p-3.mb-4
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-2
              img(src="@/assets/curso/tema1/img21.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1.text-white Inyección de dependencias
                  p.text-small.text-white Estimado aprendiz, para profundizar sobre el tema puede consultar el siguiente video.
                .col-sm-auto
                  a.boton.color-acento-contenido.texto-blanco(href="https://www.youtube.com/watch?v=31vCOJRBR7s" target="_blank")
                    span(style="color:#000000 !important") Ver video
        p #[b Módulos del #[i Framework]]: #[i Spring Framework] es un marco de trabajo muy amplio y brinda cerca de 20 módulo los cuales se asocian en el contenedor principal, “Accesos e integración de datos, #[i Web], AOP (Programación orientada a aspectos, Instrumentación, Mensajes y Pruebas)” (#[i Spring] ,2021).
        p Para trabajar con #[i Spring] se necesita tener instalado los siguientes requerimientos:
        ul.lista-ul.ms-3
          li 
            i.fas.fa-layer-group(style="color: #039BE5")
            | 
            p.mb-0 #[b Un entorno de desarrollo (IDE)] se puede seleccionar cualquiera de los relacionados en la tabla No 1.
          li 
            i.fas.fa-layer-group(style="color: #039BE5")
            |
            p.mb-0 #[b Un JDK (Kit de desarrollo de JAVA)] se puede descargar cualquiera de los relacionados en la tabla No 2.
    .row.justify-content-center.mb-5
      .col-lg-8.mb-5
        .titulo-sexto.color-acento-contenido
          p.mb-0 #[b Tabla 1.] Entornos para desarrollo en #[i Spring]
        .tabla-a.color-acento-botones1
          table
            thead
              tr
                th(width="30%") Entornos de desarrollo
                th Enlace
            tbody
              tr(style="background-color: #FFFFFF")
                td IntelliJ IDEA
                td #[a(href="https://www.jetbrains.com/idea/" target="blank") https://www.jetbrains.com/idea/]
              tr(style="background-color: #E8E8E8")
                td Spring Tools
                td #[a(href="https://spring.io/tools" target="blank") https://spring.io/tools]
              tr(style="background-color: #FFFFFF")
                td Visual Studio Code
                td #[a(href="https://code.visualstudio.com/docs/languages/java" target="blank") https://code.visualstudio.com/docs/languages/java]
              tr(style="background-color: #E8E8E8")
                td Eclipse
                td #[a(href="https://www.eclipse.org/downloads/packages/" target="blank") https://www.eclipse.org/downloads/packages/]
              tr(style="background-color: #FFFFFF")
                td NetBeans
                td #[a(href="https://netbeans.apache.org/" target="blank") https://netbeans.apache.org/]
      .col-lg-8
        .titulo-sexto.color-acento-contenido
          p.mb-0 #[b Tabla 2.] JDK para desarrollo en #[i Spring]
        .tabla-a.color-acento-botones1
          table
            thead
              tr
                th(width="30%") JDK
                th Enlace
            tbody
              tr(style="background-color: #FFFFFF")
                td JDK Oracle
                td #[a(href="https://www.oracle.com/java/technologies/downloads/" target="blank") https://www.oracle.com/java/technologies/downloads/]
              tr(style="background-color: #E8E8E8")
                td AdoptOpenJDK
                td #[a(href="https://adoptopenjdk.net/" target="blank") https://adoptopenjdk.net/]
    p.mb-5 Para construir aplicaciones en #[i Spring Framework] necesitamos:
    AcordionA(tipo="a" clase-tarjeta="tarjeta tarjeta--azul")
      .row(titulo="Elegir jars con <i>Maven</i>")
        .col-12
          p.mb-5 Lo primero que se debe hacer es la creación de un proyecto #[i Maven] o #[i Gradle] y realizar la descarga de las dependencias necesarias.
          .titulo-sexto.color-acento-contenido
            p.mb-0 #[b Figura 1.] Creación proyecto #[i Maven]
          img(src="@/assets/curso/tema2/img6.png" style="width: 900px").m-auto.mb-5
          p.mb-5 Configuración de las dependencias en el archivo pom.XML
          .titulo-sexto.color-acento-contenido
            p.mb-0 #[b Figura 2.] Configuración dependencias
          img(src="@/assets/curso/tema2/img7.png" style="width: 900px").m-auto.mb-5
          p.mb-5 Las dependencias se deben visualizar en la carpeta Dependencias
          .titulo-sexto.color-acento-contenido
            p.mb-0 #[b Figura 3.] Dependencias
          img(src="@/assets/curso/tema2/img8.png" style="width: 900px").m-auto
      .row(titulo="Creación de la Aplicación")
        .col-12
          p.mb-5 Para el ejemplo se creará un programa con el ejemplo de HolaPlaneta.
          .row.justify-content-center
            .col-lg-8
              .row
                .col-12.bg-color11
                  img(src="@/assets/curso/tema1/img8.svg")
                .col-12.bg-color10
                  .p-4
                    p.mb-0 #[span.text-deco18 public interface] #[span.text-deco19 HolaPlaneta] #[span.text-white {]
                    p.mb-0(style="margin-left:20px") #[span.text-deco20 void] #[span.text-deco19 enviarSaludo] #[span.text-white ();]
                    p #[span.text-white }]
                    p.mb-0 #[span.text-deco18 public class] #[span.text-deco19 HolaPlanetaIpml] #[span.text-deco18 implements] #[span.text-white HolaPlaneta {]
                    p.mb-0(style="margin-left:20px") #[span.text-white @Override]
                    p.mb-0(style="margin-left:20px") #[span.text-deco18 public] #[span.text-deco20 void] #[span.text-deco19 enviarSaludo] #[span.text-white () {]
                    p.mb-0(style="margin-left:40px") #[span.text-deco21 System]#[span.text-deco11 .out.println]#[span.text-white (]#[span.text-deco14 “Hola Planeta estamos en Spring Framework”]#[span.text-white );]
                    p.mb-0(style="margin-left:20px") #[span.text-white }]
                    p #[span.text-white }]
      .row(titulo="Configurar archivo XML")
        .col-12
          p.mb-5 Una vez se tenga la aplicación se realizará la configuración en el archivo springXMLconfig.
          .row.justify-content-center
            .col-lg-8.mb-5
              .row
                .col-12.bg-color11
                  img(src="@/assets/curso/tema1/img8.svg")
                .col-12.bg-color10
                  .p-4
                    p.mb-0 #[span.text-deco11 &lt;beans xmlns=]#[span.text-deco14 “http://www.springframework.org/schema/beans”]
                    p.mb-0(style="margin-left:20px") #[span.text-deco11 xmlns:xsi=]#[span.text-deco14 “http://www.w3.org/2001/XMLSchema-instance”]
                    p.mb-0(style="margin-left:20px") #[span.text-deco11 xsi:schemaLocation=]#[span.text-deco14 “http://www.springframework.org/schema/beans http://www.springframework.org/schema/beans/spring-beans-4.3.xsd”&gt;]
                    p.mb-0(style="margin-left:20px") #[span.text-deco11 &lt;bean id=]#[span.text-deco14 “saludaService”] #[span.text-deco11 class=]#[span.text-deco14 “sena.spring.introduccion.HelloPlanetaImpl”]#[span.text-deco11 /&gt;]
                    p #[span.text-deco11 &lt;/beans&gt;]
            p.mb-5 A continuación, se muestra un nuevo ejemplo de código explicando más a detalle el uso del Contenedor en #[i Spring]. Para el siguiente ejemplo se tiene un proyecto llamado “Sena” el cual tiene una clase aprendiz con los siguientes atributos:
            .col-lg-8.mb-5
              .row
                .col-12.bg-color11
                  img(src="@/assets/curso/tema1/img8.svg")
                .col-12.bg-color10
                  .p-4
                    p.mb-0.text-deco21 package com.sena
                    p.mb-0.text-deco21 public class AprendizBean {
                    p.mb-0.text-deco21(style="margin-left:20px") private String primernombre;
                    p.mb-0.text-deco21(style="margin-left:20px") private String apellidos;
                    p(style="margin-left:20px").text-deco21 private String cedula; 
                    p.mb-0(style="margin-left:20px").text-deco21 public String getPrimerNombre () {
                    p.mb-0(style="margin-left:20px").text-deco21 return primernombre;
                    p(style="margin-left:20px").text-deco21 } 
                    p.mb-0(style="margin-left:20px").text-deco21 public void setPrimerNombre (String nombre) {
                    p.mb-0(style="margin-left:20px").text-deco21 this.primernombre = nombre;
                    p(style="margin-left:20px").text-deco21 } 
                    p.mb-0(style="margin-left:20px").text-deco21 public String getApellidos () {
                    p.mb-0(style="margin-left:20px").text-deco21 return apellidos;
                    p(style="margin-left:20px").text-deco21 } 
                    p.mb-0(style="margin-left:20px").text-deco21 public void setApellidos (String apellidos) {
                    p.mb-0(style="margin-left:20px").text-deco21 this.apellido = apellidos;
                    p(style="margin-left:20px").text-deco21 } 
                    p.mb-0(style="margin-left:20px").text-deco21 public String getCedula () {
                    p.mb-0(style="margin-left:20px").text-deco21 return cedula;
                    p(style="margin-left:20px").text-deco21 }
                    p.mb-0(style="margin-left:20px").text-deco21 public void setCedula (String cedula) {
                    p.mb-0(style="margin-left:20px").text-deco21 this.cedula = cedula;
                    p(style="margin-left:20px").text-deco21 } 
                    p.mb-0(style="margin-left:20px").text-deco21 public void verAprendiz () {
                    p.mb-0(style="margin-left:20px").text-deco21 System.out.println(primernombre+” “+apellidos+”, es la actual estudiante”);
                    p(style="margin-left:20px").text-deco21 }
                    p.text-deco21 }
            p.mb-5 Al utilizar este proyecto Sena #[i Spring framework] cuenta con un archivo XML que gestiona objetos (#[i Spring] IOC #[i Container]) para este proyecto recibe el nombre de springconfig.xml y se ve de la siguiente manera.
            .col-lg-8.mb-5
              .row
                .col-12.bg-color11
                  img(src="@/assets/curso/tema1/img8.svg")
                .col-12.bg-color10
                  .p-4
                    p.text-deco21.mb-0 &amp;amp;lt;!DOCTYPE beans PUBLIC “-//PRING//DTD// BEAN 2.0//ES”
                    p.text-deco21.mb-0 “#[span.text-deco18 http://www.springframework.org/dtd/spring-beans-2.0.dtd]”&amp;amp;gt;
                    p.text-deco21.mb-0 amp;amp;lt;beans&amp;amp;gt;
                    p.text-deco21.mb-0 &amp;amp;lt;bean id=“aprendiz” class=“com.sena.AprendizBean”&amp;amp;gt;
                    p.text-deco21.mb-0 &amp;amp;lt;property name=“primernombre” value=“Zulema”&amp;amp;gt;
                    p.text-deco21.mb-0 &amp;amp;lt;property name=“apellidos” value=“Leon”&amp;amp;gt;
                    p.text-deco21.mb-0 &amp;amp;lt;property name=“cedula” value=“25.311.165”&amp;amp;gt;
                    p.text-deco21.mb-0 &amp;amp;lt;/bean&amp;amp;gt;
                    p.text-deco21 &amp;amp;lt;/beans&amp;amp;gt;
          .row.align-items-center.mb-4
            .col-lg-6
              img(src="@/assets/curso/tema2/img21.svg" style="width: 570px").m-auto
            .col-lg-6
              .row
                .col-12.bg-color12
                  .p-4
                    p.mb-0 En la configuración del archivo se ve que la etiqueta #[i “bean”] referencia la clase AprendizBean.java, además el atributo #[i “class”] dirige a la dirección del proyecto y cuenta con un atributo id que permite agregar un nombre para poder identificarlo. Las demás etiquetas como #[i “property”] indican los atributos de la clase AprendizBean y con la etiqueta #[i “value”] se pueden agregar valores directos. Por medio de los métodos #[i get] y #[i set] el #[i Spring Container] (Contenedor de #[i Spring]) obtiene acceso y puede modificar los objetos de la clase AprendizBean. Con los archivos de configuración XML #[i Spring] facilita una clase de listas por cada uno de los #[i beans] existentes para poder hacer llamado de ellos y así poder manipularlos desde otras clases sin tener que realizar varias instancias.
          p.mb-5 En el siguiente código se muestra la implementación de Spring del control de los objetos del proyecto Sena.
          .row.justify-content-center
            .col-lg-8.mb-5
              .row
                .col-12.bg-color11
                  img(src="@/assets/curso/tema1/img8.svg")
                .col-12.bg-color10
                  .p-4
                    p package com.sena 

                    p.mb-0.text-deco21 import org. springframework.beans.factory.BeanFactory;
                    p.mb-0.text-deco21 import org.springframework.beans.factory.xml.XmlBeanFactory;
                    p.mb-0.text-deco21 import org.springframework.core.io.ClassPathResource;
                    p.text-deco21 import org.springframework.core.io.Resource;
                    p.text-deco21 public class SenaLogic{ 
                    p.mb-0(style="margin-left:20px").text-deco21 public static void main(String[] args){
                    p.mb-0(style="margin-left:40px").text-deco22 Resource recurso = new ClassPathResource(“springconfig.xml”);
                    p.mb-0(style="margin-left:40px").text-deco21 BeanFactory factory = new XmlBeanFactory(recurso); 
                    p.mb-0(style="margin-left:40px").text-deco21 AprendizBean aprendizBean = AprendizBean)factory.getBean(“aprendiz”);
                    p(style="margin-left:40px").text-deco22 aprendizBean.verAprendiz();
                    p(style="margin-left:20px").text-deco21 }
                    p.text-deco21 }
          p.mb-5 Lo que mostraría el código anterior sería:
          .row.justify-content-center.mb-5
            .col-lg-6.bg-color18
              .p-5
                p.mb-0.text-center.text-white Zulema León, es la actual estudiante
          .cajon.color-primario.p-4
            p.mb-0 La salida que muestra se logró realizando las configuraciones en el archivo XML, La utilidad del uso de #[i Spring] se evidencia en proyectos grandes con varias clases y varios objetos ya que facilita un manejo mucho más eficiente.
    separador.mb-5
    #t_2_2
    .titulo-segundo.color-secundario
      h2 2.2 Spring Data
    .row.bg-color3.mb-5
      .col-12.px-5
        .row.mb-4
          .col-lg-4
            img(src="@/assets/curso/tema2/img22.svg").m-auto
          .col-lg-8
            .row
              .col-12.my-5.bg-color12
                .p-4
                  p.mb-0 #[i Spring] ofrece una variedad de proyectos independientes que se pueden articular en un proyecto principal, cada proyecto permite resolver una necesidad en especial del negocio, algunos de ellos se muestran en la siguiente imagen.
              .col-12
                img(src="@/assets/curso/tema2/img9.png" style="width: 600px").m-auto
                img(src="@/assets/curso/tema2/img10.png" style="width: 600px").m-auto
        p Uno de los proyectos más utilizados es el #[i SpringData] ya que es uno de los módulos más grandes de #[i Spring] debido a que cuenta con muchos submódulos cuyo objetivo principal es proporcionar una serie de herramientas que permiten realizar integraciones muy sencillas con los diferentes entornos de almacenes de datos disponibles. Los datos que se utilizan pueden proceder de orígenes tanto de bases de datos relacionales como no relacionales.
        p Las funcionalidades de #[i Spring Data] son:
        .row.justify-content-center
          .col-6.col-lg-3
            .p-2
              img(src="@/assets/curso/tema2/img23.svg").m-auto
          .col-6.col-lg-3
            .p-2
              img(src="@/assets/curso/tema2/img24.svg").m-auto
          .col-6.col-lg-3
            .p-2
              img(src="@/assets/curso/tema2/img25.svg").m-auto
          .col-6.col-lg-3
            .p-2
              img(src="@/assets/curso/tema2/img26.svg").m-auto
          .col-6.col-lg-3
            .p-2
              img(src="@/assets/curso/tema2/img27.svg").m-auto
    p.mb-5 Módulos de #[i Spring Data]: los módulos oficiales de #[i Spring Data] son:
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Módulos principales
    .row.bg-color19.mb-5
      .col-12.px-5
        .row.mb-5
          .col-lg-6
            LineaTiempoD.color-primario
              .row(numero="1" titulo="<i>Spring Data Commons</i>")
                .col-12
                  p Brinda infraestructura compartida para módulos de #[i spring].
              .row(numero="2" titulo="<i>Spring Data</i> JDBC")
                .col-12
                  p Implementa repositorios fundamentados en JDBC.
              .row(numero="3" titulo="<i>Spring Data</i> JPA")
                .col-12
                  p Implementa repositorios fundamentados en JPA.
              .row(numero="4" titulo="<i>Spring Data Gemfire</i>")
                .col-12
                  p Implementa GemFire para aplicaciones baja latencia.
              .row(numero="5" titulo="<i>Spring Data KeyValue</i>")
                .col-12
                  p Implementa repositorios para datos de clave-valor.
              .row(numero="6" titulo="<i>Spring Data</i> LDAP")
                .col-12
                  p Implementa repositorios para soporte de LDAP.
              .row(numero="7" titulo="<i>Spring Data MongoDB</i>")
                .col-12
                  p Soporte para documentos y repositorios de #[i MongoDB].
              .row(numero="8" titulo="<i>Spring Data Rest</i>")
                .col-12
                  p Implementa repositorios Restful.
              .row(numero="9" titulo="<i>Spring Data Redis</i>")
                .col-12
                  p Fácil acceso a Redis desde Spring.
              .row(numero="10" titulo="<i>Spring Data</i> para <i>Apache Cassandra</i>")
                .col-12
                  p Implementación para aplicaciones orientadas a datos.
              .row(numero="11" titulo="<i>Spring Data</i> para <i>Apache Geode</i>")
                .col-12
                  p Implementación para aplicaciones orientadas a datos.
          .col-lg-6
            img(src="@/assets/curso/tema2/img28.svg" style="width: 450px").m-auto(data-aos="slide-left")
        .row.justify-content-center
          .col-10.mb-4
            .cajon.color-primario.p-4
              p.mb-0 Invitación a conocer todos los módulos de #[i SpringData] en el siguiente enlace: #[a(href="https://spring.io/projects/spring-data" target="blank") https://spring.io/projects/spring-data].
    .row.mb-5
      .col-lg-6
        img(src="@/assets/curso/tema2/img11.png" style="width: 550px").m-auto
      .col-lg-6
        .row.mb-5
          .col-12.mt-4.bg-color13.tarjeta--azul
            .p-4
              p.mb-0 A continuación, se presenta un ejemplo de un mapeo para JPA que es uno de los submódulos de #[i SpringData]:
        p Para el ejemplo se realiza la clase Persona que representa una tabla en la base de datos llamada Persona.
    .row
      .col-12.mb-5
        .row
          .col-lg-6.mb-4.mb-lg-0
            ImagenInfografica.color-secundario
              template(v-slot:imagen)
                figure
                  img(src='@/assets/curso/tema2/img30.svg')
              .tarjeta.color-acento-botones.p-3(x="7%" y="10%" numero="1")
                p.mb-0 La creación de la tabla se especifica por medio de la anotación @entity y en el atributo #[i “name”] se coloca el nombre de la tabla.
              .tarjeta.color-acento-botones.p-3(x="7%" y="28%" numero="2")
                p.mb-0 Por medio de la anotación @Column se asigna cada uno de los campos de la tabla de la base de datos a los atributos de la clase Persona con la etiqueta #[i “name”] se hace referencia al nombre de la columna de la tabla.
          .col-lg-6
            img(src="@/assets/curso/tema2/img31.svg" style="width: 550px").m-auto.mb-5
            img(src="@/assets/curso/tema2/img32.svg" style="width: 550px").m-auto
      .col-12
        .cajon.color-primario.p-4.mb-4
            p.mb-0 Como se puede ver en el anterior código al extender de la clase #[i CrudRepository] nos facilita métodos como #[i findByNombre] que genera una consulta de todas las personas con el parámetro nombre que en base de datos relacionales sería SELECT * FROM persona WHERE nombre=? como se ve reduce considerablemente las sentencias permitiendo obtener consultas dinámicas.
        p.mb-0 Otro de los grandes proyectos de #[i Spring] es #[i Spring Boot] que se describe a continuación.
    separador.mb-5
    #t_2_3
    .titulo-segundo.color-secundario
      h2 2.3 #[i Spring Boot] y MySQL
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-1
        .row.mb-4
          .col-lg-4
            img(src="@/assets/curso/tema2/img33.svg").m-auto
          .col-lg-8
            .row
              .col-12.mt-5.mb-4.bg-color12
                .p-4
                  p.mb-0 #[i Spring boot] es una infraestructura liviana que suprime en gran parte la tarea de configurar las aplicaciones fundamentadas en #[i Spring], #[i Spring Boot] a diferencia de #[i Spring Framework] realiza una simplificación en cuanto a configuración y el despliegue de las aplicaciones.
            p Las características de #[i Spring Boot]
            ul.lista-ul.ms-3
              li 
                i.fas.fa-layer-group(style="color: #039BE5")
                | 
                p.mb-0 Es intuitivo: permite crear aplicaciones rápidamente gracias a sus valores predeterminados.
              li 
                i.fas.fa-layer-group(style="color: #039BE5")
                |
                p.mb-0 Permite crear aplicaciones que son independientes de #[i Spring]
              li 
                i.fas.fa-layer-group(style="color: #039BE5")
                |
                p.mb-0 Incluye los servidores de #[i Undertow], #[i Tomcat] o #[i jetty].
              li 
                i.fas.fa-layer-group(style="color: #039BE5")
                |
                p.mb-0 Usualmente realiza la configuración automática de librerías de #[i Spring] o de otros.
              li 
                i.fas.fa-layer-group(style="color: #039BE5")
                |
                p.mb-0 No hay que realizar configuraciones de archivos XML.
              li 
                i.fas.fa-layer-group(style="color: #039BE5")
                |
                p.mb-0 Agiliza el desarrollo.
    p.mb-5 #[i Spring Boot] cuenta con dos mecanismos que son los que permiten la simplificación de los procesos y son: Contenedor de aplicaciones integrado y #[i Starters].
    .tarjeta--container.row.mb-5
      .col-md.tarjeta.color-primario.p-5
        .row.justify-content-center.mb-4
          .col-4
            figure
              img(src='@/assets/curso/tema2/img34.svg')
        h2.text-center Contenedor de aplicaciones integrado
        p La compilación de las aplicaciones #[i web] las compila como archivo .jar desplegado en un servidor #[i tomcat] facilitando la distribución de las aplicaciones, anteriormente se trabajaba con .war que si se requiere se puede seguir utilizando.
      .col-md.tarjeta.color-acento-botones1.p-5
        .row.justify-content-center.mb-4
          .col-4
            figure
              img(src='@/assets/curso/tema2/img35.svg')
        h2.text-center #[i Starters]
        p Son los encargados de brindar una variedad de dependencias las cuales se agregan al proyecto, estas pueden ser de terceros o de #[i Spring]. Los #[i starters] por defecto traen una configuración de valores por defecto.
    .cajon.color-primario.p-4.mb-5
      p.mb-0 Otra de las ventajas de #[i Spring boot] es que ofrece un mecanismo que genera la estructura del proyecto de #[i Spring Boot] automáticamente, este inicializador crea el archivo pom.xml, el main de la aplicación y un archivo de #[i test] para verificar que la aplicación corre de forma correcta.
    .row.mb-5.justify-content-center
      .col-lg-8
        .titulo-sexto.color-acento-contenido
          p.mb-0 #[b Figura 5]. Inicializador de #[i Spring]
        figure
          img(src='@/assets/curso/tema2/img12.png')
          figcaption.mt-3 Nota. https://start.spring.io/
    img(src="@/assets/curso/tema2/img13.png" style="width: 1300px").m-auto
    .row.justify-content-center
      .col-10.bg-color8
        .p-4
          p.mb-0 A continuación, se realizan los pasos para la creación de un proyecto en #[i Spring Boot]. Recordar que se deben tener instaladas cualquiera de las herramientas de Entorno de desarrollo y JDK descritas anteriormente en la tabla 1 y tabla 2.
    LineaTiempoD.color-primario.mb-5
      .row(numero="1" titulo="Comienza un nuevo proyecto")
        .col-12
          p.mb-4 Ingresar a #[a(href="https://start.spring.io/" target="blank") start.spring.io] y crea un proyecto #[i web].
          img(src="@/assets/curso/tema2/img14.png" style="width: 1000px").m-auto
      .row(numero="2" titulo="Ingresa el código")
        .col-12
          p.mb-4 Después de descargar el archivo que genera el inicializador ejecute su IDE y abra el archivo, una vez ubicado en la clase principal copiar el siguiente código para ejecutar un Hola mundo.
          img(src="@/assets/curso/tema2/img15.png" style="width: 1000px").m-auto.mb-4
          .cajon.color-primario.p-4
            p.mb-0 Lo que hace el método #[i hello()] es recibir un parámetro de tipo #[i String] con el nombre de #[i name] y después concatenar este parámetro con la palabra #[i Hello] esto quiere decir que si se ingresa un nombre Zulema la salida seria “Hello Zulema”.
      .row(numero="3" titulo="Prueba del proyecto")
        .col-12
          p.mb-4 Ahora solo es probar el proyecto para esto se debe abrir una consola Windows + r, se debe ubicar en la carpeta del proyecto y ejecutar el siguiente comando:
          img(src="@/assets/curso/tema2/img36.svg" style="width: 1000px").m-auto.mb-4
          p.mb-4 y se mostrará la siguiente imagen:
          img(src="@/assets/curso/tema2/img16.png" style="width: 1000px").m-auto.mb-4
          p.mb-4 Lo que hace es ejecutar el servidor #[i Tomcat] que ya viene por defecto dentro del #[i Spring Boot], ahora se debe ingresar al navegador y escribir el #[i localhost] con el puerto 8080 y se mostrará la ejecución de la aplicación.  En la siguiente video clase se explica de forma más detallada cómo utilizar #[i Spring Boot]:
          figure
            .video
              iframe(width="560" height="315" src="https://www.youtube.com/embed/eqy6qS7wtf8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen)
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-1
        .row.mb-4
          .col-lg-4
            img(src="@/assets/curso/tema2/img17.png").m-auto
          .col-lg-8
            .row
              .col-12.mt-5.mb-4.bg-color12
                .p-4
                  p #[b #[i Spring boot] y MySQL]: para tener una aplicación web completa es necesario almacenar información por esta razón es importante realizar conexiones con bases de datos.
                  p Para  este ejemplo se mostrará cómo se realiza la conexión con la base de datos MYSQL.
                  p Los requerimientos fundamentales son tener instalado MYSQL, el entorno de desarrollo y seguir estos pasos:
    .tarjeta.tarjeta--azul1
      .pt-4.px-4
        SlyderA
          .row.justify-content-center
            .col-10
              .row.justify-content-center.align-items-center.d-flex.flex-row
                .col-auto
                  p.mb-4.text-deeco23 01
                .col-8
                  .titulo-sexto.color-acento-contenido
                    p.mb-0 #[b Declarar dependencias]: JPA, MySQL JDBC #[i Driver], #[i Web] como se mostró en el ejemplo anterior por medio del inicializador se pueden seleccionar las dependencias requeridas como se muestra en la siguiente imagen.
            .col-10
              .row
                .col-lg-8.mb-4.mb-lg-0
                  img(src="@/assets/curso/tema2/img20.png" style="width: 900px").m-auto
                .col-lg-4.align-bottom
                  img(src="@/assets/curso/tema2/img18.png" style="width: 400px").m-auto
          .row.justify-content-center
            .col-10
              .row.justify-content-center.align-items-center.d-flex.flex-row
                .col-auto
                  p.mb-4.text-deeco23 02
                .col-8
                  .titulo-sexto.color-acento-contenido
                    p.mb-0 Después de agregar las dependencias clic en #[i GENERATE] y descargará un archivo zip el cual se debe descomprimir y después importar el proyecto en el IDE para este caso #[i Spring Tool Suite]. Una vez importado el proyecto se puede ver cómo queda la estructura.
            .col-10
              .row
                .col-lg-4.align-bottom
                  img(src="@/assets/curso/tema2/img19.png" style="width: 300px").m-auto
                .col-lg-8.mb-4.mb-lg-0
                  img(src="@/assets/curso/tema2/img21.png" style="width: 400px").m-auto
          .row.justify-content-center
            .col-10
              .row.justify-content-center.align-items-center.d-flex.flex-row
                .col-auto
                  p.mb-4.text-deeco23 03
                .col-8
                  .titulo-sexto.color-acento-contenido
                    p.mb-0 El paso siguiente es abrir el archivo #[b “aplication.properties”] y configurar todas las propiedades de la conexión así:
            .col-10
              .row
                .col-lg-8.mb-4.mb-lg-0
                  ImagenInfografica.color-secundario
                    template(v-slot:imagen)
                      figure
                        img(src='@/assets/curso/tema2/img38.svg')
                    .tarjeta.color-acento-botones.p-3(x="2%" y="27%" numero="1")
                      p.mb-0 #[b Línea 1]: permite obtener los metadatos de la base de datos.
                    .tarjeta.color-acento-botones.p-3(x="2%" y="37%" numero="2")
                      p.mb-0 #[b Línea 2]: se muestra la url de la conexión con el motor de base de datos.
                    .tarjeta.color-acento-botones.p-3(x="2%" y="54%" numero="3")
                      p.mb-0 #[b Línea 3]: se especifica el nombre del usuario de la base de datos para la conexión.
                    .tarjeta.color-acento-botones.p-3(x="2%" y="64%" numero="4")
                      p.mb-0 #[b Línea 4]: se especifica clave de la base de datos para la conexión.
                    .tarjeta.color-acento-botones.p-3(x="2%" y="74.5%" numero="5")
                      p.mb-0 #[b Línea 5]: la propiedad true permite utilizar las consultas JPA a realizar en la base de datos.
                .col-lg-4.align-bottom
                  img(src="@/assets/curso/tema2/img18.png" style="width: 400px").m-auto
          .row.justify-content-center
            .col-10
              .row.justify-content-center.align-items-center.d-flex.flex-row
                .col-auto
                  p.mb-4.text-deeco23 04
                .col-8
                  .titulo-sexto.color-acento-contenido
                    p.mb-0 Lo que queda es ejecutar la aplicación y comprobar que no existan problemas con la conexión a la base de datos. Para ejecutar dar clic derecho en el archivo JAVA seleccionar la opción &gt;#[i Run As] y &gt;#[i Spring Boot App]. Si todo está bien ahora solo queda ir al motor de bases de datos y verificar si creó el esquema.
            .col-10
              .row
                .col-lg-8.mb-4.mb-lg-0
                  img(src="@/assets/curso/tema2/img22.png" style="width: 300px").m-auto
                .col-lg-4.align-bottom
                  img(src="@/assets/curso/tema2/img18.png" style="width: 400px").m-auto
    separador.mb-5
    #t_2_4
    .titulo-segundo.color-secundario
      h2 2.4 Validaciones
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-1
        .row.mb-4
          .col-lg-4
            img(src="@/assets/curso/tema2/img23.png").m-auto
          .col-lg-8
            .row
              .col-12.mt-5.mb-4.bg-color12
                .p-4
                  p.mb-0 Es muy importante realizar validaciones cuando se están desarrollando aplicaciones #[i web] en JAVA para impedir que se ingresen datos que afecten al programa, en #[i Spring] viene incluido el #[i hibernate-validator] en el paquete #[i spring-boot-starter-web] que permite validar valores de los campos #[i Beans].
            .row.justify-content-center
              .col-lg-8
                .row
                  .col-12.bg-color11
                    img(src="@/assets/curso/tema1/img8.svg")
                  .col-12.bg-color10
                    .p-4
                      p.mb-0.text-deco21 &lt;dependency&gt;
                      p.mb-0(style="margin-left:20px").text-deco21 &lt;groupId&gt;org.springframework.boot&lt;/groupId&gt;
                      p.mb-0(style="margin-left:20px").text-deco21 &lt;artifactId&gt;spring-boot-starter-web&lt;/artifactId&gt;
                      p.mb-0(style="margin-left:20px").text-deco21 &lt;version&gt;2.0.0.RELEASE&lt;/version&gt;
                      p.mb-0.text-deco21 &lt;/dependency&gt;
    .row.justify-content-center.mb-5
      .col-lg-8.bg-color20
        .p-4
          p.mb-0 #[b Para el ejemplo se realiza la creación de un bean con unas anotaciones que permiten la validación de ingreso de un usuario.]
    .row.justify-content-center.mb-5
      .col-lg-8
        .row
          .col-12.bg-color11
            img(src="@/assets/curso/tema1/img8.svg")
          .col-12.bg-color10
            .p-4
              p.mb-0.text-deco21 @Data
              p.mb-0.text-deco21 @NoArgsConstructor
              p.mb-0.text-deco21 public class Usuario{
              p.mb-0(style="margin-left:20px").text-deco21 @NotBlank(message=“Debe ingresar un nombre de usuario”)
              p(style="margin-left:20px").text-deco21 private String nombreUsuario;
              p.mb-0(style="margin-left:20px").text-deco21 @NotBlank(message=“debe ingresar un valor correcto para la edad”)
              p.mb-0(style="margin-left:20px").text-deco21 @Pattern(regexp=“^[0-9]{1,2}$”,message=“Edad incorrecta”)
              p(style="margin-left:20px").text-deco21 private String edad;
              p.mb-0(style="margin-left:20px").text-deco21 @AssertFalse(message = “Debe ser falso”)
              p.mb-0(style="margin-left:20px").text-deco21 private Boolean esfalso;
              p(style="margin-left:20px").text-deco21 /**           
              p.mb-0(style="margin-left:20px").text-deco21 */
              p.mb-0(style="margin-left:20px").text-deco21 @Pattern(regexp=“^[0-9]{4}-[0-9]{2}-[0-9]{2}$”,message=“No es correcto el formato de la fecha “)
              p.mb-0(style="margin-left:20px").text-deco21 private String fechanaciemiento;
              p.text-deco21 } 
    .row.justify-content-center.mb-5
      .col-lg-8.bg-color20
        .p-4
          p.mb-0 #[b Una vez se crean las anotaciones se debe crear el controlador.]
    .row.justify-content-center.mb-5
      .col-lg-8
        .row
          .col-12.bg-color11
            img(src="@/assets/curso/tema1/img8.svg")
          .col-12.bg-color10
            .p-4
              p.mb-0.text-deco21 @Controller
              p.mb-0.text-deco21 public class userController{
              p.mb-0(style="margin-left:20px").text-deco21 @RequestMapping(“/usuario”)
              p.mb-0(style="margin-left:20px").text-deco21 public void create (@RequestBody @Validated Usuario usuario) {
              p.mb-0(style="margin-left:20px").text-deco21 System.out.println(“hola:” + usuario.getNombreUsuario());
              p.mb-0(style="margin-left:20px").text-deco21 }
              p.text-deco21 }
    p.mb-5 Una vez se realice el controlador se puede realizar la prueba enviando una solicitud #[i Post].
    .row.justify-content-center.mb-5
      .col-lg-8.bg-color20
        .p-4
          p.mb-0 #[b {"nombreUsuario":"Ana","edad":120,"esFalso”: true,"nacimiento":"21010-21-12"}]
    p La verificación que mostraría el resultado es:
    .row.justify-content-center
      .col-lg-8
        img(src="@/assets/curso/tema2/img39.svg" style="width: 500px").m-auto

</template>

<script>
export default {
  name: 'Tema2',
  data: () => ({
    indicadorTarjetaFlip: true,
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
