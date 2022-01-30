<h1 align="center">
<img src="https://s2.glbimg.com/TES0H8Evg6phh91YTFr0rCyCxTk=/90x68/s2.glbimg.com/EVEqLFXR5M5rFugYYWIQtAg05_E=/0x0:100x100/75x75/s.glbimg.com/po/tt2/f/original/2016/03/01/java.png" width="60" height="60"> <br>
  JAVA
</h1>

<p align="justify">
Este projeto é uma coleção de tutoriais pequenos e focados - cada um cobrindo uma área única e bem definida de desenvolvimento no ecossistema Java. Aqui esta todos meus estudos particulares tendo como primazia todos os conceitos da linguagem, levando em consideração o desenvolvimento de API'S nivel backend, toda parte de desenvolvimento e modelagem de dados com integração ao banco de dados, esta em outro repositorio.
<p>

# Executando os testes
O comando mvn clean installde dentro de um módulo executará os testes de unidade nesse módulo. Para módulos Spring, isso também executará oSpringContextTest if present.

>Para executar os testes de integração, use o comando: 

````
mvn clean install -Pintegration-lite-first ou
mvn clean install -Pintegration-lite-second ou
mvn clean install -Pintegration-heavy
````

## Pirâmide testes

<img src="https://devporai.com.br/wp-content/uploads/2020/02/Pir%C3%A2mide-testes.png" width="619" height="341" align="justify">

dependendo da lista onde nosso módulo existe, os comandos serão executados com sucesso.

Dentro desse assunto, gostaria de publicar minha lista de frameworks e componentes Java utilizado nas minhas decisões arquiteturais no momento de arquiteturar uma solução. Qualquer sugestão é bem vinda!

## Arquiquetura para aplicações com microservices

<img src="https://res.infoq.com/articles/twelve-testing-techniques-microservices-intro/en/resources/twelve-testing-techniques-microservices-intro-1-1565852737541.jpg" width="842" height="456">

### Container IoC
- <a>Spring – <a href="http://www.springsource.org/">http://www.springsource.org/</a></a>
- <a>Guice – <a href="http://picocontainer.codehaus.org/">http://picocontainer.codehaus.org/</a></a>
- <a>PicoContainer - <a href="http://code.google.com/p/google-guice/">http://code.google.com/p/google-guice/</a>
- <a>EJB - <a href="http://www.oracle.com/technetwork/java/javaee/ejb/index.html">http://www.oracle.com/technetwork/java/javaee/ejb/index.html</a>
- <a>CDI - <a href="http://www.oracle.com/technetwork/articles/java/cdi-javaee-bien-225152.html">http://www.oracle.com/technetwork/articles/java/cdi-javaee-bien-225152.html</a>

### Persistência
- <a>Hibernate - <a href="http://www.hibernate.org/">http://www.hibernate.org/</a>
- <a>Spring Data - <a href="http://www.springsource.org/">http://www.springsource.org/</a>
- <a>iBatis - <a href="http://www.mybatis.org/">http://www.mybatis.org/</a>
- <a>Torque - <a href="http://db.apache.org/torque/">http://db.apache.org/torque/</a>
- <a>Castor - <a href="http://www.castor.org/">http://www.castor.org/</a>
- <a>Cayenne - <a href="http://cayenne.apache.org/">http://cayenne.apache.org/</a>

### Gerenciador de transação
- <a>Spring AOP transaction - <a href="http://www.springsource.org/">http://www.springsource.org/</a>
- <a>EJB (JTA) - <a href="http://www.oracle.com/technetwork/java/javaee/ejb/index.html">http://www.oracle.com/technetwork/java/javaee/ejb/index.html</a>

### Agendamento de tarefas
- <a>Timer Task JSE - <a href="http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/threads/timer.html">http://www.dsc.ufcg.edu.br/~jacques/cursos/map/html/threads/timer.html</a> 
- <a>Quarts – <a href="http://quartz-scheduler.org/">http://quartz-scheduler.org/</a>
- <a>EJB Timer Service – <a href="http://docs.oracle.com/javaee/6/tutorial/doc/bnboy.html">http://docs.oracle.com/javaee/6/tutorial/doc/bnboy.html</a>

