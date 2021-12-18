# IronHack
Trabalhos do curso de Data Analitycs da Iron Hack

Nome do Projeto: Global Shark Attack
Objetivo:
1.	Utilizando python, limpar e analisar os dados de uma tabela sobre ataques tubarões no mundo. 
2.	Buscar a partir desses dados responder uma pergunta que deve ser definida por pelo próprio aluno. Meu desafio será:
a.	Definir a população que mais sofre ataque de tubarão para elaboração de uma campanha de MKT voltada a prevenção de ataques.

Detalhes do projeto
A proposta principal do projeto é desenvolver as habilidades necessárias para entender uma tabela e extrair os dados úteis para uma análise, 
assim, a ênfase do projeto é voltada para o Data Cleaning. A tabela para análise foi extraída da plataforma Kaggle e conta, inicialmente, 
com mais de 600 mil elementos de informação.

Análise Descritiva
A tabela inicial estava muita suja, com muitas informações nulas que inviabilizavam sua análise. O arquivo inicial apresentava 25723 linhas, dessas, 19421 estavam completamente vazias. 
 
O arquivo conta com 24 colunas das quais 8 foram utilizadas para a análise final dos dados. Das colunas que foram excluídas, 10 não continham informações 
plausíveis para uma análise. Dentre essas informações temos: link para o PDF que descrimina sobre os acidentes, pesquisador responsável pela anotação do ataque de tubarão, número de registro do caso, dentre outros. Das 14 colunas restantes 8 foram consideradas viáveis para análise. Dentre as colunas excluídas temos, por exemplo, a coluna “Time” que apresenta o registro sobre o horário em que ocorreu o acidente, essa coluna continha menos da metade das informações preenchidas e por isso foi excluída. Outro exemplo foi o da coluna “Injury”, essa coluna não tinha um padrão de preenchimento e cada pesquisador escreveu o texto que quis na célula. Essa falta de padrão para descriminar a lesão da vítima do ataque inviabilizou sua análise, e foi excluída.

A coluna “Age”, que informa a idade da vítima do acidente, por diversas vezes apresentou mais de um caso registrado na mesma linha. Esses dados foram tratados adicionando colunas individuais com os mesmos dados do ataque, mas cada linha com uma única informação de idade da vítima. Com isso, o data frame final utilizado para a análise dos dados foi formado por 6327 linhas e 8 colunas. Essa quantidade de informações totaliza apenas 8,2% da possibilidade de informações do arquivo inicial.
A análise do nosso data frame final não nos traz novas informações sobre os ataques de tubarão no mundo, porém, confirma algumas informações já conhecidas sobre os padrões desses ataques pelo mundo.

Não podemos constatar que estamos vendo um aumento do número de ataques de tubarões com nossos dados. Apesar de termos uma aparente crescente dos ataques nos últimos 10 anos (nosso arquivo é de 2018), ou seja 2007 até 2017, diversos fatores externos aos nossos dados podem fazer parte desses resultados. Um indicativo de erro é que mais de 20% do total de ataques dos tubarões de todo o arquivo (que tem seu primeiro registro datado de 1748) está entre os 10 últimos anos de registro. Isso mostra que provavelmente o controle e os registros dos ataques vem aumentando a cada ano, e não a quantidade de ataques em si.

Outra informação que podemos tirar da literatura e que a correlação dos nossos dados aponta para o mesmo sentido é sobre o desinteresse dos tubarões em atacar humanos. Mais de 70% dos nossos dados mostram que o tubarão atacou uma vítima sem ter sido provocado. As principais atividades das vítimas de ataques de tubarões são surfe, nado e pesca submarina, que juntos totalizam quase 40% do total de ataques da nossa amostra. O nível de letalidade do ataque de tubarões é baixo, 75% dos ataques não foram fatais em nossos dados. Isso corrobora com o que a literatura apresenta sobre os ataques de tubarões. O pesquisador especialista em Tubarões da Universidade Estadual de São Paulo (Unesp), Otto Bismarck explica: “tubarões atacam por confundir o humano com algum peixe ou presa durante a caça; por ter o território invadido; e por defesa, em casos em que é atingido por alguém enquanto nada.”  

O alto nível de ataques de tubarões relacionados com esportes ou atividades do mar associado a baixa incidência de fatalidade pode demonstrar o desinteresse do animal, provavelmente ao perceber que aquela presa não faz parte da sua cadeia alimentar, corroborando assim nossos dados ao que a literatura da biologia marinha apresenta.
Outra informação que não podemos afirmar a partir dos nossos dados é a de que existe uma preferência dos tubarões em atacar homens do que mulheres. 89% dos ataques registrados era de homens, porém, é amplamente sabido que os tipos de atividades marítimas já citadas acima são de prática predominantemente masculinas. Outro ponto sabido é que homens costumam se arriscar mais de forma idiota do que mulheres. Uma referência que podemos trazer para afirmar isso é o Prêmio Darwin, que é uma revisão anual sobre quais foram as formas mais idiotas pelas quais as pessoas morreram no mundo, e no geral, 90% dessas mortes são de homens. Assim, provavelmente os ataques de tubarões não tem relação com o sexo do envolvido.

Sobre a faixa etária que mais sofreu ataques de tubarões em nossa amostra temos que mais de 40% dos ataques foram em indivíduos com idade entre 15 e 25 anos. Essa é uma faixa etária mais comum tanto para a prática de atividades marítimas como para o comportamento de risco idiota, como cutucar um tubarão dormindo para “ver o que acontece”. Assim, tendo em vista a população de risco da nossa amostra, essa é uma faixa etária que faz sentido estar no topo dos ataques.

