### Estudos Desenvolvimento Java Pleno

- Java 8, Spring Boot, Mensageria e REST/SOAP;
- Design Patterns;
- Conhecimento em AWS cloud: EC2, ELB, S3, CloudWatch, Route53, API Gateway, Beanstalk e Lambda;
- Desejável conhecimento em Testes Unitários (JUnits), Jenkins, Docker, Kubernetes e arquitetura de microsserviços;
- Desejável conhecimento em Kotlin.
- Experiência em: Java 8+ 
- Spring Boot 
- Cloud Azure 
- S.O.L.I.D 
- SQLm NOSQL 
- Swagger 
- Junit 
- Mockito 
- Git Gradlew/Maven 
- REST/SOAP
- Multithreading 
- Design Patterns 
- DDD 
- Docker  
- Arquitetura de microservices.
- Experiência em Java 8+
- spring boot,
- swagger,
- API’s,
- microsserviços;
- Banco de Dados Oracle;
- Desejável conhecimento em Angular 2+;
- Desejável Apache Camel;

- [x] Backend

APIs in the following stacks: Spring Framework/JPA/JDK8/Redis/Maven/IBM MQ/SQL Server
Besides projects, also working to improve Run the Bank concepts using SRE Models for increasing their reliability, performing regression and system-level testing to verify software quality and function prior to release.

Main technologies:
Java 8 – Spring, JPA,Hibernate, Rest Api, SOAP webservice
COBOL – IBM Rdz, TSO, Cobol 6, DB2
• Framework: Spring, EJB, JPA, Hibernate, Spring, JUnit, IBM RDz
• Development Methodology: Scrum and Waterfall
• Microservices, TDD, DDD
• Maven, Artifactory, Sonar, Fortify
• Observability (Splunk, AppDynamics)

#### 1. Aplicação de interfaces e classes abstratas

##### 1.1 Interface

- Suporta Herança Múltipla: Uma classe pode implementar múltiplas interfaces;
- Permite apenas métodos abstratos: Nenhum método com implementação. Temos algumas exceções que chegaram com o Java 8, mas essa é a ideia principal;
- Não contém atributos: Essa é outra regra que possui uma exceção. Enquanto é comum ouvirmos que interfaces não guardam o estado da classe por não suportarem a instância de atributos, elas ainda podem conter atributos constantes de classe (public static final);
- Não contém construtor
- Quando utilizar? O ideal é utilizar a interface quando várias classes diferentes compartilham apenas a assinatura de seus métodos. Em outras palavras, podemos ter várias classes sem qualquer relação entre si, mas se elas compartilharem as funcionalidades oferecidas pela interface que estamos criando, então faz total sentido que essas classes a implementem. Conclusão: interfaces estão aí para ditar o que uma classe deve fazer, ajudando a definir quais habilidades as classes que assinarem esse "contrato" devem possuir.

##### 1.2 Classe abstrata

- Não suporta Herança Múltipla
- Pode conter métodos concretos ou abstratos: Isso quer dizer que todos os métodos de uma classe abstrata podem ser tanto concretos como, também, todos podem ser abstratos;
- Pode conter atributos de todos os tipos
- Contém construtor
- Quando utilizar? Diferente da interface que pode estar envolvida com diversas classes sem qualquer relação entre si, uma classe abstrata continua sendo uma classe. E sabemos que quando uma classe X herda de uma classe Y é o mesmo que dizer que X é um Y. Ou seja, quando queremos criar várias classes que irão compartilhar um mesmo comportamento, uma classe abstrata é o componente ideal para ser a base para criação de todas elas, servindo como um molde para as futuras classes que irão derivar dela. Conclusão: classes abstratas definem a identidade de suas classes derivadas ditando o que e como uma classe deve se comportar, o que aumenta o acoplamento entre classes, porém faz total sentido em algumas situações.

#### 2. Aplicação de ORM e Driver Nativo

##### 2.1 ORM  

ORM (Object Relational Mapper) é uma técnica de mapeamento objeto relacional que permite fazer uma relação dos objetos com os dados que os mesmos representam.