### Validação
- <a>Commons Validator – <a href="http://commons.apache.org/validator/">http://commons.apache.org/validator/</a>
- <a>Java Bean Validator – <a href="http://docs.oracle.com/javaee/6/tutorial/doc/gircz.html">http://docs.oracle.com/javaee/6/tutorial/doc/gircz.html</a>

### Chamadas assíncronas
- <a>JSE Executor Services – <a href="http://docs.oracle.com/javase/tutorial/essential/concurrency/exinter.html">http://docs.oracle.com/javase/tutorial/essential/concurrency/exinter.html</a>
- <a>EJB Asynchronous Method Invocation – <a href="http://docs.oracle.com/javaee/6/tutorial/doc/gkkqg.html">http://docs.oracle.com/javaee/6/tutorial/doc/gkkqg.html</a>
- <a>EJB Message-Driven Bean – <a href="http://docs.oracle.com/javaee/6/tutorial/doc/gipko.html">http://docs.oracle.com/javaee/6/tutorial/doc/gipko.html</a>

### Kit de interface gráficas desktop
- <a>Swing – <a href="http://docs.oracle.com/javase/tutorial/uiswing/">http://docs.oracle.com/javase/tutorial/uiswing/</a>
- <a>SwingX – <a href="http://swingx.java.net/">http://swingx.java.net/</a>
- <a>JGoodies – <a href="http://swingx.java.net/">http://swingx.java.net/</a>
- <a>SWT – <a href="http://www.eclipse.org/swt/">http://www.eclipse.org/swt/</a>
- <a>SWT OPAL – <a href="http://code.google.com/a/eclipselabs.org/p/opal/">http://code.google.com/a/eclipselabs.org/p/opal/</a>

### RAD interface gráficas desktop
- <a>Eclipse Windows Builder – <a href="http://www.eclipse.org/windowbuilder/">http://www.eclipse.org/windowbuilder/</a>
- <a>NetBeans Matisse – <a href="http://netbeans.org/features/java/swing.html">http://netbeans.org/features/java/swing.html</a>

### Framework web
- <a>Click – <a href="http://click.apache.org/">http://click.apache.org/</a>
- <a>Wicket – <a href="http://wicket.apache.org/">http://wicket.apache.org/</a>
- <a>Spring MVC – <a href="http://www.springsource.org/">http://www.springsource.org/</a>
- <a>Struts – <a href="http://struts.apache.org/">http://struts.apache.org/</a>
- <a>Mentawai – <a href="http://www.mentaframework.org/"> http://www.mentaframework.org/</a>
- <a>JSF – <a href="http://www.oracle.com/technetwork/java/javaee/javaserverfaces-139869.html">http://www.oracle.com/technetwork/java/javaee/javaserverfaces-139869.html</a>
- <a>VRaptor – <a href="http://vraptor.caelum.com.br/">http://vraptor.caelum.com.br/</a>

### Framework web RIA
- <a>GWT – <a href="https://developers.google.com/web-toolkit/">https://developers.google.com/web-toolkit/</a>
- <a>Vaadin – <a href="https://vaadin.com/home">https://vaadin.com/home</a>
- <a>ZK Framework – <a href="https://vaadin.com/home">http://www.zkoss.org</a>

### Framework web full stack
- <a>Grails – <a href="http://grails.org/">http://grails.org/</a>
- <a>Ruby On Rails – <a href="http://rubyonrails.org/">http://rubyonrails.org/</a>
- <a>OpenXava – <a href="http://www.openxava.org/">http://www.openxava.org/</a>

### Provedores de JSF
- <a>Mojorra – <a href="http://javaserverfaces.java.net/">http://javaserverfaces.java.net/</a>
- <a>MyFaces – <a href="http://myfaces.apache.org/">http://myfaces.apache.org/</a>
- <a>ADF – <a href="http://www.oracle.com/technetwork/developer-tools/adf/overview/index.html">http://www.oracle.com/technetwork/developer-tools/adf/overview/index.html</a>

### Componentes JSF
- <a>RichFaces – <a href="http://www.jboss.org/richfaces">http://www.jboss.org/richfaces</a>
- <a>PrimeFaces – <a href="http://primefaces.org/">http://primefaces.org/</a>
- <a>OpenFaces – <a href="http://openfaces.org/">http://openfaces.org/</a>
- <a>IceFaces – <a href="http://www.icesoft.org/">http://www.icesoft.org/</a>
- <a>EasyFaces – <a href="http://www.easyfaces.com.br">http://www.easyfaces.com.br</a>
- <a>Gmaps4jsf – <a href="http://code.google.com/p/gmaps4jsf/">http://code.google.com/p/gmaps4jsf/</a>

