---
title: "Crie um Agente de IA no WhatsApp com CRM (Guia Completo n8n + Antigravity)"
source: "https://www.youtube.com/watch?v=Jvq47ed-fm4"
author:
  - "[[Felipe Borges - Fala IA!]]"
published: 2026-03-09
created: 2026-05-10
description: "Descubra como criar um Agente de IA no WhatsApp com CRM completo usando n8n e Google Antigravity. Copie essa automação do zero e venda para seus clientes! 🤖..."
tags:
  - "WebClip"
---
![](https://www.youtube.com/watch?v=Jvq47ed-fm4)

## Transcript

**0:00** · Nesse vídeo eu vou te mostrar o passo a passo de como criar um agente de A perfeito para WhatsApp com CRM visual construído do zero usando o Google e N8N. O que você vai aprender hoje vai valorizar os seus projetos em pelo menos 10 vezes e o melhor apenas seguindo o que eu vou te mostrar aqui sem nenhuma complicação. Isso porque um bote bonitinho ali vale algum dinheiro, mas um agente de a inteligente integrado a um CRM de verdade vale muito mais. E é isso que vai transformar um projetinho barato e um projeto de grande valor.

**0:28** · Nesse vídeo nós vamos falar sobre como conectar a API do WhatsApp, configurar os web hooks, criar o nosso banco de dados no Subabase e usar o Google Antigravery para gerenciar tudo isso e criar um CRM completo de forma super simples, apenas escrevendo promis. E fica comigo até o final, porque além de montar toda essa estrutura, eu vou liberar esse agente pronto junto com todo o material da aula para você simplesmente baixar, copiar e usar nos seus projetos para já vender pros seus clientes. Meu nome é Felipe Borges, eu vivo exclusivamente Automações Ia e se o seu sonho é viver disso também já se inscreve aqui no canal porque toda semana tem vídeo prático para te ajudar nessa jornada.

**0:59** · Antes da gente ir para mão na massa, vamos só entender rapidinho o que que nós vamos fazer aqui. Então nós vamos criar um agente de inteligência artificial conectado ao WhatsApp. Então ele vai receber as mensagens e vai responder esses leads lá no WhatsApp. Nós também vamos criar um CRM, ou seja, um sistema, um painel onde você, os seus clientes, vão conseguir acompanhar as mensagens que o agente tá mandando para os leads.

**1:19** · Isso porque muitas vezes quando a gente vende um agente de inteligência artificial, o cliente não consegue ter acesso a essas conversas, por ele precisaria logar no WhatsApp do agente e ficar acompanhando as conversas. Às vezes a gente tem dois, três, quatro sócios e os quatro querem ter acesso. A gente também precisa ter acesso como desenvolvedor desse agente.

**1:36** · Então ficaria muita gente logando no mesmo WhatsApp. Primeiro que não dá e segundo que se você tivesse vários clientes também, você não ia conseguir acompanhar isso. Você ia logar várias contas no seu computador, ficaria muito complicado essa operação. Então a gente vai criar um sistema mostrando ali um CRM com todas as conversas que a gente tá tendo no WhatsApp. E isso com certeza vai elevar muito valor dos seus projetos. Outra observação importante é que tudo que eu mostrar aqui vai tá disponível com material aqui embaixo da aula na descrição. Então você clica no link, faz o download de todo material que vai est lá na nossa comunidade, na aba desse vídeo específico e você já vai ter acesso a tudo que eu tô mostrando aqui. Beleza?

**2:08** · Agora sim podemos seguir pra nossa primeira etapa. E o primeiro passo vai ser justamente você baixar este agente aqui que tá aparecendo na sua tela. É um agente completo, ele é um agente mais simples de atendimento, né?

**2:18** · Dá pra gente colocar muito mais função nele, mas é um agente completinho aqui que vai fazer bem a nossa função para esse vídeo. E é claro que esse agente aqui que eu tô te mostrando agora é um agente, como eu disse, completo, mas um agente simples. E se você quer agregar mais valor para os seus projetos, é importante que você tenha também um agente robusto, um agente mais robusto, como esse aqui que tá aparecendo na sua tela, que é o meu super agente humanizado. é um agente muito mais completo, é um agente que entende áudio, texto, imagem, é um agente que entende mensagem picada totalmente completo e o agente que eu vendo para os meus clientes é exatamente esse.

**2:49** · E esse agente é responsável pela maior parte do meu faturamento. E se você quiser ter acesso a esse mesmo agente, mais todas as minhas estratégias de venda e captação, tudo isso em um só lugar, você pode acessar o QR code que tá aparecendo aqui na tela, que é o meu curso AI1, em que o único objetivo desse curso é fazer com que você fature seus primeiros R$ 3.000 R nos próximos 14 dias, usando os meus próprios agentes que eu vento paraos meus clientes e todas as minhas estratégias.

**3:14** · Então lá você vai ter acesso a esse agente que eu vou disponibilizar para você toda a configuração dele e você vai poder inclusive colocar ele funcionando junto com esse CRM que a gente vai ver aqui nessa aula para agregar ainda mais valor. Clica no QCode, dá uma olhada, porque o preço desse curso é absolutamente ridículo. Clica lá só para ver e depois você me diz se é ou não é um curso que realmente vale a pena.

**3:35** · Então agora voltando aqui para a nossa aula, nós temos aqui o web Hook já conectado no agente. Ele vai fazer a conexão do WhatsApp via Zapi e com isso ele vai receber as mensagens do WhatsApp, vai processar e vai enviar através desse outro node aqui, HTTP request, que é uma requisição que a gente tá fazendo para ZPI enviar a mensagem que o agente responder para o WhatsApp da pessoa que entrou em contato. E aí o resto do fluxo é basicamente critérios de ativação, que são alguns filtros que a gente vai colocar para que o agente seja ativado ou não.

**4:04** · Por exemplo, se você conectou um agente do WhatsApp e você tem um grupo e esse grupo fica mandando mensagem, você não quer que o agente seja ativado toda vez que o grupo manda mensagem, ele começaria a responder o grupo, daria o maior problema. Então aqui a gente tem alguns filtros que proíbem, né, o agente de ligar, de continuar o fluxo se ele não respeitar esses parâmetros aqui.

**4:21** · Depois a gente tem informações do lead.

**4:23** · Aqui a gente vai fazer um compilado do lead, né, do dados do lead para ficar mais fácil, né, da gente tratar esses dados mais pra frente. Aqui a gente vai extrair só o texto da mensagem. E aqui nessa parte nós vamos criar um lead lá no nosso banco de dados do Supase. Então a gente vai ter uma tabela no Supas que entrar em contato vai ser registrado lá com nome, telefone, todas as informações. Depois essa informação vai passar aqui pro nosso agente de inteligência artificial que já vai estar com esse prompt completaço. Depois você só adapta o que você quiser ou precisar aqui e eu a pessoa vai mandar a mensagem.

**4:53** · O agente com base nesse system message aqui, nesse prompt a nível do sistema, vai responder o cliente. Para fazer isso, eu tô usando a API da Open AI, mas você pode usar Gemini, Grock, o que você preferir, pode usar aqui, tranquilo, não tem problema. Vai funcionar do mesmo jeito. Você só coloca, claro, a sua API e os nossos dados vão ficar armazenados em um banco de dados no PostG, que a gente vai usar o Supas para isso também. Por fim, como eu já falei, ele vai passar por aqui, vai disparar a mensagem resposta do agente para o telefone do lead.

**5:21** · Por fim, também eu coloquei esse node para não fazer nada, para representar o fim do fluxo. Então, vai lá, baixa esse arquivo agora no seu computador e coloca ele para funcionar no N8N. Você vai ter duas formas de fazer isso. Você vai poder vir aqui depois que você fizer o download dele, import from file, importar de um arquivo. Aí você vai clicar aqui, vai acessar a pasta onde você fez o download, vai clicar e o agente vai aparecer na sua tela. Ou você pode simplesmente copiar o conteúdo que tiver dentro desse arquivo, vai ser um código em Jon, o código desse agente.

**5:50** · Você pode copiar, vi aqui numa tela do N8N vazia e dar contrtrl C. O agente também aparece na sua tela. Fica à vontade para escolher a melhor forma. Dito isso, estamos aqui então com o nosso agente já importado no N8N. Que que nós precisamos fazer agora? A primeira coisa é conectar com a ZAPI. Eu vou ensinar como você vai fazer a credencial, caso você ainda não conheça a ferramenta. Então, nós temos esse web hook aqui. Ele não precisa aqui especificamente da Zapi, mas a gente já vai começar a nossa configuração aqui.

**6:19** · Por quê? Porque esse link aqui é o link de ativação que a gente precisa colocar lá na nossa Zapii. Então, abrindo a Zapi aqui, nós vamos ter depois que você criar sua conta e pode, de novo ser uma conta gratuita, nós vamos cair nessa tela. A primeira coisa que você vai fazer não é conectar a API, nós vamos vir aqui em instâncias web.

**6:37** · Aqui vai ter todas as suas conexões.

**6:39** · Provavelmente você não vai ter nenhuma conexão, então você vai vir aqui em adicionar. Quando vier em adicionar vai abrir essa tela aqui, uma tela parecida com essa aqui do lado. Vai provavelmente ter um QR code. Você vai conectar o seu WhatsApp aqui e aí já vai aparecer conectado, igual tá aparecendo aqui para mim. Sua instância já está conectada.

**6:55** · Você pode enviar mensagens via API. A gente vai fazer isso por enquanto.

**6:59** · Agora, nessa mesma tela, você vai ver que nós temos dados de instância web, que você pode colocar o nome da sua instância. Eu coloquei teste conta. E aqui nós temos a API da instância. Isso aqui a gente vai precisar para colocar lá no http request. Então segura um pouco. A princípio, lá no começo do fluxo, a gente tem o quê? Web hook.

**7:15** · Então é aqui que a gente quer chegar primeiro. Tá vendo esse link aqui que tá escrito ao receber? É basicamente o gatilho que você vai colocar aqui. Ou seja, você precisa colocar aqui um link e através desse link ou a Zapi vai ficar escutando o N8N. Então, sempre que chegar uma mensagem, aquele web hook que tá no N8N, através desse link aqui, vai mandar uma mensagem para a Zapi dizendo: "Olha, chegou uma mensagem". Então, a gente precisa que esse mesmo link seja exatamente o link que tá aqui. Esse link para você pode estar aparecendo de outras formas escrito.

**7:45** · Tá vendo esse path aqui de caminho? Se você apagar, olha só o que acontece, ele apaga aqui em cima também. Se a gente coloca mensagem, ele adiciona nesse link mensagem também. Pra gente fazer, a gente vai continuar utilizando a URL de teste. E pra gente identificar e depois não confundir quando a gente colocar esse projeto em produção, eu vou colocar mensagem nesse caminho, senão fica uns números, ó, tá vendo? Fica um número muito ruim de decorar isso aqui. Isso aqui para dar erro é muito fácil. Então vou escrever mensagem, traço, teste, porque eu sei que eu tô fazendo um web hook lá na ZPI para receber a mensagem e que é em um RL de teste.

**8:16** · Depois quando mudar pra produção, a gente simplesmente apaga o teste. Mas isso é outro papo para não não para agora. Feito isso, eu vou copiar esse link aqui. A gente pode só clicar em cima. A gente vai voltar lá na Zapi e agora nós vamosou apagar esse link que tava aqui e colar a nossa URL lá do NN. Feito isso, se não tiver selecionado aqui para você, você pode selecionar, notificar as as mensagens enviadas por mim também, porque assim você vai conseguir testar o seu web hook para ver se ele tá funcionando. Então você consegue mandar mensagem para você mesmo. Se isso aqui tiver desativado e você manda mensagem para você mesmo, ele não vai receber lá no web hook.

**8:48** · Aconselho até que você faça isso com dois celulares, porque a experiência fica melhor para você ir entendendo, mas não tem problema se você só tiver um celular e precisar ficar mandando mensagem para você mesmo, só deixa isso aqui ativado. Depois a gente vai vir em salvar. Essa é a primeira etapa que a gente vai fazer aqui na nossa Zapi.

**9:04** · Agora a gente precisa conectar a API porque vamos lembrar para o agente conseguir enviar a mensagem pro lead, ele vai utilizar esse node aqui de HTTP request. E veja que esse node ele exige uma autenticação header que eu tenho aqui já a minha credencial criada nova ZP e LGP. Isso daqui é a minha credencial, mas eu vou te mostrar como você pode criar a sua. Você pode vir ou aqui nesse node em create new credential ou você pode vir aqui sair do seu fluxo.

**9:30** · Lembra sempre que quando for sair do fluxo dá um contrl s aí para salvar tudo que você fez. Vim aqui em cima e create credential. Você pode fazer as duas formas. Eu vou fazer da forma mais prática, que é justamente aqui no fluxo.

**9:40** · A gente vem no HTTP request e aqui mesmo viemos em create new credentio. Aqui você tem pouquíssimos dados para preencher. Esse primeiro você vai preencher com client traço token. É isso que você vai colocar aqui. Agora essa parte do velho que é o valor, você vai ter que pegar a sua chave API lá na ZPI.

**9:59** · Vou te mostrar como fazer isso. Então aqui de volta na nossa ZPI, a gente vai vir em segurança e aqui, ó, vai ter token de segurança da conta. Eu não vou gerar um outro token porque senão eu vou perder a credencial que eu tenho lá, porque eu vou ter que atualizar o token.

**10:10** · Mas o seu código que você vai precisar para colocar lá naquele campo velho que tá na nossa credencial no N8N é isso daqui. Você vai colar esse client token.

**10:19** · Tá vendo? A gente escreveu client token ali, porque é justamente isso que a gente tá passando para ele. E você vai colar esse código aqui, exatamente aqui.

**10:24** · Feito isso, você vai dar save e pronto.

**10:26** · Vai tá certinho para você já conseguir estar conectado no N8N com a Zapi. Eu vou colocar para cancelar e vou selecionar de novo a minha credencial. E tá certinho aqui pra gente usar. A única coisa que eu preciso que você fique atento é isso daqui, a URL. Por quê?

**10:41** · Aqui é uma URL única e exclusiva sua para mandar requisição lá pra ZI. Então aqui a gente vai fazer uma última mudança, a última mesmo quando a gente fala de ZI, que é apagar essa URL que tá aqui. Então a gente vai selecionar ela e apagar. Por quê? Porque aqui no nosso Zapi a gente precisa passar a requisição, o link que tá na nossa instância web. Então, a gente vai voltar a instância web, vai clicar aqui. Esse API da instância é o que a gente precisa passar.

**11:10** · E esse API, essa API da instância, ela é diferente de conta para conta. Então aqui você vai ter um código, um token referenciando a sua própria conta. Não passe isso para ninguém, claro, porque senão todo mundo vai conseguir disparar mensagens usando seu token, mas você vai precisar individualmente vir aqui, copiar a PI da instância e aí sim colar lá no nosso N8N. a gente vem aqui URL e cola.

**11:33** · Pronto. Feito isso, você já configurou as suas epi, certinho? Ela já tá funcionando, mas o agente ainda precisa algumas outras configurações. As próximas configurações e praticamente as últimas é no banco de dados do Supase.

**11:45** · Então a gente precisa ir lá para conectar a nossa credencial. E nesse caso, eu vou criar uma credencial nova para mim também, para usar um super base que eu ainda não usei. Então a gente tem aqui o credential to connect with, ou seja, credencial que eu quero me conectar. Vou vir em criar uma nova credencial. E veja que aqui eu preciso passar dois dados para ele, o host e o Service Row Secret. Vamos abrir o Supase agora e ver onde é que a gente encontra isso. Lá, aqui estamos dentro do Supas, dentro de um projeto. Você já provavelmente já tem o login no seu base. E a gente vai vir aqui nesse cantinho esquerdo, projectiew, vi em project settings.

**12:16** · Aqui dentro vai abrir um outro menu onde nós temos API Keys. E nós vamos vir aqui em legacy service row API Keys. Clicando aqui, nós vamos ter a nossa URL, que é a nossa chave API, que a gente também não pode mostrar para ninguém, até por isso tá aparecendo embaçado aí para você. A gente vai ver aqui em review, copy. A gente vai copiar isso e vamos colocar lá no nosso N8N aonde Service Row Secret, justamente aqui. Agora tá faltando a gente colocar o host, qual que é a nossa URL ali que a gente tem com o Supase.

**12:47** · Então vamos voltar lá. E para achar essa URL, tem uma maneira muito simples da gente vir aqui, ó, e escrever URL. E vai aparecer já em actions, copy API URL. A gente simplesmente clica aqui, volta no N8N e já conecta. Feito isso, a gente vai dar em save. Ele falou que a credencial foi criada com sucesso. Ela apareceu verdinho. Estamos já conectados no nosso superabase. Ainda não acabou porque a gente precisa criar duas tabelas simples no base. Uma delas é a de lead. Olhando aqui no fluxo, você já vai lembrar dela.

**13:18** · É a que vai criar os dados do lead, o nome, o telefone lá numa tabela para você ter essas informações, caso você precise e até mesmo pra gente usar depois no CRM. Então a gente precisa criar essa tabela. De volta aqui no Superabase, a gente vem aqui em table editor e a gente vai criar a nossa tabela. Atenção ao nome que eu vou criar aqui. Crie exatamente como eu tô fazendo, justamente para você não ter problemas na hora de criar o CRM lá com antigravery, que a gente vai fazer daqui a pouco. Então, a planilha, ela vai chamar leads, se escreve la, deixa eu até me mudar aqui de cima e colocar minha câmera aqui embaixo. Leads.

**13:48** · L E A D S. Leads. E aí nós precisamos colocar as colunas. A primeira coluna vai ser o ID. E o ID eu quero que ele preencha automaticamente. Essa configuração para ele preencher o ID automaticamente já tá aqui. A gente não precisa mexer nada. A segunda coluna que eu quero é created at, ou seja, em que momento que esse lead foi criado, em qual horário. Eu também quero saber o dia e o horário que esse cliente entrou na nossa base também já tá aqui como padrão. E ele tá usando o time stamp como referência now.

**14:14** · Então, se o cliente entrar agora na minha tabela, vai aparecer aqui para eu já saber que esse cliente veio nesse determinado horário, nesse determinado momento. Portanto, as duas únicas colunas que vai criar, na verdade, são a lead nome. A gente vai colocar como texto, claro, porque o nome é um texto.

**14:31** · Prontinho. Ele vai vir como nul, ele vai vir nulo, né? Essa coluna, essa linha, cada linha vai vir nula, porque quem vai preencher, na verdade, vai ser o nosso agente. Lembra do fluxo? Ele cria os dados do cliente do lead aqui no subase.

**14:41** · Por isso que essa coluna precisa est exatamente com esse nome para funcionar.

**14:45** · Então ela vem vazia, porque quem vai preencher isso é ali o próprio fluxo.

**14:48** · Depois a gente precisa criar uma outra coluna que chama lead\_line ID. E aí você vai falar: "Pô, mas já tem uma coluna de D. Esse D ele vai começar do número um.

**14:57** · 1 2 3 4 é um ID dele que não vai se repetir nem nada. Só que nós vamos criar um outro tipo de ID que também não vai se repetir, claro, que vai ser o telefone do cliente. Então aqui a gente vai colocar inclusive como texto também.

**15:07** · Por quê? Já vou te explicar, pô, mas o telefone é um texto, não é um número.

**15:10** · Quando a gente tá falando de programação, a gente coloca como número tudo aquilo que a gente quer calcular.

**15:14** · Então, se eu quero fazer uma conta, eu vou colocar como número. Se eu não quero fazer uma conta, mas é um número, então 360 é um número, mas eu não quero fazer nenhuma conta, nenhum cálculo com isso, eu coloco ele como texto. Isso facilita muito, tá? um é um uma boa prática da programação. Então, coloca aqui como texto também, até porque vai facilitar muito o nosso trabalho quando a gente for falar lá do nosso CRM. Feito isso, você vai dar salvar. Só uma coisa antes, perceba as quatro colunas que nós temos.

**15:37** · ID, created at, lead nome e lead ID. Por que que eu tô falando isso? Porque lá no nosso N8N, quando a gente vem aqui, ele vai rodar o node de su base para encontrar o cliente. Então esse é o primeiro node que ele vai rodar aqui.

**15:52** · Para isso, ele vai usar a operação get na planilha leads, tá vendo? Com S, ele vai procurar o ID lead edit. E é um string, é um texto. É isso aqui na nossa planilha que ele vai procurar. Nesse caso, a gente precisa conectar, você no caso que acabou de criar uma nova credencial no Supabase, você vai conectar essa nova credencial aqui. No meu caso, supase account 2, já tá selecionado. Então ele sabe que eu tenho só essa planilha de no meu base. E aqui também você vai selecionar as colunas que você tem lá, quais a gente tem.

**16:22** · ID, created, nome do lead e o nosso lead, que é a coluna que a gente vai usar.

**16:30** · Perfeito. Feito isso, ele vai ver se o cliente existe. Se o cliente existir, ele passa paraa frente. Se o cliente não existir, ele vai criar um cliente. Aí ele vai usar a operação create na tabela leads e ele vai colocar, olha só, os nomes das colunas. Ele já tem o nome do lead, que é o dado que ele precisa preencher, e o lead ID. Lembra que ele precisa preencher só esses dois dados?

**16:47** · Porque o ID e o created at ele já preenche automático. Pois é, a gente vai pedir pro próprio fluxo preencher isso de acordo com os dados que ele vai receber lá do web hook que a ZPI vai mandar pra gente. Esse é praticamente o fluxo. Acabou. Quase acabou. Agora a gente vai precisar simplesmente conectar o Postgre. Para isso, a gente vai entrar aqui no nosso Postg. Eu vou criar uma nova credencial. Então a gente vai vir aqui em cred create new credential e a gente precisa passar todos esses dados que tá pedindo aqui. Então para isso, a gente vai lá no nosso Supabase e vamos encontrar onde ficam essas informações.

**17:19** · A gente vem em connect. Dentro de connect a gente vem aqui em, tá vendo que tem direct? a gente vai trocar para transcription poler, a gente vai vir aqui em view parameters, ou seja, pra gente visualizar os parâmetros. E aqui tem as informações que a gente precisa.

**17:31** · Primeira informação é o host. Então eu vou colocar o host aqui. A segunda informação que eu preciso agora é a nossa porta 6543. Vamos voltar lá e colocar aqui embaixo porta e colar o que tava lá. Aproveitando que a gente já tá aqui embaixo, tá vendo esse SSL? A gente precisa vir aqui em ignorar SSL issos.

**17:49** · Então a gente simplesmente já dá um checkzinho aqui. Continuando, a gente precisa então do nosso database. Vamos procurar lá no nosso superabase database é justamente o postgis que já tá inclusive dito lá no nosso N8N. A gente não precisa fazer nada aqui. O user usuário, ele tá como postg, mas aqui sim a gente vai ter que colar outra informação. A gente vem aqui, cola esse usuário, vai lá de volta no N8N e coloca aqui. A última informação que ele vai pedir é o password, a senha. Para isso, a gente volta também lá no Superabase. A gente vai precisar em outro lugar.

**18:19** · Aí aqui a gente vem, tá vendo? Reset your database password. A gente vem aqui em database settings, vai abrir essa tela e a gente vem em reset password. Tá vendo?

**18:29** · Resetar a senha. Pode colocar como reset. Agora a gente vai precisar colocar uma senha no nosso postg database. Aqui a gente poderia digitar uma senha, mas na verdade eu vou vir aqui em gerar uma senha. Ele mesmo já vai gerar para mim. Eu vou copiar. Eu não posso perder isso porque eu preciso colocar ali no N8N. Então, garanta que esteja copiado. Vem em reset password, espera carregar, porque aí ele tá agora trocando realmente essa senha. Agora sim, a gente vai lá no N8N e cola aqui em password. Prontinho. Feito isso, a gente vem em save. Ele deu que a credencial foi criada com sucesso.

**18:59** · E agora, Felipe, eu preciso fazer o quê?

**19:03** · Não precisa fazer mais nada. Você conectou isso daqui, ele já entendeu. A nossa credencial já tá aqui. Deixa eu selecionar ela, que é essa credencial aqui. Quando a gente receber a primeira mensagem, ele vai criar um histórico do nosso chat. Então, tudo que a gente conversou com o lead vai ficar armazenado numa tabela que se chama N8N chat histories.

**19:21** · Feito todas as configurações que a gente já acabou, nós vamos agora testar tudo que a gente fez, desde a ZI, se tá tudo certo, se ela tá recebendo mesma mensagem até o agente, se ele tá funcionando, se o modelo tá funcionando e o nosso post também juntamente com o Supase. É isso que a gente vai fazer agora. Eu vou vir aqui no web hook. Como ele tá em fase de teste, eu preciso sempre ficar escutando, pedir para ele fica escutando se eu recebo alguma requisição. Para isso, eu tenho que vir aqui, ó, listen for test event. Ele tá aqui escutando.

**19:48** · Agora eu vou lá no meu WhatsApp agora e aqui dentro do meu WhatsApp eu vou mandar mensagem para esse número aqui, que é o número que tá conectado lá na ZPI. Por isso que eu falei que se você tiver dois números fica mais fácil.

**19:58** · Então eu tô num outro número conectado aqui no meu computador. Vou mandar mensagem para aquele número que tá conectado lá na ZPI. E aí eu vou mandar oi, boa noite. Agora vamos ver no nosso N8N se ele recebeu. E veja que ele já recebeu. O node foi executado com sucesso. E aqui eu tenho todas as informações da minha mensagem. Por exemplo, o meu nome, cadê? Ele tá aqui.

**20:16** · Easus Felipe, que é o nome desse número que eu acabei de enviar, o nome que tá lá. Ele tem até o link da foto. Ele tem inclusive a o nosso texto. Oi, boa noite. Ele tem também o telefone que eu acabei de enviar essa mensagem. Então ele tem todas as informações, informações essas que a gente vai usar para criar os leads. É daqui que vem as informações para criar lá no Supase. É daqui que vem as informações para ele jogar lá no histórico de conversa do N8N. Enfim, para que a gente não precise ficar toda hora que a gente quiser testar o fluxo vindo aqui em listen for test event, eu vou simplesmente pinar essa mensagem.

**20:44** · Quando a gente clica aqui, ela fica salva. É como se sempre que eu rodasse esse fluxo, ele vai rodar como se eu tivesse acabado de receber essa mensagem. Basicamente é isso. Feito isso, eu já pinei. Veja que apareceu o pinzinho aqui e eu vou executar agora o fluxo como um todo. E aí vamos ver se ele tá rodando muito bem, se tá rodando tudo certo. Veja que ele acabou de executar o node do Super Base, então aparentemente deu certo. Ele precisa ter criado esse lead lá no Supase. Agora ele me deu um problema aqui no HTTP request.

**21:10** · Na hora de enviar essa mensagem de volta, era para ter recebido aqui uma mensagem. Lembra que esse número tá conectado lá com a Zap? Ele pediu essa requisição aqui para enviar a ZPI. Envia essa mensagem, por favor. E ele não enviou. Vamos ver o porquê. Ele tá me falando que o campo mensagem está vazio e na verdade ele não tá. Ele só tá, não sei por ele deu algum problema aqui. Não tem problema. Veja que a gente precisa arrastar pro campo mensagem, se esse problema acontecer com você, esse campo de output. Que que é essa mensagem? Essa mensagem aqui é a mensagem que o agente enviou.

**21:41** · Fica tranquilo que no fluxo que você vai baixar não vai dar esse problema que eu já corrigi aqui. Então você não vai ter que fazer essa troca que eu acabei de fazer. Mas só para você entender qual foi o problema. E essa mensagem aqui de output é a resposta do agente. Olha só. Oi, boa noite, seja bem-vindo. Me conta rapidinho. Você tá buscando saber mais sobre atualizações com IA, cursos, eventos, comunidade, Techmoney, isso tudo. Da onde ele tirou essas informações? Que que é Techmoney?

**22:00** · Eu coloquei para ele no prompt que se você quiser alterar pro nome da sua empresa, pro seu cliente, você fica à vontade. Tá todo aqui no prompt. Isso aqui é só a título de exemplo. Então essa foi a mensagem do agente. Agora sim que eu preenchi certinho, né, que tava faltando, eu vou dar o execute step. Ou seja, só executei esse último node, que era o que tinha dado o problema. E olha o que apareceu aqui no meu WhatsApp, a mensagem: "Oi, boa noite, seja bem-vindo, me conta rapidinho. Você tá buscando saber mais sobre automação e a então tá tudo funcionando com a Zapi criou tudo certinho lá no Superabase.

**22:26** · Então aqui dentro do nosso base, a gente vem em project overview". A gente na verdade vem em table editor e a planilha lead é para ter criado o nosso lead e de fato ele ainda não criou. Provavelmente isso aqui aconteceu porque eu selecionei a minha credencial errada no N8N. Então deixa eu já corrigir isso. Na verdade, olhando aqui, tava tudo certinho. A minha credencial tava certo. Supas account 2. Só que veja que esse node aqui ele vai encontrar o cliente. Então ele vai buscar se esse cliente existe lá na nossa planilha.

**22:53** · Uma vez que ele não existe, porque a planilha não tem nada, como vocês acabaram de ver, ele vai vir para cá, para baixo, em criar cliente. E aqui tá selecionado a minha credencial errada. Então eu vou selecionar minha credencial de maneira correta. Agora vou executar o fluxo de novo. Então é como se ele tivesse recebido de novo essa mensagem. Então ele vai gerar uma nova resposta aqui pra gente, mas a gente testa o fluxo como um todo. Prontinho, de novo. Eu recebi minha a mesma mensagem, então ele tá respondendo como se eu por que eu não mandei boa noite de novo? Porque lá eu pinei a mensagem.

**23:21** · Então para ele é como se eu tivesse mandado boa noite de novo. Ele vai gerar todo o fluxo novamente, inclusive com a resposta. Então aqui aparentemente deu certo. Aqui inclusive ó ele apareceu que ele já criou meu nome. Vamos ver de novo lá no superabase se deu certo. Agora sim, se a gente olha aqui na nossa planilha leads, ele criou o ID. Lembra que eu falei que sempre começa num a data e o horário que foi criado? o meu lead, o nome do lead e o meu telefone.

**23:42** · Perfeito. Outra coisa que eu preciso ver é aqui em N8N chat Hister. Lembra que eu falei que ele mesmo automaticamente ia criar essa planilha, ia colocar aqui tudo que a gente conversasse? Ele mesmo criou isso. Ele criou a coluna ID, session ID. E veja que esse session ID ele é o telefone do lead. Veja que aqui a gente tem o Lead ID, que é o telefone do lead. Isso aqui é muito importante para você entender. Quando a gente criar o CRM, ele vai pegar as informações da planilha lead e colocar junto com as mensagens recebidas aqui. Então ele precisa ter um dado, uma coluna em comum. Através de qual coluna eu vou saber qual lead qual? Através da session ID.

**24:13** · Por telefone não se repete, cada um tem o seu. Leads, quando a gente vem aqui, lead, telefone não se repete, cada um tem o seu. Então ele vai cruzar esses dados e vai conseguir juntar as informações. Vai ficar mais claro daqui a pouquinho quando a gente for ver lá.

**24:24** · Então, já tá tudo certo. A única coisa que eu quero que você faça aqui é dentro de N8N Chat History, você clique aqui para criar uma coluna nova, porque essa coluna ela vai ser a coluna que vai mostrar pro nosso CRM depois o horário que o lead mandou mensagem. E o nome dessa coluna que você vai colocar vai ser justamente esse: Hora sem espaço, underline data underline mensagem. Você vai vir aqui em type, ou seja, o tipo de dado que você vai passar para ela, e você vai selecionar time stamp, mas não é qualquer time stamp, é time stamp pz, tá vendo?

**24:54** · Ele vai dar data e hora, incluindo time zone, o horário ali de acordo com a região. Depois que selecionou isso, a gente simplesmente vem em save. Ele foi criado essa tabela.

**25:02** · Pronto, agora ele salvou. Tá vendo que tá vazio? Por que tá vazio? Porque a gente mandou mensagem antes. Antes não existia essa coluna aqui com data e hora. Então o que que a gente vai fazer agora? Vamos rodar o fluxo mais uma vez para ver se a próxima mensagem já vem com horário e data. Então, aqui no nosso N8N, vamos rodar o fluxo mais uma vez.

**25:17** · Eu vou receber mais uma mensagem ali no WhatsApp. Quero justamente ver se agora recebemos a mensagem e eu quero ver se lá no Supas ele colocou o horário também da mensagem que eu recebi. Veja que ele não colocou. Então tem alguma configuraçãozinha aqui que eu preciso arrumar. E na verdade o que faltou foi o valor padrão. Tá vendo? Default velho.

**25:34** · Eu preciso colocar aqui o now. Ele vai preencher com data, horário. Mas qual dato, horário? Eu não tinha passado para ele. E aqui em default value ele a gente precisa passar com horário e data de agora. Então, agora que eu passei essa expressão, vou salvar novamente, vou rodar o fluxo mais uma vez e aí a próxima vai aparecer aqui com a mensagem, já com o horário, com a data.

**25:53** · Então, vou rodar mais uma vez o fluxo.

**25:54** · Recebi mais uma vez a mensagem e agora sim recebemos a mensagem que eu enviei com o horário e com a data. Isso aqui vai ser importante de novo, porque quando a gente colocar lá no CRM, ele precisa ter um referencial para saber quais foram as mensagens de hoje, que hora que foi enviado, enfim. Prontinho, agora o nosso fluxo, o nosso agente, ele tá completamente criado e totalmente pronto para usar. Agora que já tá tudo criado no nosso N8N com o nosso agente, nós vamos para o antigrav integração do CRM com esse agente, na verdade com o nosso super base para pegar as informações.

**26:24** · Mas antes eu já quero pedir que se você tiver curtindo esse vídeo cheio de informação, já deixa o like aqui que ajuda demais o trabalho, ajuda demais o canal, beleza? Então deixa o likezão aí, se não tiver inscrito, já se inscreve no canal também. Chegando aqui no Anti Gravity, no Google AntiGravy, quando você abrir a ferramenta, você precisa instalar ela no seu computador, caso você ainda não tenha. Quando você instalar ela, vai abrir essa tela aqui. Nessa tela a gente vai ver claramente que ele já pede um open folder. O Antigravity, já tem um vídeo, inclusive meu explicando tudo sobre o Antigravity.

**26:53** · Vocês não assistiu, eu vou deixar aqui para você, vai tá na descrição também. Pode clicar e assistir o vídeo para entender melhor como é que funciona o Anti Gravy, se for o seu caso. Mas o Antigravery ele é baixado no seu computador e ele cria todos os projetos no seu computador. Então claro, a gente vai criar aqui um CRM, mas se você quiser hospedar esse CRM, colocar ele em nuvem para que outras pessoas consigam acessar, você vai precisar ali, por exemplo, usar um serviço da Hosinger, inclusive Hoshinger, que tem cupom aqui de desconto do canal. Então, se você for no nossa descrição e entrar pelo link que tá ali, você vai pagar com desconto as hospedagens da Hostinger.

**27:24** · Usa Hostinger quando for usar, usa aqui o cupom de desconto para você pagar mais barato e também dar uma força aqui pra gente. Mas voltando aqui pro antigravy, por isso, já que ele tá sendo criado no seu computador, ele vai pedir para você um open folder, para você abrir uma pasta no seu computador, onde ele vai criar o projeto. Eu vou abrir aqui uma pasta, vou vir aqui em nova pasta e vou criar projeto CRM wats. Essa pasta acabou de ser criada. Eu vou vir aqui em abrir. Quando eu venho em abrir, ele vai abrir essa pasta, literalmente abrir essa pasta. Tá escrito aqui projeto CRM wats. E tudo a partir de agora que ele criar, ele vai colocar dentro dessa pasta. Aliás, essa é a parte importante.

**27:57** · Aqui embaixo também, né, na descrição, no material, existe um documento que se chama CRM kit replicação MD. Que que é isso? para que a gente garanta que você vai ter o melhor resultado com esses promps que a gente vai mandar. Eu já passei uma uma instrução, uma pré-instrução para ele do que que ele precisa fazer no projeto. E aí eu salvei nesse arquivo que se chama CRM kit replicação. E por que replicação? Porque é exatamente o sistema que eu já fiz outras vezes, que inclusive eu já fiz para clientes meus.

**28:23** · Então para facilitar, para você não ficar gastando um monte de prompt, a gente não ficar gastando muito tempo aqui, eu deixei esse arquivo que você vai precisar fazer o seguinte, você vai baixar esse arquivo, tá? Ele tá num ponto MD que significa markd, uma linguagem. E a gente vai colocar ele aqui, ó, em projeto CRM wats. Você pode simplesmente arrastar aqui e é o que eu vou fazer.

**28:42** · Então, eu tenho já esse arquivo baixado aqui e eu vou simplesmente colar ele aqui. Vou soltar, arrastar para ele.

**28:48** · Veja que ele já abriu dentro de projeto CRM Wats. Precisa estar aqui, não é em Open Editors, é dentro de projeto CRM Wats. E aqui tem todas as instruções, ó.

**28:56** · Se você lê kit, replicação, tal, tal, tal, como usar, copia esse documento, OK? Isso aqui é instrução para o antigravery. Tem um documento que também é instrução para você. que é um documento que tá no Not, que é exatamente esse documento aqui, guia do aluno, como criar seu CRM de conversas no WhatsApp. Então, sim, tá tudo aqui explicando tudo que você precisa fazer.

**29:14** · Siga as etapas abaixo na ordem. Então, caso você tenha assistido a aula, uma aula longa, mas você quer ter um material, tá aqui que você precisa fazer. E temos os passos. Passo um, prepare a pasta do projeto. Então, cria uma pasta vazia no seu computador pra gente colocar o nosso kit replicação, que é o que a gente acabou de fazer.

**29:29** · depois iniciar um chat com um antigravery. E aí eu já deixei o prompt que você vai mandar pro antigravy. Então tá aqui, a gente vai copiar esse prompt.

**29:38** · Vamos abrir aqui o antigravery e a partir disso a gente vai pedir para ele criar o CRM. Mas a gente precisa antes de tudo criar um MCP. Que que é o MCP?

**29:47** · Uma maneira do antigravery conseguir se comunicar com o Supase. Então lembra que ele vai colocar todas as informações do lead para aparecer pra gente? Então vai aparecer lá o nome do lead, o telefone do lead que foi conversado. Aonde ele vai pegar essas informações? lá no Supase. Então, a gente precisa criar um MCP lá no Supase. A gente tem aqui, ó, no canto superior direito, você vai ver aqui, ó, MCP Server, vai abrir um monte de MCP, tem um monte de MCP aqui já integrado nativamente com antigravery, mas a gente vai escrever aqui supase.

**30:13** · Encontrando o Supase. A gente vai clicar aqui, vai vir em install, fazer a instalação, e ele vai pedir o quê? o seu Base Access token. Nesse caso, a gente vai abrir o nosso Base, vir aqui no canto superior direito, vi em account preference. Aqui dentro vai aparecer uma um access token aqui nessa nesse menuzinho lateral aqui. A gente vai generate new token. É um lugar diferente porque aqui eu tô gerando um token pro MCP, não é um token necessariamente para usar a API, que é o que a gente fez no NN. A ideia é a mesma, só que são coisas diferentes.

**30:45** · Então a gente vem aqui em generate new token. A gente vai colocar um nome para esse token. Esse token ele pode inspirar em 30 dias, em um ano, nunca inspirar. Você pode colocar aqui sempre que você quiser, customs, se você quiser colocar um outro período, eu vou deixar para ele inspirar em 30 dias, porque eu não vou usar esse projeto. Mas se você for usar esse projeto, lembra que todo dia, todo momento, o MCP do Antigravery precisa conversar ali, precisa, na verdade, o Antigravy precisa conversar com o Supas MCP. Se ele inspirar em 30 dias, daqui 30 dias o teu projeto vai dar errado.

**31:12** · Quando o antigravery for conversar, quando na verdade o sistema de CRM ali, o antigravery for conversar com o Supas, não vai conseguir conversar porque vai ter inspirado. Então, no seu caso, eu aconselho colocar nunca, tá bom? Então eu vou colocar 30 porque para mim não tem problema, eu não vou usar esse projeto mesmo. Então a gente vai gerar o token. Token gerado, não vai mostrar para ninguém claramente. E você vai copiar esse token. Copiado o token, a gente volta no antigravy e a gente cola esse token aqui. Prontinho. Já falei pro antigravery, ó, sou eu lá, pode fazer a integração aqui. Ele já vai fazer o MCP já integrando com o meu token.

**31:42** · Então, a hora que a gente der save aqui, ele já tá criando tudo. Uma vez que ele tiver criado, ele vai aparecer aqui como enabled, ou seja, ativado. E agora, se a gente vi aqui em cima e ver em manage mp servers, a gente já vai ver que nós temos ativado o MCP do Supase com as 29 requisições, tarefas que ele aprendeu a pedir, se comunicar com o Supase. Então, a partir de agora tá tudo pronto, já estamos integrado com Supas aqui do Antigravery.

**32:09** · Se ele precisar falar para pedir qualquer informação com Superabase, a gente não precisa passar, ele vai fazer de maneira automática, só a gente mandando prompts. E agora sim, então, dito isso, eu vou voltar lá no Notion, copiar aquele prompt e colar aqui de novo. A gente tá aqui no guia do aluno. Vou copiar esse prompt. Vamos voltar no antigraven e colar ele aqui do lado. Simplesmente colei o prompt do jeito que tá lá e vamos apertar send para enviar e ver o que que ele cria a partir daqui.

**32:39** · Prontinho, eu já fiz a minha requisição.

**32:41** · Ele criou um plano de implementação, que inclusive é esse aqui que tá na tela, ó.

**32:45** · Ele vai mostrar aqui onde ele vai explicar tudo, tudo que ele vai fazer. A única questão importante é: eu esqueci de mandar uma imagem anexa como referência de design. Eu também deixei essa imagem anexa referência de design liberada no arquivo ali. Eu vou simplesmente pegar essa imagem e vou enviar para ele como referência para ele entender como que eu quero que o meu CRM seja em termos de design ali, até mesmo algumas funcionalidades. Eu só tinha esquecido de fazer isso. Vou adicionar aqui. Você já pode mandar de primeira aqui junto com o promp. Se você tiver esquecido também, coloca igual eu vou fazer aqui. O bond Gravity é isso.

**33:15** · A gente consegue simplesmente conversando com ele, mandando conforme a gente lembrar, conforme a gente quiser mudar alguma coisa no projeto com a maior facilidade do mundo. As referências de imagem que eu vou mandar são essas aqui.

**33:26** · Então, se você quiser, inclusive um processo exatamente igual ao meu, você pode mandar essa mesma imagem. Eu só vou vir aqui em copiar imagem. Vou no antigravery, vou colar essa imagem aqui.

**33:37** · No prompt anterior, eu esqueci de enviar essas essas imagens como referência de design. Então, por favor, leve em consideração essas imagens como referência de design para criar o CRM.

**33:47** · Prontinho. Agora eu vou só enviar novamente. Com isso, ele vai colocar, né, essas imagens como referência no próprio plano de implementação e depois eu vou simplesmente aceitar o plano de implementação para ele já ir criando o CRM por conta própria aqui, sem eu precisar fazer mais nada. Aqui ele tá me mandando algumas informações para eu dar run, para eu aceitar que ele rodeo. Tá vendo? Ele tá rodando vários códigos aqui por trás e ele vai me pedindo, tá vendo que ele tem aqui ask everytime? A gente pode colocar para ele sempre correr o código, sem precisar me pedir nada.

**34:18** · Eu gosto de colocar ask every time, então por costume, eu deixo assim padronizado. Eu tenho sempre que vir aqui aceitar, pedir para correr, porque eu fico dando uma olhada aqui no que ele faz. Eu entendo algumas coisas aqui do código. Se der algum problema, eu consigo eu já mexer e resolver isso aqui muito rápido. Então eu gosto. Mas se você preferir também, quiser mais agilidade, você pode vir aqui e deixar em ask everytime, always run, que aí você não precisa dar nenhum desses OKs que eu tô dando aqui.

**34:43** · Agora sim, ele já entregou. Veja que ele mandou algumas coisas aqui importantes.

**34:47** · Primeiro, ele mandou todas as alterações que ele pediu para fazer em todos os arquivos. Quais arquivos? Esses aqui que são que estão dentro do nosso projeto.

**34:54** · Tá tudo aqui, tá vendo? Isso tudo tá dentro da nossa pasta projeto CRM wats.

**34:58** · Eu vou simplesmente dar um aceitar all e vamos ler o que ele falou. Tudo pronto.

**35:02** · O app do CRM WhatsApp Viewer foi totalmente desenvolvido usando as imagens de referência como base e tal, tal, tal. E tá me dizendo que tá tudo certo, que eu já posso acessar o site.

**35:10** · Eu vou pedir para ele um link clicável para que a gente possa entrar no nosso navegador para visualizar esse site. Me mande um link clicável para que eu possa abrir essa página no meu navegador web.

**35:24** · Agora sim, ele forneceu um link. Vamos ver se funciona. E funcionou. Vou colocar aqui na tela para vocês verem.

**35:31** · Tá aqui. Acessar o chatbox. Aqui ele tá me pedindo um e-mail e aqui ele tá pedindo uma senha. Felipe, como que eu vou colocar um e-mail e senha aqui? Da onde que veio isso? Presta atenção, porque essa parte é importante. Quando a quando a gente tá falando de um sistema como esse, um sistema onde só determinadas pessoas podem ter acesso ao que tá escrito aqui, ao que tá, as mensagens estão sendo trocadas aqui, a gente não pode simplesmente colocar um botão aqui escrito crie próprio login e senha, porque qualquer um que viesse aqui ia poder criar o seu próprio login e senha e entrar e visualizar as mensagens. A gente não quer isso.

**35:59** · Quem vai garantir os acessos que vão poder entrar aqui somos nós, por uma questão de segurança óbvia. Isso aí você inclusive vai aplicar com seus clientes.

**36:08** · Para fazer isso, nós vamos lá no Supas vou te mostrar como você vai criar um login e senha. Então aqui dentro do nosso superabase a gente vai sair, nós vamos vir aqui em authentication, nós vamos criar, nós vamos adicionar um usuário, add user. Tá vendo? a gente pode enviar uma uma invitation, um convite via e-mail ou a gente simplesmente pode criar esse usuário aqui. Eu vou criar com qualquer e-mail, vou criar esse usuário aqui no nosso sistema do Supas, que também vai fazer essa gestão de quem pode ou não acessar o site. Ele tá falando que essa senha foi encontrada no vazamento de dados e tudo mais.

**36:39** · OK, vamos só deixar assim mesmo porque eu quero só acessar lá. A gente volta aqui agora a gente precisa colocar o mesmo e-mail\_lineas.com.

**36:50** · E aqui eu vou colocar 1 2 3 4 5 6.

**36:52** · Coloquei minha senha e vou dar entrar.

**36:54** · Vamos ver se tá funcionando o sistema de login. Ele deu e-mail ou senha incorretos. Vamos ver se eu digitei tudo certo. Vou copiar exatamente o e-mail que eu coloquei aqui. E ah, eu tinha escrito errado o e-mail lá no Supase. Ó, é ias. Mas tudo bem. Deixa, deixa aqui a senha. 1 2 3 4 5 6. Não tem como tá errado. E vamos dar entrar. Feito isso, de novo, apareceu o aviso lá da senha para eu trocar, porque não é uma senha forte. Claro. Feito isso, estamos dentro já aqui do nosso CRM.

**37:18** · E aqui a gente pode clicar na mensagem e nós vamos ter aqui toda a nossa conversa sendo feita aqui entre o agente e o nosso lead. Veja que a gente tem as mensagens que o agente mandou. Então aqui tá escrito quem que mandou essas mensagens para quem que foi mandado. A eu. Sou no caso eu, né? Que na verdade era para est contrário. Aqui a gente pode pedir para corrigir, mas o que eu quero que você veja são as funções. Tudo funcionando aqui. A gente não tem nada nessas outras telas.

**37:47** · A gente pode inclusive pedir para ele tirar essas outras informações e deixar somente mensagens. A gente clicando aqui, a gente tem acesso a tudo que foi conversado do nosso cliente. A gente só precisa agora pedir para ele colocar as datas. Na verdade, ele até colocou as datas, mas eu quero que ele coloque o horário no estilo formato WhatsApp. Então, vou mandar um print do WhatsApp para ele colocar do jeitinho que fica no WhatsApp. Aqui embaixo aparecendo a data. A data já vai aparecer aqui, né, hoje, amanhã e também aparecendo o horário que foi enviado.

**38:13** · Para isso, vou vir aqui no nosso WhatsApp e vou mandar para ele que eu quero este formato aqui de data e hora nas mensagens. Vou enviar para ele a imagem e o promptora. Por favor, gostaria que você colocasse esse mesmo sistema de data e hora que o WhatsApp utiliza nas mensagens. Então, por favor, embaixo de cada mensagem enviada e recebida, coloque o horário que foi enviado e recebida e também agrupe tudo por datas, como dia hoje, ontem, dia 2/02/2026, enfim, agrupe as imagens no estilo WhatsApp.

**38:43** · Prontinho, vamos dar esse prompt, vamos ver se ele corrige. Isso aqui é só mais uma das coisas que a gente consegue fazer. Lembra o que eu falei? É tudo feito via prompt, então você tem essa facilidade, você consegue ir conversando e pedindo para ele cada erro que aparecer, pedindo para ele atualizar algumas coisas no projeto, no design. Então você fica muito livre para isso.

**39:04** · OK? Ele tá me dizendo que ele já fez as alterações. Vamos dar um refresh aqui na página. A gente tem aqui as mesmas mensagens e ele tá me dizendo que ele colocou já as datas. O que ele fez foi agrupar hoje. Então veja que a data mais recente e a única que a gente tem o horário, ela tá mais para cima. Na verdade, eu quero que ela fique mais para baixo. Faz mais sentido, né, quando a gente lê as mensagens, que as mensagens mais recentes estejam mais para baixo aqui no scroll. Também vou pedir isso para ele, para ele dar uma ajustada. Perfeito.

**39:32** · Eu apenas gostaria que as mensagens mais recentes estivessem para baixo, assim como o WhatsApp faz. As mensagens mais novas, elas ficam mais para baixo ali na tela.

**39:41** · E eu gostaria que você fizesse a mesma coisa. Quero também que você exclua todos os painéis laterais que não tenham função. Deixe apenas o painel de mensagens e o painel de settings ou configurações. E dentro do painel de configurações, eu gostaria de adicionar uma opção que permita que a gente altere para dark mode ou light mode, sendo o light mode o modelo que já está branco e azul, e o dark mode, a mesma versão, só que com fundo preto. Prontinho, vamos enviar isso para ele e vamos esperar ele fazer essas novas mudanças e adaptações no nosso layout.

**40:19** · Mais uma vez ele responde: "Prontinho, resolvi tudo que você pediu". E mais uma vez a gente vai dar uma olhada como é que ficou. Para isso, a gente vem, dá um refresh na página. Veja que já funcionou. Ele colocou aqui e o nosso mensagem e settings. Ele manteve só esses menus. Vamos ver se ele corrigiu a mensagem mais recente. Tá para baixo agora, inclusive com o horário, inclusive da mesma maneira, mesma formatação que o WhatsApp usa. Aqui em settings, ele deu a opção de light mode ou dark mode. Então agora a gente pode oferecer pro nosso cliente essa opção de dark mode. E aí, olha só, ele já deixa tudo escurão, tudo bonitão.

**40:50** · E basicamente é isso. A partir de agora, todas as mensagens que você enviar lá no nosso WhatsApp, o fluxo do agente do N8N vai fazer toda aquela recepção da mensagem, vai passar pro agente, ele vai responder, que é aquilo que a gente tem justamente nesse fluxo aqui que a gente viu. E ele vai fazer todo o atendimento, passar tudo lá pro Supas e do Supas ele vai passar para o nosso CRM.

**41:14** · Lembrando mais uma vez que para você ter um projeto desse bem robusto, funcionando muito bem, não basta você ter só um CRM funcionando bem, você também precisa de um agente de inteligência artificial funcionando da melhor forma possível. E por isso eu não poderia deixar de te mostrar o meu super agente humanizado aqui. Um agente completo, bem mais completo que o outro. Um agente que entende vários tipos de mensagem, texto, áudio, imagem, um agente que entende mensagens picadas, que também responde de uma forma humanizada, ou seja, através de mensagens picadas também.

**41:44** · todo esse fluxo muito mais inteligente do que aquele que a gente acabou de criar, fazendo com que o seu projeto valha ainda mais, atendendo os clientes do seu cliente de uma maneira muito mais personalizada e adicionando muito mais valor para os seus projetos. E este fluxo, não só este fluxo, como todas as minhas estratégias de venda e captação,

**42:03** · estão disponíveis para você no Aian, o meu curso, em que o único objetivo é fazer com que nos próximos 14 dias você fature R$ 3.000 usando os meus agentes, esse aqui que eu te mostrei, mais um outro agente de agendamento, que são os agentes que eu vendo para os meus clientes até hoje e também mostrando todas as minhas estratégias de venda e captação. O único objetivo desse curso é fazer você faturar seus primeiros 3.000 nos próximos 14 dias. E o preço desse curso é absolutamente ridículo. Então entra lá no QR code que tá aparecendo aqui na tela e confira você mesmo o valor que é absolutamente ridículo.

**42:32** · Agora eu quero saber de você o que você achou dessa nossa super aula completaça, criando e passando por tudo que você podia ver sobre o nosso agente de agendamento aqui no WhatsApp conectado já funcionando e também essa criação desse fluxo completo com CRM visual, bonito, interativo, muito bem construído, usando apenas pouquíssimos prompts que a gente mandou usando o \[música\] antigravery e com todo esse material. Diz aí, você gostou ou não gostou dessa aula?

**42:57** · Se você gostou, por favor, deixa o seu like, deixa o seu comentário também dizendo o que você achou, se ficou com alguma dúvida e manda esse vídeo para algum colega seu, algum amigo que também tá querendo aprender mais sobre automação, porque isso ajuda demais o nosso canal \[música\] a crescer cada vez mais e a trazer cada vez mais conteúdos como esse, detalhados, totalmente completos aqui para você. Também vou deixar você aqui agora com um vídeo onde eu explico para você quais são os 14 nodes essenciais do N8N, aqueles nodes que você precisa saber. Eu criei o guia do preguiçoso.

**43:26** · Você só precisa saber 14 nodes do N8N para saber criar fluxos completos. E quais são esses 14 nodes? Assiste aqui no vídeo e descubra. No mais, semana que vem eu tô de volta. Tamo junto. Um grande abraço e falou. Yeah.