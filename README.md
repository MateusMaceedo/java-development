<img src="https://s2.glbimg.com/TES0H8Evg6phh91YTFr0rCyCxTk=/90x68/s2.glbimg.com/EVEqLFXR5M5rFugYYWIQtAg05_E=/0x0:100x100/75x75/s.glbimg.com/po/tt2/f/original/2016/03/01/java.png" width="60" height="60">



<h1> JAVA </h1>
Este projeto é uma coleção de tutoriais pequenos e focados - cada um cobrindo uma área única e bem definida de desenvolvimento no ecossistema Java. Aqui esta estudo particulares tendo como primazia todos os conceitos da linguagem, levando em consideração o desenvolvimento de API'S nivel backend, toda parte de desenvolvimento e modelagem de dados com integração ao banco de dados, esta em outro repositorio.

# Executando os testes
O comando mvn clean installde dentro de um módulo executará os testes de unidade nesse módulo. Para módulos Spring, isso também executará oSpringContextTest if present.

````
Para executar os testes de integração, use o comando:
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








