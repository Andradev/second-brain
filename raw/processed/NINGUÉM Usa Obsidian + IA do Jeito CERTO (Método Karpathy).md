---
title: "NINGUÉM Usa Obsidian + IA do Jeito CERTO (Método Karpathy)"
source: "https://www.youtube.com/watch?v=6Ok9f7J9j3c"
author:
  - "[[Matheus Battisti - Hora de Codar]]"
published: 2026-04-30
created: 2026-05-10
description: "Você organiza seu Obsidian, escreve suas notas, tenta fazer o Claude Code ler tudo isso e mesmo assim a IA não entrega o que você esperava. A sensação é semp..."
tags:
  - "WebClip"
---
![](https://www.youtube.com/watch?v=6Ok9f7J9j3c)

## Transcript

### New way to use Obsidian + AI (LLM Wiki, Karpathy Method)

**0:00** · Galera, Andre Capart ataca novamente.

**0:03** · Antes ele criou um processo de automelhoria de skills, a gente cobriu aqui no canal. Agora ele trouxe uma forma nova de integrar o cloud code com Obsidian pra gente ter o que ele chama de llak, ou seja, uma base de conhecimento nossa, que a Ia pode interagir e a gente fica alimentando ela infinitamente e ela também vai ser autoorganizada ali pelo cloud code.

**0:27** · Isso faz com que a gente tenha um enorme banco de dados com os dados que nos interessam e a gente possa resgatar as informações quando nós precisarmos. É muito interessante, é bem inteligente esse método e eu vou mostrar para vocês exatamente como ele funciona e como vocês podem configurar aí também. Desde o nosso último vídeo obsidian aqui, eu tenho explorado bastante a ferramenta e buscado novidades para trazer para vocês também.

**0:58** · E essa é uma delas e é bem excelente. Para quem não me conhece, sou Mateus Batista, programador há mais 10 anos e venho hoje me aventurando aqui no mundo da trazendo só o que tem de melhor para vocês. Se curtiu o vídeo, deixa aqui um like e também se inscreva no canal para receber vídeos todo santo dia sobre inteligência artificial. Beleza, galera? Então bora, deixa enrolação e vamos lá entender melhor como é que funciona esse método. Então como é que funciona, galera? Esse método que ele desenvolveu foi baseado num guist.

**1:24** · Para quem não sabe o que é GIST, são pequenos arquivos que as pessoas colocam no GitHub geralmente com a solução de algum problema. E ele criou esse guist com o passo a passo de como configurar o cloud code com Obsidian para ele funcionar como essa LLM wick, tá? Então a gente já vai ver como é esse guist e basicamente o que a gente precisa fazer é colocar o guist no cloud, né, o conteúdo dele e pedir pro cloud configurar o obsidian pra gente. Aí depois disso, a gente vai extrair conteúdos e artigos que não nos interessam, né?

### How the Karpathy Method of LLM Wiki works (Claude Code + Obsidian)

**1:54** · Não precisa ser só isso, pode ser outros documentos que tu tenha, pode ser uma transcrição de um vídeo, mas ele tem que tá em markdown, né, pro Obzin ali entender. E para isso a gente tem uma ferramenta excelente que é o web clipper, que eu já vou mostrar para vocês, que vai fazer esse papel de transformar um artigo, um site, né, em um MD e jogar direto no Obsidian para poupar muito o nosso tempo de transformar um texto em MarkD.

**2:17** · Depois o cloud, ele vai ler o que tá em RAW, que são os artigos que a gente colocou lá, né? seria o conteúdo crew e vai colocar ali em weekdato que o capt definiu. Depois, quando ele tá processado, né, ele saiu do Row, ele virou o conteúdo puro, digamos assim, nós podemos acessar ali via carry o o banco de dados que tá no obsidian, fazer as perguntas, tirar as nossas dúvidas e isso vai se e retroalimentando, né?

**2:50** · Porque a gente vai colocando mais conteúdo novo, ele vai compilando e a gente vai usando o cloud. Ele aprende nesse processo, os nossos dados ficam mais refinados e a gente tem ali praticamente uma wik do que a gente quiser e com LLM como motor, né, e o Obsidian como banco de dados, vamos dizer assim. E tudo funciona muito bem, sem estrutura muito complexa, né? Bom, quais são os diferenciais? 100% markdown local, né? Então, um arquivo simples que as IAS conseguem entender muito fácil.

**3:21** · Ele cresce de forma inteligente porque ele vai condensando o conhecimento que a gente coloca em Row no obsidian, né, no nosso VT. Não precisa de banco de dados, né, nem uma um rag, né, um banco de dados vetorizado, não precisa de uma infraestrutura, não precisa de servidor.

**3:35** · A LLM vai escrever tudo. A gente só vai precisar fazer a curadoria. portável, tu consegue colocar no Git ou em qualquer lugar para as outras pessoas acessarem ou tu mesmo ter ali ele salvo na nuvem e consegue criar um graph view diretamente no obsidian, né? Porque com a base do conhecimento as coisas vão se construindo lá de uma maneira que fica visualizável, vamos dizer assim, tá bom?

**3:57** · A gente vai fazer esse setup aqui. Só antes, não se esqueça, galera, a gente tem um vídeo aqui da configuração do cloud code com obsidian, mas utilizando o método que é bem interessante também.

**4:07** · O editor vai deixar aqui a tamb, eu vou deixar o izinho. Galera gostou muito desse vídeo, eu recomendo que tu assista porque é uma outra estratégia que é interessante também com Obsidian Cloud Code, tá bom? Vamos lá. Llak é esse cara aqui. Eu vou deixar o link aqui do Gist no na descrição, tá? Para vocês acessarem. E a gente vai precisar copiar esse conteúdo e pedir pro cloud fazer a configuração. Então a gente pode vir aqui no RAW, ó acessar esse conteúdo e dar um contrtrl C e colar lá no cloud, tá? Vai ter que ter o Obsían instalado, é óbvio, né?

### How to configure the LLM Wiki in Claude Code

**4:38** · Então basta baixar, não tem mistério, é só o next next da vida. Tu vai instalar ele e tu vai precisar criar um VT. Eu já criei aqui um, é só tu iniciar ele que já vai pedir para tu criar esse cofre, né? O chamado VT. Tu vai ter aqui, aqui são os meus dois que eu tô trabalhando para tutoriais, né? E aqui ele dá a mensagem que o teu vai est também, tá? Criar o novo crofre. Aí tu vai criar numa pasta que tu queira e beleza. Aí quando tu cria esse cofre, tu vai ter que abrir o cloud code nele, beleza? Então, eu abri aqui o cloud na pasta que tá o VT.

**5:08** · E aqui agora a estratégia é a seguinte, pedir pro próprio cloud fazer a configuração do VT seguindo que o Carpate ali escreveu no método. Beleza? Então eu vou copiar isso aqui, dar um control A, conttrl C. Te volta aqui pro cloud code, botão direito para colar. Aí aqui, ó, tu pode colocar eh do lado de todo o promptim. configura isso. Para mim, o tema é conteúdos sobre IA, né?

**5:40** · Então, mais generalista é esse VAL que eu vou criar aqui junto com vocês, beleza? Aí, pedindo isso, colocando o que tá no guist, ele vai configurar o VT baseado em como Capou ali, né? E a ideia, deixa eu voltar aqui, acho que eu tenho até estruturinha de pastas aqui. Deixa eu ver aqui, ó. A ideia, esse cara comentou, mas é bem semelhante, tá? Então ele vai ter a wick, que é onde a gente vai extrair as informações, e o RAW é onde vai ter as fontes de informação.

**6:09** · Então basicamente tu vai colocar tudo em RAW e aí o Cloud Code vai transformar isso em conteúdo pesquisável, né? Bom, enquanto ele cria lá, galera, tem que dar as confirmações aqui que eu falei para vocês também é importante. A gente vai precisar do clipper para poder transferir os arquivos em MD mais fácil. Beleza? Já vou mostrar para vocês.

**6:32** · Só não se esqueçam, galera, se tu quer dominar Cloud Code, aprender Vibe Code a fundo, do básico avançado, nós estamos com as inscrições abertas da formação Vibe Code. O link vai est aqui no comentário fixado. É um treinamento completo com acesso vitalício para tu aprender tudo sobre programação assistida por IA com diversas ferramentas, Codex, Cloud Code, Open Code, Antigaraft. Tem mais de 35 horas de treinamento, tá? Tô atualizando semanalmente. E aqui tu pode conhecer todos os detalhes do curso. Nesse vídeo aqui também eu explico tudo passo a passo.

**7:03** · Então dá uma olhada aí que vai valer a pena se tu se interessa por cloud code, tá bom? Bom, o clipper, deixa eu ver aqui, ó, é essa extensão aqui, né? O site é igual do obsidian.

### Converting pages to md with Obsidian Web Clipper

**7:15** · Então tu vai, é porque é do obsidiano, né? Tu vai acessar aqui obsidian.

**7:20** · MDMD/Clipper.

**7:22** · E aí é uma extensão de Chrome, né, do Google Chrome, que tu vai adicionar e aí vai ficar o iconezinho do Obsidian aqui.

**7:28** · Como é que ela funciona? Então, tem os artigos de várias IAS abertos aqui, tá?

**7:34** · E aí basta a gente clicar aqui que ele vai transformar esse HTML num MD. Só deixa eu ver se ele terminou aqui, ó.

**7:41** · Ele terminou, tá? Então a gente pode ver a estrutura de pastas, ó. Fica assim, ó.

**7:47** · Row, que é onde a gente vai colocar as coisas, e o Wick, que é onde vai ficar as informações. Então, vamos lá, vamos pegar todos esses artigos aqui. Eu separei do GLM, do Minimex, do Química 2.5, que a gente tem vídeos aqui no canal do Cloud Opus 4.6, saiu faz um tempo, né? São mais novos. E vamos colocar ele na nossa eles, né, na nossa base de conhecimento. Aí aqui, galera, a gente pode clicar na extensão e adicionar ao obsidian. Que que ele vai fazer? ele vai adicionar ao nosso obsidian aberto, né? Esse é o comportamento de F.

**8:17** · Se não ir, tu pode simplesmente colocar aqui guardar ficheiro, tá? E isso vai fazer com que ele baixe o MD. Aí tu pode colocar lá tu mesmo, tá? Então vou fazer isso em todos, só para mostrar para vocês o processo, né? Mais manual do que do que o automático. Então veja como é bem rápido, né? Essa extensão, ela acaba facilitando um pouco o processo, né?

**8:37** · Deixando mais tranquilo pra gente. Então a gente vai abrir o obsidian. Então tu abre a pasta do teu obsidian, né, do teu Volt, e tu vai colocar todos os artigos dentro de RAW, tá bom? Aí quando tiver a base de conhecimento que tu quer, claro que tu não vai fazer isso de uma vez, né? Talvez a primeira vez sim, mas depois vai ser um ou outro artigo, né?

**8:58** · Tu vai colocando a medida que tu quer que avance na tua base de conhecimento.

**9:02** · Nós vamos dizer que chegou num ponto, OK? Ou tu adicionou alguma coisa nova, vai ter que colocar o seguinte: prompt compila o RAW pro wik seguindo o esquema. Então isso vai fazer com que ele pegue o conteúdo cru, né? O conteúdo sem nenhum filtro, sem nenhuma padronização e transforme ele no wick da maneira que o Gist pede. E aí a gente teria o conteúdo acessível via cloud code que está lá no Obsidian. Então veja aqui, ó, ele identificou quatro fontes, que foi exatamente o que a gente fez, né, que a gente pegou.

### Creating the LLM Wiki based on added knowledge

**9:29** · Ele vai criar as páginas em fontes, modelos, entidades e conceitos e vai atualizar também os arquivos MD, que são arquivos gerais do nosso repositório, vamos dizer assim.

**9:41** · Tem que dar as permissões, tá? E esse vai ser sempre o processo, né? Como eu coloquei lá no Sky Draw, é um loop.

**9:47** · Depois a gente vai usando e adicionando novas fontes, tendo novos conhecimentos para que a gente possa ter sempre uma base atualizada com as melhores informações. Então, olha só, galera, ele indexou todas as fontes e agora ele tá no processo de criação da Wik. A gente pode até acompanhar em tempo real aqui o que tá acontecendo, né? Ó, ele já colocou as fontes, ele já colocou alguma coisa em modelos, visão geral. Então, tá ficando bem bacana, né? a gente vai ter informações em texto. A gente pode consultar dessa maneira aqui, né? Ou seja, usar o obsidian como ele foi criado para ser utilizado.

**10:19** · Mas é muito melhor a gente ter uma LLM plugada nele, né? porque daí a gente consegue tá indo mais direto ao ponto. Eu acredito que a LLM é um filtro que vai nos economizar muito tempo nesse processo aqui. E outra coisa legal, né, a visão de gráfico que vai fazendo também, porque algumas IAS,

**10:39** · né, elas vão tendo pontos em comum, por exemplo, vão dizer que mais de uma tenha esse agent swarm, então a gente consegue entender, fazer essas comparações para poder decidir qual IA que a gente vai utilizar no nosso dia a dia baseado na quantidade de recursos, né, qual que traz mais benefícios pra gente e até ter uma comparação mais justa do que um benchmark que a gente não sabe como é que ele foi feito, né? Porque aqui a gente tá colocando dados e eles estão sendo postos à prova, né? Uma LLM contra outra, vamos dizer assim. Acompanhar o projeto aqui, ó.

**11:09** · Cloud Code quase terminando. Inclusive, galera, a gente tem aqui uma playlist cloud code também.

**11:14** · Vou deixar o editor vai deixar a TAM aqui do primeiro vídeo. É um curso de cloud code para tu aprender a utilizar a ferramenta. Eu vou deixar o izinho aqui para que vocês possam acessar essa playlist. Tem mais de 50 vídeos. O deve est chegando aí no nosão, bastante conhecimento de qualidade gratuitamente para vocês, né? E daí se tu quiser se aprofundar mais, tem a formação Vibecode. Então vou esperar ele terminar aqui, depois vou mostrar para vocês o resultado final e como que a gente vai extrair informações daqui, né? Ó, galera, então ele termina e ele me dá aqui uma visão geral, né, do que foi feito.

**11:44** · Então, um desses quatro artigos que a gente mandou, ele criou 19 páginas na nossa wik, tá? Então aqui é a visão de gráfico completa, né, que a gente vai ter o nosso sisteminha que a gente criou. Aí ele criou, por exemplo, uma área para agente hardness, agente, que são conceitos importantes, né? Cada modelo pode ter o seu, né? Aí ele criou as entidades, são as empresas por trás das IA, as fontes, né? Então ele deu uma melhorada nos artigos de fonte.

**12:11** · E aqui a gente continuaria ou olhando ali via artigos, né? Ou fazendo prompts aqui, por exemplo. Ah, olha meu IK, me diz o que eu sei sobre Kim K2.5, né? que foi um dos modelos que a gente colocou ali, ele vai pesquisar e vai nos dar a resposta. A gente podia fazer até uma interface gráfica para acessar o nosso obsidian, né? Não precisa depender do terminal.

### Seeking knowledge in the LLM Wiki

**12:33** · Eu posso também não só tá pedindo por coisas, né, de um modelo específico, eu posso buscar conexões entre as informações que eu coloquei aqui também. Eu vou mostrar para vocês como a gente pode fazer isso, ó. Então ele me traz aqui dessa forma, né? A identidade que K2.5 single flagship da Moonshot AI, que é a empresa, né, apresentado como modelo open source, mas poderoso até a data e tudo mais, tudo mais. Aí se eu quisesse uma conexão entre várias fontes, olha o wik, me mostra três conexões interessantes entre conceitos que eu não percebi.

**13:04** · Então aqui ele vai juntar formações de várias fontes e aí ele vai me trazer o resultado. Outra coisa que eu posso usar também, meu caso aqui, né, a gente pode ter usais, né, pro pro para esse LLM wick, é, por exemplo, produção de conteúdo baseado no que eu encontrei aqui, que é interessante, porque não depende de ficar olhando milhares sites, eu vou juntando conteúdo e ele pode me dar ideias futuras para eu produzir conteúdos.

**13:32** · Deixa de me responder que eu vou mostrar para vocês como que a gente pode fazer nesse sentido também, né? Ó, ele mostrou aqui, então, três nomes para o mesmo modo de falha. Então, serial collapse, orquestrador regrid para single agent com com mesmo capacidade paralela platô precoce, modelo aplica técnicas familiares, estagna. Então, outra coisa aqui, context compaction e subagent freezing são a mesma ideia, né?

**13:58** · Então, são nomes iguais para mesma coisa, né? Todos estão comizando o harness, não o modelo, né? Tá muito em alta, o agentness. E aqui a gente juntou, por exemplo, informações de quatro fontes diferentes para trazer ideias, né, que se são semelhantes. E aqui, por exemplo, a baseado no meu wick me sugere três ideias de blog posts sobre a pra próxima semana. Então, tô gerando conteúdo baseado no conhecimento que tá condensado ali na minha wik.

**14:22** · Bom, galera, daí ele veio aqui e me sugeriu as três ideias, né? modo de falha que ninguém nomeou direito, o dia em que Harness commodity, esqueça melhor o segredo arquitetural dos agentes de longa duração. Bom, e assim a gente tem uma base de conhecimento utilizando, né, o Obsidian e o cloud Code dessa maneira CarP, né, que ele desenvolveu para poder agregar muito conhecimento de fontes raw, né, cruas e depois compilar com o

### My thoughts on the Karpathy LLM Wiki Method

**14:51** · cloud code para que fique mais assertivo e extrair as informações e ficar fazendo isso em loop até que ele tenha bases de conhecimentos muito confiáveis e interessantes pro para qualquer tipo de uso, né? Aí tu vai definir dependendo do que tu precisa. Galera, comentem o que acharam, se tão utilizando o Cloud Code com Obsidian. Eu tô curtindo, tô usando bastante, tô testando várias coisas e pretendo trazer mais conteúdos aqui pro canal.

**15:15** · Se curtiram a ideia, curtiram o vídeo, não se esqueçam, deixem o like, também se inscrevam, isso é muito importante e ajuda bastante a continuar o nosso trabalho aqui de postar vídeos todos os dias. Dá uma olhadinha também na formação VB code. E por hoje é isso.

**15:28** · Vou ficando por aqui. Espero você no próximo vídeo.