### Extensões JSF
- <a>PrettyFaces – <a href="http://ocpsoft.org/prettyfaces/">http://ocpsoft.org/prettyfaces/</a>
- <a>Omnifaces – <a href="https://showcase-omnifaces.rhcloud.com/">https://showcase-omnifaces.rhcloud.com/</a>

### Soluções web mobil
- <a>JSF RichFaces Mobile – <a href="http://www.jboss.org/richfaces">http://www.jboss.org/richfaces</a>
- <a>JSF PrimeFaces Mobile – <a href="http://primefaces.org/">http://primefaces.org/</a>
- <a>JSF OpenFaces Mobile – <a href="http://openfaces.org/">http://openfaces.org/</a>
- <a>JSF IceFaces Mobile – <a href="http://www.icesoft.org/">http://www.icesoft.org/</a>
- <a>Spring Mobile – <a href="http://www.springsource.org/">http://www.springsource.org/</a>
- <a>JQuery Mobile – <a href="http://jquery.com/">http://jquery.com/</a>
- <a>DOJO Mobile – <a href="http://dojotoolkit.org/">http://dojotoolkit.org/</a>

### Autenticação e autorização web
- <a>Spring Security – <a href="http://www.springsource.org/">http://www.springsource.org/</a>
- <a>JGuard – <a href="http://jguard.xwiki.com/xwiki/bin/view/Main/WebHome">http://jguard.xwiki.com/xwiki/bin/view/Main/WebHome</a>
- <a>JEE Container Managed Security (Configuração especifica para cada provedor de container JEE). Veja o Tomcat – <a href="http://tomcat.apache.org/tomcat-7.0-doc/realm-howto.html">http://tomcat.apache.org/tomcat-7.0-doc/realm-howto.html</a>

### JEE web container standalone
- <a>Tomcat – <a href="http://tomcat.apache.org/">http://tomcat.apache.org/</a>
- <a>Jetty – <a href="http://jetty.codehaus.org/jetty/">http://jetty.codehaus.org/jetty/</a>
- <a>JBoss – <a href="http://www.jboss.org/">http://www.jboss.org/</a>

### JEE EJB container (web profile e JEE Full)
- <a>Tomee – <a href="http://openejb.apache.org/apache-tomee.html">http://openejb.apache.org/apache-tomee.html</a>
- <a>Simpas – <a href="http://siwpas.mechsoft.com.tr/">http://siwpas.mechsoft.com.tr/</a>
- <a>Resin – <a href="http://www.caucho.com/resin-application-server/">http://www.caucho.com/resin-application-server/</a>
- <a>JBoss – <a href="http://www.jboss.org/">http://www.jboss.org/</a>
- <a>Glassfish – <a href="http://glassfish.java.net/">http://glassfish.java.net/</a>
- <a>Webshere – <a href="http://www-142.ibm.com/software/products/br/pt/appserv-was">http://www-142.ibm.com/software/products/br/pt/appserv-was</a>
- <a>WebLogic – <a href="http://www.oracle.com/us/products/middleware/application-server/weblogic-suite/index.html?ssSourceSiteId=ocombr">http://www.oracle.com/us/products/middleware/application-server/weblogic-suite/index.html?ssSourceSiteId=ocombr</a>
- <a>Geronimo – <a href="http://geronimo.apache.org/">http://geronimo.apache.org/</a>

### Relatórios
- <a>iReport – <a href="http://jasperforge.org/projects/ireport">http://jasperforge.org/projects/ireport</a>
- <a>DynamicReport – <a href="http://dynamicreports.sourceforge.net">http://dynamicreports.sourceforge.net</a>
- <a>Birt – <a href="http://www.eclipse.org/birt/phoenix/">http://www.eclipse.org/birt/phoenix/</a>
- <a>iText – <a href="http://itextpdf.com/">http://itextpdf.com/</a>
- <a>PDFBox – <a href="http://itextpdf.com/">http://pdfbox.apache.org/</a>

### Gerador de gráficos charts
- <a>JFreechart – <a href="http://www.jfree.org/jfreechart/">http://www.jfree.org/jfreechart/</a>
- <a>HighCharts – <a href="http://www.highcharts.com/">http://www.highcharts.com/</a>

