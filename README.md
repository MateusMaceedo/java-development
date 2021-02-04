<a title="java.com" class="desktopOracleLogo jvl0 hidden-xs" data-bind="attr: { href: SCSRenderAPI.getPageLinkUrl(SCS.navigationRoot).substring(0,SCSRenderAPI.getPageLinkUrl(SCS.navigationRoot).lastIndexOf('/')+1) }" href="/pt-BR/"><span class="headerLogo">Oracle</span></a>

# Liguagem de programação JAVA
Este projeto é uma coleção de tutoriais pequenos e focados - cada um cobrindo uma área única e bem definida de desenvolvimento no ecossistema Java.

# Executando os testes
O comando mvn clean installde dentro de um módulo executará os testes de unidade nesse módulo. Para módulos Spring, isso também executará oSpringContextTest if present.

Para executar os testes de integração, use o comando:

mvn clean install -Pintegration-lite-first ou

mvn clean install -Pintegration-lite-second ou

mvn clean install -Pintegration-heavy

dependendo da lista onde nosso módulo existe


