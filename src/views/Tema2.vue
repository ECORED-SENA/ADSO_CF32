<template lang="pug">
.curso-main-container.pb-3
  BannerInterno
  .container.tarjeta.tarjeta--blanca.p-4.p-md-5
    
    .titulo-principal.color-acento-contenido
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
                  p.mb-4 Es un Framework de código abierto que facilita crear aplicaciones empresariales de alto rendimiento en Java, además de Java tiene soporte para los lenguajes Groovy y Kotlin. La estructura que lo compone es modular esta estructura cuenta con una flexibilidad para implementar una variedad de arquitecturas dependiendo de los requerimientos de las aplicaciones haciendo que la programación sea lo más hacedera posible, rápida y muy segura.
                  .row.mb-4.bg-color4.justify-content-end
                    .col-12
                      img(src="@/assets/curso/tema1/img2.svg" style="width: 50px; margin-left:40px")
                    .col-10
                      .p-2
                        p.text-white Historia: Rod Johnson creador de Spring se da cuenta que necesitan una herramienta para simplificar y facilitar la construcción de aplicaciones JEE utilizando EJB y escribe el libro expert one-on-one J2EE Development que es un conjunto de buenas prácticas para la creación de aplicaciones empresariales y en el año 2004 lanza primera versión 1.2.6 de Spring, según el autor era el inicio de J2EE tradicional.
                        .row.align-items-center
                          .col-10.d-inline
                            p.text-white.text-end.mb-0 #[b Johnson,( 2004)]
                          img(src="@/assets/curso/tema1/img3.svg" style="width: 40px")
                  p La siguiente figura muestra las Versiones de Spring Framework:
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Versiones de Spring Framework
    img(src="@/assets/curso/tema2/img2.png" style="width: 1000px").m-auto.mb-5
    p.mb-5 Unas de las características principales de Spring son:
    .row
      .col-lg-6.mb-4.mb-lg-0
        LineaTiempoD.color-primario
          .row(numero="1" titulo="Flexibilidad")
            .col-12
              p Contiene un grupo flexible de librerías y extensiones de terceros de Spring facilitando a los desarrolladores construir aplicaciones fácilmente.
          .row(numero="2" titulo="Inyección de dependencia (DI)")
            .col-12
              p Ofrece un patrón que permite ayudar en el acoplamiento bajo, esto quiere decir que cuando existe dependencias entre las clases y se necesita crear un objeto de esta clase lo que hace spring es suministrar este objeto obteniendo beneficios en la modularidad, escalabilidad y dependencia de clases.
          .row(numero="3" titulo="ORM (Object Relational Mapping)")
            .col-12
              p Suministra un fácil acceso a datos por medio del ORM.
          .row(numero="4" titulo="Estructura y módulos")
            .col-12
              p Spring integra una variedad de módulos que se pueden integrar para el desarrollo de las aplicaciones.
      .col-lg-6
        img(src="@/assets/curso/tema2/img1.svg" style="width: 470px").m-auto
    .row.bg-color16.mb-5
      .col-12.px-5
        .row.justify-content-center
          .col-12.mb-4.mt-3
            .p-4
              p.mb-0 La siguiente figura nos muestra lo que se puede crear con Spring Framework: Aplicaciones de consola, Aplicaciones de escritorio, Aplicaciones Web, Aplicaciones Móviles, Servicios SOAP, REST. Spring está orientado esencialmente al backend.
          .col-10
            .row.justify-content-evenly.mb-0.mb-lg-4
              .col-8.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img2.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img3.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Microservicios
                      p.text-center Permite crear y ejecutar microservicios en producción a escala
              .col-8.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img4.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img5.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Nube
                      p.text-center Ejecución de servicios en la nube
              .col-8.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img6.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img7.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Aplicaciones web
                      p.text-center Creación rápida de aplicaciones web
            .row.justify-content-evenly
              .col-8.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img8.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img9.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Reactive
                      p.text-center Permite la creación de proyectos reactivos basados en mensajes
              .col-8.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img10.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img11.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Servlets
                      p.text-center Permite la ejecución de código impulsado por eventos se encarga del escalado y la seguridad del lado del servidor
              .col-8.col-lg-4.mb-4.mb-lg-0
                .tarjeta.tarjeta-flip.color-secundario(@mouseover="indicadorTarjetaFlip = false")
                  .indicador--hover(v-if="indicadorTarjetaFlip")
                  .tarjeta-flip__contenedor
                    .tarjeta-flip__img(:style="{'background-image': `url(${require('@/assets/curso/tema2/img12.svg')})`}")
                    .tarjeta-flip__contenido.p-4.p-xl-5
                      img(src="@/assets/curso/tema2/img13.svg" style="width: 100px").m-auto.mb-3
                      h1.text-center Batch
                      p.text-center Aplicaciones de procesamiento de datos en lote
    #t_2_1
    .titulo-segundo.color-secundario
      h2 2.1 Introducción
    .row.bg-color3.mb-5
      .col-12.px-5.px-lg-0
        .row
          .col-lg-6
            img(src="@/assets/curso/tema2/img3.png").m-auto
          .col-lg-6
            .row
              .col-12.mt-5.bg-color12
                .p-4
                  p.mb-0 El Framework Spring básicamente con su inyección de dependencias se encarga de construir objetos y configurar todas las dependencias que estos necesiten. En Spring estos objetos que son creados son llamados beans que son anotaciones que son agregadas a las clases así: @component, @Service, @Repository etc. Uno de los principios principales de Spring es el de Inversión de Dependencia (DIP) el cual habla de que los módulos de alto nivel no deben depender de los de bajo nivel, lo que quiere decir es que hay que hacer más referencia a las abstracciones que a las implementaciones por lo que no se debe depender de una clase ni de una implementación en particular. La implementación de este principio es llamado Inversión de Control (IOc) que se encarga de desacoplar el código utilizando eventos, también es llamado como el principio de Hollywood “no nos llames; nosotros te llamaremos”, que consisten en una manera de programar donde la aplicación es quien interviene en cambio del código, para realizar la implementación del IOc se necesita un agente externo que recibe el nombre de contenedor quién es el encargado de verificar el flujo de la aplicación. Los IOc utilizan Service locator, Eventos y los DI (Inyecciones de dependencias) enfocando el Spring Framework en la DI.
              .col-12
                .p-4
                  p #[b Inyección de Dependencias]: es un patrón de diseño de software, subtipo de inversión de control cuyo objetivo es tener un código fácil de mantener o desacoplado. Su función es determinar lo que los objetos necesitan.
                  p.mb-4 Existen 3 formas de realizar inyección de dependencias:
                  img(src="@/assets/curso/tema2/img14.svg" style="width: 470px").m-auto
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Principio inversión de control
    .row.bg-color15
      .col-12
        .p-4
          img(src="@/assets/curso/tema2/img15.svg" style="width: 800px").m-auto.mt-5
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
              p.mb-0 Resumiendo, la inversión de control es un patrón de programación para obtener un acoplamiento flexible logrando que los objetos independientes no sean responsables de sus dependencias si no que sean recibidas desde afuera; el contenedor de IOc recoge los metadatos que vienen de un archivo XML, o código Java, y recibe las indicaciones de los objetos que debe crearlos, enlazarlos, configurarlos y destruirlos por medio de POJOs (Objetos simples de Java) creando objetos por medio del proceso que recibe el nombre de Spring Beans y resultando objetos preparados para la inyección de dependencia.
        p La siguiente figura evidencia el funcionamiento de una vista abstracta de Spring.
      .col-lg-6
        img(src="@/assets/curso/tema2/img5.png" style="width: 570px").m-auto
    .row.align-items-center.mb-5
      .col-lg-6.tarjeta--azul
        .p-4
          img(src="@/assets/curso/tema2/img20.svg" style="width: 570px").m-auto
      .col-lg-6
        p.mb-4 En el video se explican aspectos generales de la inyección de dependencias:
        .tarjeta.color-primario.p-3.mb-4
          .row.justify-content-around.align-items-center
            .col-3.col-sm-2.col-lg-2
              img(src="@/assets/curso/tema1/img21.svg")
            .col
              .row.justify-content-between.align-items-center
                .col.mb-3.mb-sm-0
                  h3.mb-1.text-white Método save
                  p.text-small.text-white Estimado aprendiz, para profundizar sobre el tema puede consultar el siguiente video.
                .col-sm-auto
                  a.boton.color-acento-contenido.texto-blanco(:href="obtenerLink('/downloads/prueba.pdf')" target="_blank")
                    span(style="color:#000000 !important") Ver video
        p #[b Módulos del Framework]: Spring Framework es un marco de trabajo muy amplio y brinda cerca de 20 módulo los cuales se asocian en el contenedor principal, “Accesos e integración de datos, Web, AOP (Programación orientada a aspectos, Instrumentación, Mensajes y Pruebas)” (Spring ,2021).
        p Para trabajar con Spring se necesita tener instalado los siguientes requerimientos:
        ul.lista-ul.ms-3
          li 
            i.fas.fa-layer-group(style="color: #039BE5")
            | 
            p.mb-0 #[b Un entorno de desarrollo (IDE)] se puede seleccionar cualquiera de los relacionados en la tabla No 1.
          li 
            i.fas.fa-layer-group(style="color: #039BE5")
            |
            p.mb-0 #[b Un JDK (Kit de desarrollo de java)] se puede descargar cualquiera de los relacionados en la tabla No 2.
    .row.justify-content-center.mb-5
      .col-lg-8.mb-5
        .titulo-sexto.color-acento-contenido
          p.mb-0 #[b Tabla 1.] Entornos para desarrollo en Spring
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
          p.mb-0 #[b Tabla 2.] JDK para desarrollo en Spring
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
    p.mb-5 Para construir aplicaciones en Spring Framework necesitamos:
    AcordionA(tipo="a" clase-tarjeta="tarjeta tarjeta--azul")
      .row(titulo="Elegir jars con Maven")
        .col-12
          p.mb-5 Lo primero que se debe hacer es la creación de un proyecto Maven o Gradle y realizar la descarga de las dependencias necesarias.
          .titulo-sexto.color-acento-contenido
            p.mb-0 #[b Figura 1.] Creación proyecto Maven
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
            p.mb-5 A continuación, se muestra un nuevo ejemplo de código explicando más a detalle el uso del Contenedor en Spring.Para el siguiente ejemplo se tiene un proyecto llamado “Sena” el cual tiene una clase aprendiz con los siguientes atributos:
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
            p.mb-5 Al utilizar este proyecto Sena Spring framework cuenta con un archivo XML que gestiona objetos (Spring IOC Container) para este proyecto recibe el nombre de springconfig.xml y se ve de la siguiente manera.
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
                    p.mb-0 En la configuración del archivo se ve que la etiqueta “bean” referencia la clase AprendizBean.java, además el atributo “class” dirige a la dirección del proyecto y cuenta con un atributo id que permite agregar un nombre para poder identificarlo. Las demás etiquetas como “property” indican los atributos de la clase AprendizBean y con la etiqueta “value” se pueden agregar valores directos. Por medio de los métodos get y set el Spring Container (Contenedor de Spring) obtiene acceso y puede modificar los objetos de la clase AprendizBean. Con los archivos de configuración XML Spring facilita una clase de listas por cada uno de los beans existentes para poder hacer llamado de ellos y asi poder manipularlos desde otras clases sin tener que realizar varias instancias.
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
            p.mb-0 La salida que muestra se logró realizando las configuraciones en el archivo XML, La utilidad del uso de Spring se evidencia en proyectos grandes con varias clases y varios objetos ya que facilita un manejo mucho más eficiente.
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
                  p.mb-0 Spring ofrece una variedad de proyectos independientes que se pueden articular en un proyecto principal, cada proyecto permite resolver una necesidad en especial del negocio, algunos de ellos se muestran en la siguiente imagen.
              .col-12
                img(src="@/assets/curso/tema2/img9.png" style="width: 600px").m-auto
                img(src="@/assets/curso/tema2/img10.png" style="width: 600px").m-auto
        p Uno de los proyectos más utilizados es el SpringData ya que es uno de los módulos más grandes de Spring debido a que cuenta con muchos submódulos cuyo objetivo principal es proporcionar una serie de herramientas que permiten realizar integraciones muy sencillas con los diferentes entornos de almacenes de datos disponibles. Los datos que se utilizan pueden proceder de orígenes tanto de bases de datos relacionales como no relacionales.
        p Las funcionalidades de Spring Data son:
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
    .row.mb-5.ps-4.ps-md-1.bg-color6
      .col-8.col-lg-4.bg-color7
        h3.mb-0.text-white Módulos principales
    .row.bg-color19.mb-5
      .col-12.px-5
        .row.mb-5
          .col-lg-6
            LineaTiempoD.color-primario
              .row(numero="1" titulo="Spring Data Commons")
                .col-12
                  p Brinda infraestructura compartida para módulos de spring.
              .row(numero="2" titulo="Spring Data JDBC")
                .col-12
                  p Implementa repositorios fundamentados en JPA.
              .row(numero="3" titulo="Spring Data JPA")
                .col-12
                  p Implementa repositorios fundamentados en JPA.
              .row(numero="4" titulo="Spring Data Gemfire")
                .col-12
                  p Implementa GemFire para aplicaciones baja latencia.
              .row(numero="5" titulo="Spring Data KeyValue")
                .col-12
                  p Implementa repositorios para datos de clave-valor.
              .row(numero="6" titulo="Spring Data LDAP")
                .col-12
                  p Implementa repositorios para soporte de LDAP.
              .row(numero="7" titulo="Spring Data MongoDB")
                .col-12
                  p Soporte para documentos y repositorios de MongoDB.
              .row(numero="8" titulo="Spring Data Rest")
                .col-12
                  p Implementa repositorios Restful.
              .row(numero="9" titulo="Spring Data Redis")
                .col-12
                  p Fácil acceso a Redis desde Spring.
              .row(numero="10" titulo="Spring Data para Apache Cassandra")
                .col-12
                  p Implementación para aplicaciones orientadas a datos.
              .row(numero="11" titulo="Spring Data para Apache Geode")
                .col-12
                  p Implementación para aplicaciones orientadas a datos.
          .col-lg-6
            img(src="@/assets/curso/tema2/img28.svg" style="width: 450px").m-auto
        .row.justify-content-center
          .col-10.mb-4
            .cajon.color-primario.p-4
              p.mb-0 Invitación a conocer todos los módulos de SpringData en el siguiente enlace: #[a(href="https://spring.io/projects/spring-data" target="blank") https://spring.io/projects/spring-data].
    .row.mb-5
      .col-lg-6
        img(src="@/assets/curso/tema2/img11.png" style="width: 550px").m-auto
      .col-lg-6
        .row.mb-5
          .col-12.mt-4.bg-color13.tarjeta--azul
            .p-4
              p.mb-0 A continuación, se presenta un ejemplo de un mapeo para JPA que es uno de los submódulos de SpringData:
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
                p.mb-0 La creación de la tabla se especifica por medio de la anotación @entity y en el atributo “name” se coloca el nombre de la tabla.
              .tarjeta.color-acento-botones.p-3(x="7%" y="28%" numero="2")
                p.mb-0 Por medio de la anotación @Column se asigna cada uno de los campos de la tabla de la base de datos a los atributos de la clase Persona con la etiqueta “name” se hace referencia al nombre de la columna de la tabla.
          .col-lg-6
            img(src="@/assets/curso/tema2/img31.svg" style="width: 550px").m-auto.mb-5
            img(src="@/assets/curso/tema2/img32.svg" style="width: 550px").m-auto
      .col-12
        .cajon.color-primario.p-4.mb-4
            p.mb-0 Como se puede ver en el anterior código al extender de la clase CrudRepository nos facilita métodos como findByNombre que genera una consulta de todas las personas con el parámetro nombre que en base de datos relacionales seria SELECT * FROM persona WHERE nombre=? como se ve reduce considerablemente las sentencias permitiendo obtener consultas dinámicas.
        p.mb-0 Otro de los grandes proyectos de Spring es Spring Boot que se describe a continuación.
    separador.mb-5
    #t_2_3
    .titulo-segundo.color-secundario
      h2 2.3 Spring Boot y MySQL

</template>

<script>
export default {
  name: 'Tema2',
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