### Web Services REST
- <a>Jersey – <a href="http://jersey.java.net/">http://jersey.java.net/</a>
- <a>Restlet – <a href="http://www.restlet.org/">http://www.restlet.org/</a>
- <a>RestEasy – <a href="http://www.jboss.org/resteasy/">http://www.jboss.org/resteasy/</a>
- <a>Serfj – <a href="http://serfj.sourceforge.net/">http://serfj.sourceforge.net/</a>
- <a>CXF – <a href="http://cxf.apache.org/">http://cxf.apache.org/</a>

### Gerenciador de e-mails
- <a>Commons Email – <a href="http://commons.apache.org/email/">http://commons.apache.org/email/</a>
- <a>JavaMail – <a href="http://www.oracle.com/technetwork/java/javamail/index.html">http://www.oracle.com/technetwork/java/javamail/index.html</a>

### Web Services SOAP
- <a>Metro – <a href="http://jax-ws.java.net/">http://jax-ws.java.net/</a>
- <a>Axis – <a href="http://axis.apache.org/axis/">http://axis.apache.org/axis/</a>
- <a>XFire – <a href="http://xfire.codehaus.org/">http://xfire.codehaus.org/</a>
- <a>CXF – <a href="http://xfire.codehaus.org/">http://cxf.apache.org/</a>

### JavaScript
- <a>DOJO Toolkit - <a href="http://dojotoolkit.org/">http://dojotoolkit.org/</a>
- <a>JQuery - <a href="http://jquery.com/">http://jquery.com/</a>
- <a>Ext-JS - <a href="http://docs.sencha.com/ext-js/4-0/">http://docs.sencha.com/ext-js/4-0/</a>
- <a>DWR - <a href="http://directwebremoting.org/dwr/index.html">http://directwebremoting.org/dwr/index.html</a>

### Integração com redes sociais
- <a>Spring Social - <a href="http://www.springsource.org/">http://www.springsource.org/</a>

### Cache
- <a>Space4J – <a href="http://www.space4j.org/">http://www.space4j.org/</a>
- <a>Memcache - <a href="http://memcached.org/">http://memcached.org/</a>
- <a>Ecache – <a href="http://ehcache.org/">http://ehcache.org/</a>
- <a>Prevayler – <a href="http://prevayler.org/">http://prevayler.org/</a>
- <a>JBoss Infinispan – <a href="http://www.jboss.org/infinispan.html">http://www.jboss.org/infinispan.html</a>

### NoSQL
- <a>MongoDB – <a href="http://www.mongodb.org/">http://www.mongodb.org/</a>
- <a>Neo4j – <a href="http://neo4j.org/">http://neo4j.org/</a>
- <a>Db4o – <a href="http://www.db4o.com/">http://www.db4o.com/</a>
- <a>MemcachedDB – <a href="http://memcachedb.org/">http://memcachedb.org/</a>
- <a>CouchDB – <a href="http://couchdb.apache.org/">http://couchdb.apache.org/</a>
- <a>Project Voldemort – <a href="http://project-voldemort.com/">http://project-voldemort.com/</a>
- <a>MarkLkogic Server – <a href="http://www.marklogic.com/">http://www.marklogic.com/</a>
- <a>BaseX – <a href="http://basex.org/">http://basex.org/</a>
- <a>SimpleDB – <a href="http://aws.amazon.com/simpledb/">http://aws.amazon.com/simpledb/</a>
- <a>HBase – <a href="http://hbase.apache.org/">http://hbase.apache.org/</a>
- <a>Casandra – <a href="http://cassandra.apache.org/">http://cassandra.apache.org/</a>
- <a>Hypertable – <a href="http://hypertable.org/">http://hypertable.org/</a>
- <a>OrientBD – <a href="http://www.orientechnologies.com/">http://www.orientechnologies.com/</a>

### Gerenciador de schemas SGDB
- <a>Liquibase - <a href="https://www.liquibase.org/">https://www.liquibase.org/</a>
- <a>Flyway - <a href="https://flywaydb.org/documentation/">https://flywaydb.org/documentation/</a>