- [Hibernate é o framework para persistência de dados mais utilizado em projetos Java.](https://www.devmedia.com.br/guia/hibernate/38312)
- [NHibernate é livre e de código aberto (open source) e é a versão portada do Java para o Microsoft .NET do Hibernate.](https://www.devmedia.com.br/introducao-ao-nhibernate-framework-para-mapeamento-objeto-relacional/28671)
- [Entity Framework](https://www.devmedia.com.br/entity-framework-tutorial/27764)

##### 2.2 Driver Nativo (JDBC)

O driver JDBC é o fator mais importante na performance de aplicações que utilizam base de dados para armazenar e filtrar informações.

- [Java JDBC: Melhorando o Desempenho de Aplicações Java](https://www.devmedia.com.br/java-jdbc-melhorando-o-desempenho-de-aplicacoes-java/31976)

#### 3. Padrões de Arquitetura de projetos

>EX: Aplicação usando MVC, acesso a banco de dados com DAO, arquitetura de integração com SOA e REST.

##### 3.1 Definições e Acrônimos

|ACRÔNIMO	| DESCRIÇÃO                                                        |
----------| -----------------------------------------------------------------|
|IHM	    | Interface Homem Máquina                                          |
|JSP	    | Java Server Pages (Páginas Java)                                 |
|POJO	    | Plain Old Java Object (Objeto Java Simples)                      |
|OS	      | Operational System (Sistema Operacional)                         |
|MVC	    | Model View Controller (Modelo Visão Controle)                    |
|DAO	    | Data Access Object (Objeto de Acesso à Dados)                    |
|JEE	    | Java Enterprise Edition (Java Edição Corporativa)                |
|DI	      | Dependency Injection (Injeção de Dependência)                    |
|IOC	    | Inversion of Control (Inversão de Controle)                      |
|SOA	    | Service Oriented Architecture (Arquitetura Orientada ao Serviço) |
|UML	    | Unified Modeling Language (Linguagem de Modelagem Unificada)     |
|TLD	    | Tag Library Descriptor (Descritor da Biblioteca de Tags Java)    |
|JPA	    | Java Persistence API (API de Persistência Java)                  |

##### 3.2 Arquitetura lógica

A arquitetura das aplicações deve ser de no mínimo 3 camadas: • clientes simples do tipo navegador Web, que se contentam em enviar as requisições dos usuários aos sistemas• um servidor de aplicações JEE ou Web que contenha o core das aplicações • um servidor de dados, com bases de dados relacionais para realizar a persistência dos dadosOs servidores de aplicações e de bases de dados podem ser múltiplos (cluster) para realizar o balanceamento de carga sem impactar nas 3 camadas. Os postos cliente deverão estar equipados com um navegador Web independente do contexto do projeto (intranet, internet, extranet). Por padrão exige-se que as aplicações sejam compatíveis com o Mozilla FireFox e IE. O servidor de aplicações será o Glassfish. Como servidor web para testes locais poderá ser utilizado o Jetty ou Tomcat.O servidor de base de dados deverá ser por padrão o PostgreSQL (eventualmente a base de dados Caché e Sybase para os sistemas legados).

#### 4. Padrões de projetos

- [A importância dos Padrões de Projeto](https://www.devmedia.com.br/a-importancia-dos-padroes-de-projeto/22549)

Quando utilizados de forma correta, os padrões de projeto colaboram para a obtenção de um design flexível, mais coeso e menos acoplado.

##### 4.1 Padrões criacionais

> Abstract Factory 
- Permite que você produza famílias de objetos relacionados sem ter que especificar suas classes concretas.

> Adapter 
- Permite a colaboração de objetos de interfaces incompatíveis.

> Builder 
- Permite construir objetos complexos passo a passo. O padrão permite produzir diferentes tipos e representações de um objeto usando o mesmo código de construção.

> Bridge 
- Permite que você divida uma classe grande ou um conjunto de classes intimamente ligadas em duas hierarquias separadas—abstração e implementação—que podem ser desenvolvidas independentemente umas das outras.

> Factory Method 
- Fornece uma interface para criar objetos em uma superclasse, mas permite que as subclasses alterem o tipo de objetos que serão criados.

> Composite 
- Permite que você componha objetos em estrutura de árvores e então trabalhe com essas estruturas como se fossem objetos individuais.

> Prototype 
- Permite que você copie objetos existentes sem fazer seu código ficar dependente de suas classes.

> Decorator 
- Permite que você adicione novos comportamentos a objetos colocando eles dentro de um envoltório (wrapper) de objetos que contém os comportamentos.

> Singleton 
- Permite a você garantir que uma classe tem apenas uma instância, enquanto provê um ponto de acesso global para esta instância.

> Facade 
- Fornece uma interface simplificada para uma biblioteca, um framework, ou qualquer outro conjunto complexo de classes.

> Flyweight 
- Permite que você coloque mais objetos na quantidade disponível de RAM ao compartilhar partes do estado entre múltiplos objetos ao invés de manter todos os dados em cada objeto.

> Proxy 
- Permite que você forneça um substituto ou um espaço reservado para outro objeto. Um proxy controla o acesso ao objeto original, permitindo que você faça algo ou antes ou depois do pedido chegar ao objeto original.

##### 4.2 Padrões comportamentais

> Chain of Responsibility 
- Permite que você passe pedidos por uma corrente de handlers. Ao receber um pedido, cada handler decide se processa o pedido ou passa para o próximo handler da corrente.

> Command 
- Transforma o pedido em um objeto independente que contém toda a informação sobre o pedido. Essa Transformação permite que você parametrize métodos com diferentes pedidos, atrase ou coloque a execução do pedido em uma fila, e suporte operações que não podem ser feitas.

> Iterator 
- Permite que você percorra elementos de uma coleção sem expor as representações estruturais deles (lista, pilha, árvore, etc.)

> Mediator 
- Permite que você reduza as dependências caóticas entre objetos. O padrão restringe comunicações diretas entre objetos e os força a colaborar apenas através do objeto mediador.

> Memento 
- Permite que você salve e restaure o estado anterior de um objeto sem revelar os detalhes de sua implementação.

> Strategy 
- Permite que você defina uma família de algoritmos, coloque-os em classes separadas, e faça os objetos deles intercambiáveis.

> Template Method 
- Define o esqueleto de um algoritmo na superclasse mas deixa as subclasses sobrescreverem etapas específicas do algoritmo sem modificar sua estrutura.

> Visitor 
- Permite que você separe algoritmos dos objetos nos quais eles operam.

#### 5. Diferenças entre Padrões de Projeto e Padrões Arquiteturais:

Padrões de projetos, porque aplicar?

- Encurta a sua decisão, você acaba tomando as decisões mais rapido.
- Facilita em varias areas, como exemplo aréa de passagens de conhecimento como unboarding, pra outras areas, equipes etc..
- Ajuda a ser assertivo, na hora de encontrar e resolver problemas.

Padrões de arquitetura, porque aplicar?

- Padrões estruturais, definem a estrutura e responsabilidade das camadas, define como a sua aplicação será dividida;
- Facilidade em manuntenção, porque o código sera sempre igual, mudando apenas as regras;
- Facidade na hora de explicar o fluxo da aplicação, para gerar insumos para novas implementações;
- Aumento de produtividade;
- Uniformidade na estrutura do software;
- Redução de complexidade no código;
- As aplicações ficam mais fácies de manter;
- Facilita a documentação;
- Estabelece um vocabulário comum de projeto entre desenvolvedores;
- Permite a reutilização de módulos do sistema em outros sistemas;
- É considerada uma boa prática utilizar um conjunto de padrões para resolver problemas maiores que, sozinhos, não conseguiriam;
- Ajuda a construir softwares confiáveis com arquiteturas testadas;
- Reduz o tempo de desenvolvimento de um projeto.

#### 5.1 Vantagens e desvantagens do padrão MVC

- Separação muito clara entre as camadas de visualização e regras de negócios;
- Manutenção do sistema se torna mais fácil;
- Reaproveitamento de código, principalmente da camada de modelo, que pode ser reutilizada em outros projetos;
- As alterações na camada de visualização não afetam as regras de negócios já implementadas na camada de modelo;
- Permite o desenvolvimento, testes e manutenção de forma isolada entre as camadas;
- O projeto passa a ter uma melhor organização em sua arquitetura;
- Torna o entendimento do projeto mais fácil para novos programadores que não participaram de sua criação.
- As desvantagens são poucas, mas alguns desenvolvedores acabam não usando o padrão MVC por conta delas, veja algumas:
- Em sistemas de baixa complexidade, o MVC pode criar uma complexidade desnecessária;
- Exige muita disciplina dos desenvolvedores em relação à separação das camadas;
- Requer um tempo maior para modelar o sistema.

#### 5.2 Exemplos de padrões arquiteturais:

- [MVC - O Padão MCV (modelo Model-View-Controller)](https://www.devmedia.com.br/padrao-mvc-java-magazine/21995)
- [MVP - O Padrão MVP (Model-View-Presenter)](https://www.devmedia.com.br/o-padrao-mvp-model-view-presenter/3043)
- [N-TIERS - O Padrão N-TIES (Arqui-N-Camadas)](https://pt.stackoverflow.com/questions/26735/o-que-realmente-%C3%A9-uma-aplica%C3%A7%C3%A3o-n-tier)
- [MVVM - O Padrão MVVM (Model-View-ViewModel)](https://www.devmedia.com.br/entendendo-o-pattern-model-view-viewmodel-mvvm/18411)

#### Como funciona a arquitetura monolítica

As principais linguagens de desenvolvimento de aplicações oferecem abstrações para quebrar a complexidade dos sitemas em módulos. Entretando. são projetadas para a criação de um único executável monolítico, no qual toda a modularização utilizada é executada em uma mesma máquina. Assim, os módulos compartilhar recursos de processamento, memória, banco de dados e arquivos.

Uma arquitetura monolítica típica de um sistema complexo pode ser representada pela fica abaixo, na qual todas as funções de negócio estão implementadas em um único processo.

#### Desafio da arquitetura monolítica

Ao longo do tempo o sistema vai crescendo, se tornando compleo e consumindo cada vez mais recursos, o que acaba gerando também alguns desafios substanciais para a manuntenção desse tuoi de arquitetura. São eles:

- Aumento da complexidade e tamanho ao longo do tempo 
O sitema se torna tão complexo que a manuntenção fica cada vez mais cara e lenta, porque os desenvolvedores têm que navegar em uma infinidade de códigos.

- Alta dependência de componenetes de código
Muitas funcões são interdepentes e entreleçadas, de forma que a inclusão ou manuntençaõ de componentes do sistema pode causas inconsistências ou comportamentos inesperados.

- Escalabilidade do sistema é limitada
Mesmo que apenas parte da funcionalidade seja necessária na nova instância, uma arquitetura monolítica exige que todos o sistema seja replicado, o que gera custos maiores do que o esperado.

- Falta de flexibilidade
Exige que os desenvolvedores fiquem amarrados à tecnologia originalmente escolhida para o sistema, mesmo que em algumas situações ela não seja a melhor escolha.

- Dificuldade para colocar alterações em produção
Qualquer mudança, por menor que seja, requer a reinicialização do sistema. Como isso pode causar algum risco operacional, é necessário que as equipes de desenvolvimento testes e manuntenção desse sistema acompanhem essas alterações.

#### Como funciona a arquitetura de micro serviços
A arquitetura de micro serviços é utilizada para desenvolver uma aplicação como um conjunto de pequenos serviços, que funcionam com seu próprio processo. Cada serviço é desenvolvido em torno de um conjunto de regras de negócio específicas, e é implementado de forma independente.

Com isso, é possível quebrar algumas barreiras existentes no modelo de arquitetura monolítica.

Benefícios dos micro serviços
- Manuntenção e evolução dos serviços mais estáveis
Como os desenvolvedores vão trabalhar com códigos que executam uma única função, os serviços individuais não vão acompanhar o potencial crescimento do sistema, evitando que precise carregar uma parte desnecessária da aplicação.

- Serviços com baixo nivel de acomplamento e interdependência
A manuntenção em um serviço especifico não interfere diretamente nas outras funcionalidades do sistema.

- Escalabilidade do sistema
Os deploys e replicações de micro serviços são feitos por meio de infraestrutura de servidores, máquinas virtuais e containers que se organizem de forma independente. Isso torna o crescimento e a possibilidade de adaptação do sistema muito mais flexível.

- Redução de custos
Cada aplicação só utiliza os serviços que necessita. Por isso, você não vai ter gastos extras carregando funcionalidades não utilizadas, afinal os custos estão diretamente associados à funcionalidade e à carga de uso do sistema.

- Flexibilidade de tecnologia
Por conta de baixo acoplamento entre os serviços, não é necessario amarrar os desenvolvedores a uma tecnologia específica, o que te permite escolher a melhor opção para atender cada caso. 

Isso diminui os riscos de obdolescência tecnológica e possibilita a evolução constante do sistema.

- Facilidade de colocar alterações em produção
As mundanças no sistema são executadas por meio de alteraões e evoluções feitas nos serviços. Portanto, o sistema como um todo não precisa ser reinicializado para continuar funcionando. 

Assim, o time de desenvolvimento que vai precisar acompanhar a mudança será apenas o de responsáveis pelos serviços que estão sendo alterados.

Porque os micro serviços são importantes para os negócios?

- Foco na experiência do usuário:
Dinamismo e interatividade são conceitos que não podem ficar de fora quando o assunto é entregar valor para o usuário, independentemente da plataforma (o que inclui também os dispositivos móveis);

- Escalabilidade: 
As aplicações desenvolvidas precisam estar altamente disponiveis. Além disso, deve ser possivel executá-las em ambiente de nuvem;

- Atualizações suaves e tranquilas:
O ideal é que as atualizações não ocasionem paradas ou instabilidades que prejudiquem os usuários.

#### Quando usar Kafka ou RabbitMQ?

- Kafka é ideal para casos de uso de big data que exigem o melhor rendimento.
- RabbitMQ é ideal para entrega de mensagens de baixa latência, garantias por mensagem e roteamento complexo.
