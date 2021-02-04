<img src="https://www.google.com/imgres?imgurl=https%3A%2F%2Fs2.glbimg.com%2F5pgaEIiZXIVWgSTOtfKBtm5AHaU%3D%2F695x393%2Fs2.glbimg.com%2FvME2Bq4OSpm6f6IE16BhcVLR98U%3D%2F695x0%2Fs.glbimg.com%2Fpo%2Ftt2%2Ff%2Foriginal%2F2014%2F11%2F14%2Fjava-logo.jpg&imgrefurl=http%3A%2F%2Fwww.techtudo.com.br%2Fdicas-e-tutoriais%2Fnoticia%2F2014%2F11%2Fjava-entenda-para-que-serve-o-software-e-os-problemas-da-sua-ausencia.html&tbnid=NFbiWp3iWLwSUM&vet=12ahUKEwj6ztDPkM_uAhXfCrkGHTsfCb4QMygAegUIARCpAQ..i&docid=FKWIPBReaovjTM&w=695&h=393&q=Java&ved=2ahUKEwj6ztDPkM_uAhXfCrkGHTsfCb4QMygAegUIARCpAQ" width="60" height="60">



# Liguagem de programação JAVA
Este projeto é uma coleção de tutoriais pequenos e focados - cada um cobrindo uma área única e bem definida de desenvolvimento no ecossistema Java.

# Executando os testes
O comando mvn clean installde dentro de um módulo executará os testes de unidade nesse módulo. Para módulos Spring, isso também executará oSpringContextTest if present.

Para executar os testes de integração, use o comando:

mvn clean install -Pintegration-lite-first ou

mvn clean install -Pintegration-lite-second ou

mvn clean install -Pintegration-heavy

dependendo da lista onde nosso módulo existe

