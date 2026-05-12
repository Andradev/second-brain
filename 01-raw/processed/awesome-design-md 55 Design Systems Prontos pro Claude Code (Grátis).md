---
title: "awesome-design-md: 55 Design Systems Prontos pro Claude Code (Grátis)"
source: "https://www.youtube.com/watch?v=S6IP41RnE5w&t=171s"
author:
  - "[[Matheus Battisti - Hora de Codar]]"
published: 2026-04-25
created: 2026-05-10
description: "IA gera código bom mas a UI sai feia. Resultado: tudo parece o mesmo template Tailwind genérico. Existe um arquivo markdown que muda isso completamente e um ..."
tags:
  - "WebClip"
---
![](https://www.youtube.com/watch?v=S6IP41RnE5w)

## Transcript

### How Awesome Design MD works

**0:00** · Chega de design genérico e feio. Um cara criou um repositório com referências de design das maiores marcas e com melhor design do mundo. Ou seja, tu vai ter acesso a um arquivo com orientações para uma IA gerar um site ou um projeto com o design de marcas famosas e isso vai resultar em projetos com designs excelentes. É isso que a gente vai ver nesse vídeo. A gente vai aprender a utilizar esse repositório e criar sites com excelentes designs.

**0:30** · Eu sou Mateus Batista, programador há mais 10 anos e hoje estô me aventurando muito no mundo daá e trazendo só as melhores novidades para vocês como essa. Então se tu curtiu a ideia não esquece, deixa o like e também se inscreve aí para receber vídeos todos os dias. Agora sim, bora lá entender melhor essa história e aplicar no Cloud Code. Chega aí. Então galera, só um primeiro disclaimer fundamental, não precisa ser cloud code, tá? Vou usar aqui por conveniência, beleza? Eu acredito também o resultado tende a ser melhor. Então o repositório é esse aqui.

### DESIGN.md + Claude Code to create amazing UIs

**1:02** · Vou deixar o link na descrição também, tá? Aome Design MD. Ele tem uma coleção de designs MD, tá? Para tu poder usar de marcas que tm designs ou e layouts excelentes, tá? Então vamos lá. Que que é? Basicamente, design systems em Markdown, criado pelo Google Stitch, cores, tipografia, componentes, LLMs, lenativamente.

**1:23** · Então, o cara foi conseguiu fazer uma engenharia reversa do design de um site X e extraiu o design MD dele, né, que é o design system e a gente consegue tá utilizando em qualquer projetos. Esse repositório que eu mostrei para vocês, tá? Ele, cara, ele tava, ele cresceu de forma insana, tá com 48.000 1000 stars aqui.

**1:43** · Deixa eu acompanhar o crescimento.

**1:44** · Tinha, é, não tem aqui, mas eu tinha levantado ele faz um tempo e agora que eu vou fazer o vídeo, né? Ele tá até atualizadinho, né? Dois quatro dias atrás. Beleza. Então, o cara tá, aliás, aqui o design medir, onde tem os designs cinco dias atrás. Então ele tá colocando mais também, tá? Botei 30 mais, deve ter mais. Agora como é que tu usa? Você vai copiar o GitHub, né? Copiou o código lá, o medir, só um arquivo de texto, cola na raiz do projeto e pede pro cloud utilizado, faz uma referência a ele, a cria tal projeto seguindo essa linha de design aqui. Bem simples, tá? Tem várias marcas top, né?

**2:14** · Linear, Stripe, Versel, Notion, só marca grande que pagou designers, designers para poder fazer aquele layout. Tu vai conseguir replicar isso facilmente. Não é um clone de um projeto, tá? Então, tu não tá clonando o site do Stripe, tu tá clonando basicamente as linhas e ideias de design dele. Então, tu vai ter uma linguagem visual que não copia logo nem conteúdo, tokens, CSS são públicos e o produto novo, né, que é o teu, segue a estética da marca. Basicamente isso, tá?

**2:44** · Aqui eu vou trazer dois projetos, tá? um seguindo o liner e outro seguindo o stripe paraa gente poder entender como que esse framework, pra gente entender como esse repositório vai se portar, tá?

**2:58** · Vou abrir o site aqui rapidinho. Então o liner é esse aqui, né, galera? Esse produto aqui eu vou fazer um site baseado nele, nesse design aqui, tá? Pra gente comparar depois. E o stripe é esse aqui. Eu vou fazer uma dashboard baseada na dashboard do Stripe, tá? Que é o sistema de pagamentos. Bom, vamos começar então. Só antes não se esquece, né? Estamos com as inscrições abertas da formação Vibe Coding lá. lá é onde tu vai aprender tudo que tu vê aqui no canal de forma mais profunda. Cloud Code, Antigaraft, Codex. Agora a gente tá lançando o curso de Open Code. Tô até produzindo ele aqui, tá aberto, tá?

**3:25** · Se tu quer dominar essa criação de projetos assistidas com IA, né, o Vibe Coding, se matricula no treinamento, aproveita acesso vitalício, grupo VIP no WhatsApp, condição especial, link aqui no comentário fixado, beleza? Tô te esperando lá. Bom, vamos seguir aqui.

### Creating a Landing Page with Claude Code and Awesome Design MD

**3:40** · Então, eu tô aqui com o VS Code aberto e agora eu vou abrir o cloud code, tá?

**3:46** · Então vamos abrir ele rapidão. Bom, aí fechou, tá? Agora que que eu vou ter que fazer? Vou ter que copiar o design medir, tá? E mandar um prompt para ele criar o projeto em cima daquele arquivo.

**3:59** · Então vamos utilizar o do liner, como eu falei antes. Então tu vai vir aqui, tu vai achar o que tu quer, ó, tá aqui, ó, liner me. E que a gente acessa esse link aqui, tá? E ele vai ter o design medir aqui, tá? Então ele traz toda as informações numa página, né? Eu posso estar utilizando esse comando aqui para baixar o design MD. Então vamos voltar aqui.

**4:24** · Vou fazer assim, ó. Crie uma pasta chamada linear clone e execute este comando para trazer o design em medida o projeto. Vou colocar o comando aqui, tá?

**4:40** · Então eu já vou criar a pasta do projeto e tal, né? E aí vou pedir para ele executar e criar o arquivo. E depois eu vou fazer um promptência ao design MD, tá? E também a criação do projeto. Ó, então ele trouxe aqui, esse é o design system do Lineer, tá? Tem todas as explicações necessárias pro cloud code entender o que ele tem que fazer ou trar, tá galera? E aqui agora eu vou colar um prompt para ele seguir esse design medido.

**5:11** · Então dentro do da pasta línea clone seguindo o design medir, crie este projeto. Aí eu pedi aqui crie uma landing page completa de SAS de gerenciamento de tarefas chamado Tesk Flow. Quero herer com hero com headline, headline e CTA. Sessão de features com quatro cards, sessão de pricing com três planos e footer. Uso anex jss com app router, ta wind, chatn. Quero algo bonito e profissional.

**5:42** · Então pronto. É basicamente isso aqui. Não tem muito mistério. Agora ele vai criar o projeto e a gente vai ver o resultado e comparar com Lineer de fato, tá? Galera, para quem não sabe também a gente tem uma playlist aqui de cloud code, tá?

**5:53** · praticamente um curso, mais de 40 vídeos, tudo gratuito para ti. Vou deixar aqui a tum do primeiro vídeo, o editor vai deixar para mim, que é um cursinho de cloud code para tu aprender os fundamentos da ferramenta e o izinho aqui, tu vai direto pra playlist, beleza? Então, acessa lá que vale a pena. Agora vamos aguardar ele criar aqui, só para recapitular, né, galera? A gente vai fazer esse processo sempre que a gente precisar criar o projeto. Então, ah, eu quero o design system da Ferrari.

**6:16** · Ah, daí vem para cá, quero design system da Apple, vem para cá, da BMW. É basicamente isso, não tem muito mistério, só vamos ver se ele realmente respeita, né, se a consegue replicar os layouts, pelo menos semelhantes, né?

**6:29** · Vamos entender qual que é a profundidade de utilizar essa estratégia. Então, ó, galera, ele entregou aqui para mim e ele, eu pedi para iniciar aqui, então ele falou que segui o design system, né, que a gente que a gente entregou para ele, tá? Ele deu passo a passo para iniciar, mas eu pedi para ele iniciar porque tinha preguiçoso, né? Então vou clicar aqui e olha só, ficou bem interessante mesmo, ó. Então esse aqui é o criado com design system, né?

**6:57** · Esse aqui eu li, né? Então claro, tem alguns tons, tal, porque assim, a empresa pode mudar, né? O site também, daí o cara tem que mudar o arquivo.

**7:06** · Mas vejam que segue o mesmo padrão, né?

**7:09** · Bem parecido mesmo. Isso aqui ficou legal. Agora eu vou criar a dashboard seguindo o design system da stripe.

**7:17** · Então a ideia é muito parecida. Ter que ir lá. Acho o stripe. Achei o stripe, vem para cá. Copio o npx.

**7:26** · Agora vou botar aqui crie uma pasta chamada dashboard stripe e eh baixe o design medir com coloco o comando e até eu vou fazer o seguinte. Olha só.

### Creating a Dashboard with Claude Code and Awesome Design MD

**7:42** · Dá um clear, crie uma pasta chamada landing page test e execute este projeto. Eu vou pedir para ele criar agora o mesmo projeto que o mesmo prompio anterior sem o design med. Tá aqui também. Inicie o projeto para mim, só pra gente colocar lado a lado para ver se vai ser muito diferente.

**8:05** · Galera, enquanto a gente vê essa comparação, não esqueçam de baixar o nosso guia de gera de propt, tá? Esse material tá gratuito aqui na descrição desse vídeo. Ele vai te ensinar a escrever promp melhores. Se tu quer aprender a criar prompts assertivos que realmente vão te ajudar a criar projetos melhores, economizar tokens, esse material é essencial. Beleza? Então baixa lá e aproveita. Vou voltar aqui e vou esperar ele me entregar para mim. Ó, galera, então ele me entregou aqui, tá?

**8:32** · Vamos utilizar o 3003 como ele me entregou, né? Deixa eu ver aqui, ó. Bom, eu não pedi tema light dark, né? Mas vejam aqui o resultado, tá? Não ficou tão ruim também, né?

**8:48** · Aliás, não ficou ruim, né? Mas não ficou tão premium quanto o nosso. Tá, deixa eu ver aqui.

**8:56** · É, eu preferia do liner, né? Não sei se por causa do tema dark e tal, mas me chamou mais atenção. Mas mesmo sem design, né? O Cloud também tem ideia de como gerar algo, OK? Tá, essa fonte serifada também acho que não pegou muito bem, mas dá para usar, né? Só que com o design MD, a gente vai ter também uma base para todo o sistema, né? A sequência do sistema para criar as próximas páginas, ele vai ajudar a gente também. Beleza? Então agora vamos testar o dashboard. Vou dar um clear também aqui para não pegar contexto.

**9:27** · Vamos fazer assim, ó. na pasta dashboard stripe.

**9:34** · Siga o design med. Não é esse aqui, ó.

**9:40** · Esse design medir aqui, tá? E crie o seguinte projeto. Colocar agora para criar uma dashboard, né? Pode ser algo mais ou menos assim. Cria um dashboard analytics completo. Quero sa barra esquerda com navegação, dashboard tasks, team settings e billing. Header no topo com search, notificações e avatar. Quatro card de mé métricas no topo. Gráfico de linha mostrando eh revenue dos últimos seis meses.

**10:09** · Gráfico de barras com top customers, gráfico de pizza de traffic sources, tabela de transações recentes com oito linhas e a stack definida aqui, tá? Então ele vai criar o projeto agora.

**10:22** · utilizando os conhecimentos do design medido do Stripe e também as solicitações que a gente pediu aqui.

**10:26** · Vamos ver como é que fica, se realmente fica parecido com Stripe, né? Lembrando que eu não estou logado no Stripe, né?

**10:31** · Mas ele tem essa cara. Ah, deixa eu ver aqui. Acho que tem até uma conta teste aqui, ó, galera. Essa aqui é uma conta que eu tenho no Stripe de faço os testes aqui dos projetos da hora de codar, né?

**10:41** · E o dashbo Stripe é assim. Então, vamos ver se fica semelhante, né? Então, vou esperar ele criar aqui e já mostro para vocês. Então, olha só, galera, ele me entregou aqui, tá? Vamos ver como é que ficou o projeto. Então, olha só, esse aqui ficou bem legal também. Gostei bastante do resultado, tá? E a gente poderia fazer um outro teste, né, sem, mas aqui eu vou deixar por conta de vocês, tá?

**11:05** · Claro, ele usou umas cores a mais e tal, mas talvez aqui se tivesse mais preenchido o dashboard do meu stripe, ele também teria outras cores, tá? Mas eu gostei bastante do resultado.

**11:16** · E é assim que a gente usa o repositório ali do Awesome, deixa eu ver aqui.

### My thoughts on Awesome Design MD

**11:23** · Awesome design MD, né? O cara tá atualizando bastante. Achei um trabalho bem bacana. Serve bastante pra gente tirar ali designs bonitos de aplicações que a gente não teria nenhuma ideia de design. Tá bom? Espero que vocês tenham curtido. Eh, deixa aí nos comentários se você usaram, se estão pensando em utilizar, quais foram as experiências de vocês. Também o like. E a inscrição é muito importante, é claro, fico esperando vocês também na formação VB Code. Se vocês querem dominar aí Cloud Code, Antigaravity e outros, lá é o lugar certo. Lembrando, site vitalício, tá? Também grupo VIP no WhatsApp.

**11:54** · Bom, galera, por hoje é isso. Vou ficando por aqui e espero vocês no próximo vídeo.