Por fim, a última informação que podemos tirar de nossa análise é sobre as principais localidades para os ataques de tubarões. Nossos dados mostram que no total de registros, os EUA lideram o ranking de ataques com um total de 2235 (35,6%), seguido pela Austrália com um total de 1343 (21,4%) e em terceiro a África do Sul com 580 (9,2%). Esses dados são condizentes com os dados publicados pela revista Forbes em 2017, onde apresenta um levantamento de 2007 até 2016 de ataques de tubarão no mundo. Assim como nossos dados, o levantamento da Forbes traz os mesmos top 3 em sua matéria.

Olhando para os estados ao invés dos países, a Florida é o estado mais acometido por ataques no mundo, sendo responsável por 17,7% de todos os ataques da nossa amostra. Um rápido levantamento no Google nos mostra New Smyrna Beach é uma cidade localizada no estado americano da Flórida, no condado de Volusia e é intutulada como a “capital mundial das mordidas de tubarão”. Em nossos dados essa praia também lidera o ranking de localidades, inclusive, o top 3 localidades com mais ataques de tubarão se encontram na Florida, dentro do condado de Volusia.

Só por nota de curiosidade, nosso querido Brasil aparece na lista de localidades mais afetadas por ataques de tubarões. Boa Viagem, no Recife, garantiu a sétima colocação no ranking de localidades.

COMO CRIAR UMA COMUNICAÇÃO PARA PREVINIR OS ATAQUES DE TUBARÕES?

Definindo a População alvo para a campanha:
	- Nossa campanha precisa estar voltada para o público masculino, entre 14 e 25 anos que gostam de esportes de aventura.
	- Os pontos com mais ataques de tubarões se encontram em regiões onde as ondas são constantes e a prática do surfe é uma tradição. Esses locais normalmente são muito visados para Surf Trip´s. Assim, o foco da campanha deve estar voltado não para os locais que conhecem a região e seus perigos, mas sim para estrangeiros que se aventuram nessas regiões em busca de um ambiente favorável à prática esportiva.

Casos sobre a imprudência da nossa população que podem ajudar no direcionamento da campanha:
1.	Um jovem Australiano chamado Harrison, que andava de barco com seus amigos avistou uma baleia boiando no meio do mar. O jovem “gênio” não hesitou e pulou no mar para ‘surfar’ na baleia que ele achou que estava machucada. A inteligência em forma de gente escalou a baleia e fingiu que estava surfando. O que ele não percebeu, é que era a carcaça de uma baleia morta, que estava sendo devorada por dezenas de tubarões. Ao perceber a besteira que fez ficou lá, sentado na baleia até a guarda costeira se aproximar e tirar em segurança de cima do animal morto! Parabéns, Harrison!!
2.	Um jovem de 25 anos, em um dia em que uma tempestade transformou as ruas de Brisbane em rios turbulentos, o FERA pensou: “Vou surfar pelas ruas de Brisbane”. Parecia divertido, até que ele foi sugado para dentro de um dos esgotos. Depois de uma jornada acidentada e sinuosa de três quilômetros através do esgoto pluvial, ele saltou em um riacho, relativamente ileso. Fica a dica, nunca surfe em uma rua inundada.
3.	O jovem Zenk, um bodyboarder, resolveu viajar até a California para pegar onda. Essa costa é banhada pelo Oceano Pacífico, para quem não sabe, o Oceano Pacífico é maior do que toda a área terrestre combinada do nosso planeta. Você simplesmente não se joga para dentro do Pacífico sem antes estudar bem a região em que você está. O ponto de surfe que o jovem resolveu escolher foi um ponto onde os próprios surfistas locais não surfam, exatamente pela força da água e pelo fato de arrebentação terminar em uma parede rochosa. Os próprios salva-vidas de jet-ski foram avisar Zenk que ele estava em uma região muito perigosa e que deveria sair dali, mas o prodígio resolveu ignorar os avisos. Não muito tempo depois, um conjunto de ondas o jogou sobre as rochas e o jovem não sobreviveu.

Pontos Importantes para a Campanha:
1.	Por mais engraçado que possa parecer, não faça nada estúpido dentro do mar.
2.	Se está indo praticar um esporte de aventura marinha em um local desconhecido:

     a.	Estude o local antes de cair na água.
     
     b.	Converse com locais sobre os principais picos, às vezes o melhor pico é também o mais perigoso.
     
     c.	Sempre pense na relação custo-benefício antes de se jogar em um pico. Pegar um tubo pode custar a sua perna, ou pior...
     

CAMPANHA FINAL

Instrutor: Fala aí brotheri, beleza?

Surfista: Ahn?

Instrutor: É! Você mesmo! Tá indo fazer uma Surf Trip na Florida?

Surfista: Só... Vai ser irado!

Instrutor: Já se preparou para chegar nos melhores picos com segurança?

Surfista: Ihhh maninho, surfo desde mlk tá ligado. O surf tá na veia, é só cair no mar que eu faço o resto!

Instrutor: Não tenho dúvida disso, mas você sabia que a costa da Florida é a costa com a maior concentração de tubarões no mundo?

Surfista: ahn?

Instrutor: Tô falando, é o local com mais ataques de tubarões no mundo. Antes de cair no mar, troca uma ideia com os locais para saber se está com alerta de tubarão na região. E nunca caia na água nessa região se estiver com um corte ou sangrando de alguma maneira. Tubarões sente cheiro do sangue e vão atrás.

Surfista: Como assim irmão? Dá para sentir cheiro embaixo d’água?

Instrutor: ... / Acredite, eles podem sentir uma gota de sangue a quilômetros de distância. Cara, curte seu surfe, mas não tente inovar. Se não tem ninguém surfando em um pico com boas ondas, com certeza tem algo errado. É melhor encarar um “crowdzinho” do que se arriscar ser atacado por um tubarão.
