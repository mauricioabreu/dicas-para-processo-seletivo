# Dicas para o seu processo seletivo

Se você tem dificuldade de resolver os desafios de processos seletivos ou não sabe como se desenvolver em uma entrevista técnica, talvez as dicas a seguir podem te ajudar.

## Antes de aplicar para a vaga

Um melhor desempenho começa antes da entrevista, antes mesmo de você aplicar para a vaga que você viu na internet.

Conhecer a empresa que você vai trabalhar, como é o clima, remuneração e como a empresa ganha dinheiro são pontos que podem decidir se vale a pena o esforço mental gasto.

Se você é mulher cis ou trans, LGBTQIA+, pessoa preta ou que sofre preconceito por outras características, a sugestão é conferir se na empresa há pessoas com características semelhantes as suas. Isso pode ajudar a entender se a empresa vai proporcionar um lugar seguro para você se desenvolver.

## Desafio técnico

Concordando ou não com a aplicação de desafios técnicos, boa parte das empresas de tecnologia tem isso como parte principal do processo seletivo.

Ao receber o desafio, é importante ler todo o enunciado com calma. Caso você tenha perguntas, mande um e-mail para a empresa visando esclarecer os pontos que pareceram confusos.

### Escolhendo as tecnologias

Geralmente os desafios deixam em aberto a escolha da tecnologias a serem utilizadas. Dito isso, use a tecnologia que você mais domina. Isso é muito importante pois o seu projeto tende a ficar com uma qualidade maior, mais robusto e mais fácil de entender e explicar.

Vale ressaltar que a ferramenta que você mais domina não é a qual você sabe tudo sobre ela, mas sim a que te deixa mais confortável para escrever o código que resolve o problema, os testes, os scripts de execução, deploy, etc.

### Comente sobre suas decisões

Algumas empresas pedem que a pessoa candidata documente as decisões tomadas no projeto. Independente desse pedido existir, documentar os motivos de cada decisão pode elevar suas chances em busca de uma resposta positiva no processo, além de ser um ótimo exercício para sua evolução.

Se o seu projeto usa banco de dados, explique por qual motivo você escolheu um banco relacional, por exemplo:
> Eu escolhi o banco de dados PostgreSQL pois as entidades do projeto tem fortes relacionamentos. Além disso, a quantidade de joins nas consultas me levou a escolher esse banco. Adicionalmente, o suporte a JSON oferecido pelo banco de dados ajudou a resolver a parte X do problema.

Explique também porque você escolheu a linguagem:
> Eu escolhi a linguagem Rust porque ela é uma linguagem ótima pro problema. O problema exige muito uso de memória pois nele preciso traduzir um IP para coordenadas geográficas, e esse banco é mapeado em memória. Rust lida muito bem com memória. Outro fato é que a linguagem tem um suporte bom para programação funcional e ela é imutável por padrão, o que me ajuda a escrever um código mais correto.

Há muitos frameworks hoje em dia, e muitos extremamente populares. Fica até difícil escolher um às vezes, não é?
Explicar as decisões técnicas de um framework pode ir desde sua popularidade até sua base de desenvolvedores e limitações tecnicas que ele tem. Escolha um framework que você está acostumado e que você conheça como os pontos positivos dele podem ajudar você a resolver o problema.

### Escrevendo código

Desde a resolução de fizzbuzz, conjectura de Collatz, um jogo de luta ou uma aplicação web, é muito importante que seu código funcione como esperado. Abaixo segue uma lista de dicas para alcançar esse objetivo:

### Documentação

Produza uma documentação com os passos necessários para executar o projeto, para testar o projeto e até para verificar coverage, linters e outras ferramentas que podem aferir que você escreveu o código seguindo padrões já estabelecidos.

Não deixe de documentar o que você faria se tivesse mais tempo. Cada débito técnico que você deixou pode virar uma oportunidade de demonstrar como você resolveria se tivesse mais tempo e conhecimento.

Se o projeto for uma API web, use algum tipo de ferramenta como o [swagger](https://swagger.io/). Além da ferramenta documentar as principais rotas da sua API, ela também facilita o teste com uma UI poderosa.

### Resolvendo o problema

Essa é a etapa onde maior parte do nosso foco é concentrado, e não é à toa, pois esta é uma das partes que mais contam para entender o seu jeito de pensar ao resolver um problema. Abaixo uma lista de dicas para te ajudar a evoluir mais rápido e consistente na resolução:

* Escreva em algum lugar todos os passos que você acha necessários para chegar na solução;
* A seguir teste algumas hipóteses, mesmo sem testes. Elas vão te dar uma visão suficiente e com feedback rápido sobre a dificuldade do problema;
* Tudo bem se você não é do time que escreve testes antes do código, mas lembre de ir criando testes ao longo do desenvolvimento. Eles vão ajudar você a não quebrar o que já funciona;
* Tente cobrir com testes todos os casos de uso do desafio. Valide as entradas e saídas do programa. Cerifique-se de que você testou os diversos comportamentos apresentados pelo programa;
* Utilize Makefile ou scripts para acelerar builds, execução dos diversos testes, para subir a aplicação, etc. Não esqueça de colocar na documentação do projeto todas esses comandos;
* Valide bem sua solução. Não caia no [off by one error](https://en.wikipedia.org/wiki/Off-by-one_error). Teste seu código com entradas que você acha que podem gerar problemas. Se o problema em questão deve ser resolvido com um número pré-estabelecido de entradas, teste com algumas diferentes, explorando possíveis problemas que a própria empresa não previu;
* Facilite o teste do seu programa. Use alguma tecnologia de container ou provisionamento para que as pessoas revisoras não tenham que passar horas instalando os diversos componentes do seu desafio.

## Materiais para estudo

* [The System Design Primer](https://github.com/donnemartin/system-design-primer) é um guia de preparação para entrevistas. Nele você vai encontrar conhecimento sobre protocolos, bancos de dados, sistemas de cache, programas assíncronos, etc.