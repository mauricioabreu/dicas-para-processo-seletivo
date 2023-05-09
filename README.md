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
* Refatore seu código antes de enviar. Com os testes feitos, você tem segurança para modificar partes que você acredita estarem pouco legíveis. Leia atentamente o código que você escreveu e se imagine dando suporte a ele daqui a 3 meses. Se você acha que vai ter dificuldade de entendê-lo, sugiro refatorar.

### Pareamento

Algumas empresas adotam como etapa o pareamento de código com a pessoa candidata.

Nessa etapa você vai evoluir o desafio que você entregou, desenvolvendo novas extensões que vão desde novas features à mudanças expressivas nas características existentes.

Tem empresa que usa essa etapa para entender como a pessoa desevolve, qual o modelo racional ela utiliza para resolver problemas. Outras usam o momento para ver como a pessoa trabalha em time e como ela recebe críticas e sugesstões sobre o código. Independente de qual desses objetivos a empresa tem, leve em consideração:

* Revise as suas configurações de editor, de ambiente e qualquer outra coisa que possa virar um problema no dia;
* Receba críticas construtivas com calma, elas vão te ajudar a corrigir possíveis erros ou trabalhar em melhorias apontadas pelas pessoas que estão pareando com você. Não leve para o lado pessoal;
* Constantemente fale em voz alta o que você está pensando, mesmo se a ideia for absurda. Essa é uma ótima maneira de você demonstrar como você resolve problemas e, tambémm, ajuda as pessoas que estão com você a te guiar;
* Para cada extensão desenvolvida, crie um teste. Criar o teste antes ou depois do código interessa menos do que testar.

## Questões de backend

Algumas questões em entrevistas para vaga de backend são bem frequentes. Elas podem variar desde design de código do backend até utilização de bancos de dados, ferramentas de deploy, até conhecimentos específicos sobre _runtime_ de linguagens.

Abaixo descrevemos algumas perguntas e respostas. As respostas podem variar de acordo com o cenário proposto, então a dica é sempre coletar maiores detalhes sobre o objetivo da pergunta.

### Performance geral de aplicações

Performance é um tópico não exclusivamente está relacionado a CPU e memória. Performance é, também, sobre erros, latência, _freshness_, etc.

Um ponto genérico a se discutir sobre aplicações é que, sem medir, dificilmente você vai focar os esforços de otimização no lugar correto, e isso piora com o tamanho da sua aplicação e componentes envolvidos.

**Minha aplicação está demorando para carregar, como encontrar onde está o problema?**

Primeiro, verificar se há gráficos que mostrem mais informações da lentidão. Quais os horários, qual a aplicação, etc. Segundo, entender qual parte da aplicação está demorando, se é um job, uma rota de uma API.

Por fim, usar as ferramentas específicas pra isso. Se a aplicação já mede a latência (usando percentis, por exemplo) fica mais fácil ler o código relacionado para achar o problema.

Um caso extremamente comum é o mal uso de SQL. A falta de join, por exemplo, pode aumentar drasticamente o número de consultas em uma simples página.

**Aplicação está utilizando muita memória, como resolver?**

Identificar onde exatamente é o primeiro passo. Da minha experiência, boa parte do mal uso de memória tende a estar relacionado com largas coleções sendo carregadas em memória. Usar técnicas como lazy evaluation, generators, cursores e similares podem melhorar e muito a performance de aplicações web.

[Flamegraphs](https://www.brendangregg.com/flamegraphs.html) são ótimos pra entender, no detalhe, qual parte da sua aplicação está usando memória excessiva. Entender onde exatamente mora o problema com números é mais produtivo do que analisar o código linha a linha eliminando casos usando intuição.

### Go

Go é uma linguagem que tem sido muito usada para criar micro-serviços e há grandes aplicações escritas nela, como o Kubernetes, além de outros inúmeros softwares de vídeo, chat e ferramentas de observabilidade, como Prometheus e Grafana.

**Como otimizar a performance de um programa em go?**

* [Concorrência](https://go.dev/doc/effective_go#concurrency): use quando você pode disparar rotinas que são usadas como jobs, por exemplo. Uma prática comum é você fazer cache de dados usando _goroutines_, exemplo: faz cache de dados de 5 em 5 minutos de uma API, sem uso de uma engenharia mais complexa de fila de jobs usando Redis.
* [Context](https://pkg.go.dev/context): _Context_ é um pacote do Go que ajuda programas a economizarem recursos. Se você tem uma rota na sua API que a query no banco de dados demorou, você pode usar esse pacote para gerenciar o cancelamento dessa query, liberando recurso pra outras queries a serem feitas no banco.

[Benchmarks](https://pkg.go.dev/testing#hdr-Benchmarks) fazem parte do framework nativo de teste do go.

## Materiais para estudo

* [The System Design Primer](https://github.com/donnemartin/system-design-primer) é um guia de preparação para entrevistas. Nele você vai encontrar conhecimento sobre protocolos, bancos de dados, sistemas de cache, programas assíncronos, etc.
* [Refatoração](https://novatec.com.br/livros/refatoracao/) aqui um livro focado em refatoração de código. O livro discute e mostra técnicas para escrever código que seja mais fácil de entender, além de demonstrar quando se deve refatorar, como e porque e até entender quando um código não está legível o suficiente.
* [Entendendo algoritmos](https://www.amazon.com.br/Entendendo-Algoritmos-Ilustrado-Programadores-Curiosos/dp/8575225634) é um livro que explica famosos algoritmos e como aplicá-los. Além disso, o livro fala sobre [Complexidade de tempo](https://pt.wikipedia.org/wiki/Complexidade_de_Tempo), um tópico importante para você entender, de pequenas à grandes empresas.
