<img src="https://s2.glbimg.com/TES0H8Evg6phh91YTFr0rCyCxTk=/90x68/s2.glbimg.com/EVEqLFXR5M5rFugYYWIQtAg05_E=/0x0:100x100/75x75/s.glbimg.com/po/tt2/f/original/2016/03/01/java.png" width="60" height="60">



#### JAVA
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






