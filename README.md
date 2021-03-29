<img src="https://s2.glbimg.com/TES0H8Evg6phh91YTFr0rCyCxTk=/90x68/s2.glbimg.com/EVEqLFXR5M5rFugYYWIQtAg05_E=/0x0:100x100/75x75/s.glbimg.com/po/tt2/f/original/2016/03/01/java.png" width="60" height="60">



<h1> JAVA </h1>
Este projeto é uma coleção de tutoriais pequenos e focados - cada um cobrindo uma área única e bem definida de desenvolvimento no ecossistema Java. Aqui esta estudo particulares tendo como primazia todos os conceitos da linguagem, levando em consideração o desenvolvimento de API'S nivel backend, toda parte de desenvolvimento e modelagem de dados com integração ao banco de dados, esta em outro repositorio.

# Executando os testes
O comando mvn clean installde dentro de um módulo executará os testes de unidade nesse módulo. Para módulos Spring, isso também executará oSpringContextTest if present.

>Para executar os testes de integração, use o comando: 

````
mvn clean install -Pintegration-lite-first ou
mvn clean install -Pintegration-lite-second ou
mvn clean install -Pintegration-heavy
````

dependendo da lista onde nosso módulo existe, os comandos serão executados com sucesso.

Dentro desse assunto, gostaria de publicar minha lista de frameworks e componentes Java utilizado nas minhas decisões arquiteturais no momento de arquiteturar uma solução. Qualquer sugestão é bem vinda!

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
- <a>Tomee –
- <a>Simpas –
- <a>Resin –
- <a>JBoss –
- <a>Glassfish –
- <a>Webshere –
- <a>WebLogic –
- <a>Geronimo –

### Relatórios
- <a>iReport –
- <a>DynamicReport –
- <a>Birt –
- <a>iText –
- <a>PDFBox –

### Gerador de gráficos charts
- <a>JFreechart –
- <a>HighCharts –

### Web Services REST
- <a>Jersey –
- <a>Restlet –
- <a>RestEasy –
- <a>Serfj –
- <a>CXF –

### Gerenciador de e-mails
- <a>Commons Email –
- <a>JavaMail –

### Web Services SOAP
- <a>Metro –
- <a>Axis –
- <a>XFire –
- <a>CXF –

### JavaScript

### Integração com redes sociais

### Cache

### NoSQL

### SGDB Java embutidos

### Testes

### Loggin

### Testes cargas e perfomance

### JSON

### Boletos bancárioBoletos bancário

### Manipulaçao de arquivos MS Office

### Gerais

## 👨🏻‍🚀 Sobre mim
<a href="https://www.linkedin.com/in/mateus-macedo-937a32163/">
 <img style="border-radius:50%" width="100px; "src="https://avatars.githubusercontent.com/u/63172367?s=460&u=11fd26ea8a7f5663d7707d7ef254e4f8bfca1b05&v=4"/>
 <p>Mateus Macedo</p>
</a>