### SGDB Java embutidos
- <a>HyperSQL – <a href="http://hsqldb.org/">http://hsqldb.org/</a>
- <a>JavaDB – <a href="http://www.oracle.com/technetwork/java/javadb/overview/index.html">http://www.oracle.com/technetwork/java/javadb/overview/index.html</a>
- <a>Apache Derby – <a href="http://db.apache.org/derby/">http://db.apache.org/derby/</a>
- <a>H2Database – <a href="http://www.h2database.com">http://www.h2database.com</a>

### Testes
- <a>DBUnit – <a href="http://www.dbunit.org/">http://www.dbunit.org/</a>
- <a>JUnit – <a href="http://www.junit.org/">http://www.junit.org/</a>
- <a>EJBUnit – <a href="http://ejb3unit.sourceforge.net/">http://ejb3unit.sourceforge.net/</a>
- <a>JSFUnit – <a href="http://www.jboss.org/jsfunit/">http://www.jboss.org/jsfunit/</a>

### Loggin
- <a>jse – <a href="http://docs.oracle.com/javase/7/docs/api/java/util/logging/package-summary.html">http://docs.oracle.com/javase/7/docs/api/java/util/logging/package-summary.html</a>
- <a>Log4J – <a href="http://logging.apache.org/index.html">http://logging.apache.org/index.html</a>

### Testes cargas e perfomance
- <a>JMeter – <a href="http://jmeter.apache.org/">http://jmeter.apache.org/</a>
- <a>WebLoad – <a href="http://www.webload.org/">http://www.webload.org/</a>

### JSON
- <a>JSON – <a href="http://www.json.org/java/">http://www.json.org/java/</a>
- <a>XStream – <a href="http://xstream.codehaus.org/json-tutorial.html">http://xstream.codehaus.org/json-tutorial.html</a>
- <a>Google-JSON – <a href="http://code.google.com/p/google-gson/">http://code.google.com/p/google-gson/</a>

### Boletos bancárioBoletos bancário
- <a>Boletos Bancário - <a href="http://www.boletobancario.com.br">http://www.boletobancario.com.br</a>
- <a>Bopepo – <a href="http://www.jrimum.org/bopepo/">http://www.jrimum.org/bopepo/</a>
- <a>Stella – <a href="http://github.com/caelum/caelum-stella/wiki/Gerando-boleto">http://github.com/caelum/caelum-stella/wiki/Gerando-boleto</a>

### Manipulaçao de arquivos MS Office
- <a>Apache POI – <a href="http://poi.apache.org/">http://poi.apache.org/</a>
- <a>JExcelApi – <a href="http://jexcelapi.sourceforge.net/">http://jexcelapi.sourceforge.net/</a>
- <a>Docx4j – <a href="http://dev.plutext.org/trac/docx4j">http://dev.plutext.org/trac/docx4j</a>
- <a>Java Docx – <a href="http://www.javadocx.com/">http://www.javadocx.com/</a>
- <a>Aspose – <a href="http://www.aspose.com/categories/java-components/aspose.total-for-java/default.aspx">http://www.aspose.com/categories/java-components/aspose.total-for-java/default.aspx</a>
  
### Serverless Java Container
- <a>Spring - Java Container - <a href="http://maven.apache.org/">https://search.maven.org/#artifactdetails%7Ccom.amazonaws.serverless%7Caws-serverless-java-container-spring%7C1.0%7Cjar</a>

### Gerais
- <a>Maven – Gerenciador de dependências – <a href="http://maven.apache.org/">http://maven.apache.org/</a>
- <a>JLicense – Gerenciador de licenciamento de uso de software – <a href="http://www.websina.com/products/jlicense.html">http://www.websina.com/products/jlicense.html</a>

#### Boas práticas 
- [x] [Code Review](https://www.javacodegeeks.com/2021/04/guidelines-for-java-code-review.html)
- [x] Libs de teste para proteger a arquitetura das aplicações:
- [.NET](https://archunitnet.readthedocs.io/en/latest/)
- [JAVA](https://www.archunit.org/)

## 👨🏻‍🚀 Sobre mim
<a href="https://www.linkedin.com/in/mateus-macedo-937a32163/">
 <img style="border-radius:50%" width="100px; "src="https://avatars.githubusercontent.com/u/63172367?s=460&u=11fd26ea8a7f5663d7707d7ef254e4f8bfca1b05&v=4"/>
 <p>Mateus Macedo</p>
</a>

