---
layout: post
title:  "Projeto OPAC - A nova platafora e interface web para SciELO"
date:   2018-04-17 23:59:59 -0300
categories: pt-br jobs scielo
---

## Préfacio:

Se você não sabia, eu trabalho no projeto SciELO por pelo menos 4 anos. SciELO é um dos maiores portais de periódicos de acesso aberto do mundo.
Você pode encontrar mais informação sobre SciELO no seu [portal principal][scielo-portal] e no seu [blog oficial][scielo-blog]

Nos últimos 2 anos, eu estive trabalhando tempo completo com Jamil e Roberta para reconstruir o maior ponto de acesso para conteúdo científico do SciELO.
Esse projeto foi chamado de OPAC. OPAC é um acrônimo para: **O**nline **P**ublic **A**ccess **C**atalog. Portanto o desafio foi a construção do zero de um site
que deve atender a pelo menos **22 milhões** de page views por mês.

O texto a continuação foi escrito para ser publicado no blog oficial, acabou não sendo publicado.

## Autores:

Escrevi este texto com a ajuda dos meus colegas: [**Roberta Takenaka**][linkedin-roberta] e [**Jamil Atta**][linkedin-jamil]. Ambos são pessoas desenvolvedoras
com grande experiência e  muito mais tempo no SciELO do que eu.


## Agradecimentos:

Obrigado para Roberta e Jamil, pelo trabalho duro e a paciência de cada dia. Também obrigado para Artúro Rendón de SciELO México que colaborou com código e conhecimento no projeto.
E finalmente, muito obrigado para Fábio Batalha, nosso chege até final de 2017, ele ajudou muito e nos deu liberdades para assumir riscos e trazer inovação para este projeto.

## Introdução:

Desde seu nascimento, o objetivo principal do Projeto SciELO é disponibilizar artigos científicos de acesso aberto e além de indicadores bibliométricos
da produção científica nacional alinhado com o estado da arte internacional. Desde de 2013, o Programa SciELO vem adotando as linhas prioritárias de ação de
fortalecimento da **profissionalização**, **internacionalização** e **sustentabilidade**.

A partir de novembro de 2017 contamos com um novo website SciELO para a coleção [SciELO Saúde Pública][scielo-sp]. Apresentamos aqui uma visão geral desta nova plataforma
assim como as novas funcionalidades e seus benefícios.

### Uma nova etapa no desenvolvimento com maior flexibilidade, rapidez e segurança:

Desde 2010, [SciELO][scielo-portal] tem usado [Python][python-org] como principal linguagem de programação para modernizar suas ferramentas e soluções tecnológicas,
pela sua natureza de ser uma linguagem de alto nível, multiplataforma e multi paradigma, entre outras características, o que mostrou-se acertado para o cenário e
os desafios apresentados ao longo do tempo.

Em novembro de 2017, foi lançado o novo website SciELO para a coleção [SciELO Saúde Pública][scielo-sp]. Esta nova plataforma, além de oferecer uma nova interface
com experiência visual mais agradável, apresenta também outras novidades como a integração com outras ferramentas e fontes de informação variadas como o [blog SciELO][scielo-blog]
em Perspectiva e o [blog de Press Releases][scielo-press].


Os usuários perceberão que as páginas do site são carregadas com maior rapidez, isso é devido ao uso da tecnologia [HTTP 2][http2], uma evolução do já velho conhecido protocolo HTTP
que reina na web. A comunicação também é mais segura pelo uso do protocolo HTTPS[1] permitindo que a comunicação entre o servidor e o navegador seja criptografada o que garante a
autenticidade do conteúdo enviado pelo site ao navegador e o sigilo de todos os dados enviados pelo usuário ao site
(por exemplo, quando o usuário utiliza a funcionalidade de "Enviar página por e-mail" na área de compartilhar).

Uma nova homepage com métricas atualizadas frequentemente, além dos número mais recentes, as últimas publicações no [blog SciELO em Perspectiva][scielo-blog] e o
[blog de Press Releases][scielo-press], e também no twitter da Rede SciELO. Assim, o usuário pode ficar atualizado com as últimas novidades e inclusive acessar diretamente estas
novidades clicando nos links.

A homepage do periódico também está de cara nova com acesso destacado para as páginas informativas e link ao sistema de submissão. Métricas atualizadas periodicamente e destaque
para as [Goolge Metrics][google-metrics] (índice e mediana [h5][h5]) além de link para a plataforma [Analytics de SciELO][scielo-analytics] facilitando o acesso para as métricas
do periódico em questão dentro do âmbito da coleção escolhida. Finalmente queremos destacar uma nova seção de artigos mais recentes e de notícias, permitindo assim ao visitante
frequente do periódico um acesso direto aos novos conteúdos.


Agora quando o usuário consultar o sumário de um número qualquer, podemos ver um novo recurso disponível: a ordenação de artigos desse número por critérios como: os mais novos
primeiro ou os mais antigos primeiro, o que facilita muito na hora de procurar um artigo específico em casos de publicação contínua por exemplo.

A parte central do novo site: a página do artigo, foi redesenhada totalmente para facilitar a leitura, informação dos autores e das afiliações, acesso aos PDFs em todos os idiomas
disponíveis, assim como o navegação simplificada entre as seções do texto e melhor acessibilidade aos recursos como as figuras e tabelas, como citar o artigo em questão. E em
coleções que estejam habilitadas o usuário também poderá usufruir de acesso ao serviço ReadCube.


### Uma gestão de conteúdo mais eficiente e amigável:

Quanto à gestão do conteúdo do site, os tempos de processamento para disponibilizar o conteúdo online, foram reduzidos drasticamente, também é possível atualizar qualquer artigo
a qualquer momento. Os ativos dos artigos, ou seja, imagens, PDF, XML, são carregados em um sistema próprio e cada ativo poderá ter seus metadados enriquecidos.

As páginas informativas podem ser criadas e editadas no editor de conteúdo [WYSIWYG][editor-web] dentro do próprio sistema, sendo desnecessário que o usuário possua conhecimento técnico da
linguagem [HTML][html], pois basta escrever o conteúdo como se editasse um blog. E as alterações destas páginas ficam publicadas imediatamente.

Também disponibilizamos novas funcionalidade que permitem um controle mais eficiente das mudanças como a exibição da data da última atualização de cada página informativa e um
controle de auditoria que permite saber quais foram as mudanças realizadas em cada versão das páginas, assim como a data e o usuário que as realizou.

### Mais que um website, uma plataforma de serviços:

Além do website que o usuário pode visitar (que é a Interface e internamente recebe o codinome de **OPAC**, acrônimo do inglês: Online Public Access Catalog), foram criados outros
dois sistemas, um dele foi nomeado: **PROC** (o codinome vem da abreviação de "processamento"), para melhorar a incorporação de conteúdo, integração com serviços internos e externos,
e o outro: **SSM** (acrônimo de Static Storage Manager), que serve de repositório de ativos (imagens, PDFs) permitindo assim o enriquecimento do arquivo com mais metadados, permitindo
assim uma rápida busca e recuperação para atender a demanda do site.


O **SSM**, pela sua natureza simples, de se tratar de um repositório de arquivos não tem muita complexidade na lógica de negócios, nem na modelagem dos dados, porém tem um esforço
grande para aumentar ao máximo as capacidades de armazenamento e recuperação dos ativos de diferentes naturezas (imagens, PDFs, XMLs) utilizando APIs, assim como a flexibilidade para
enriquecer seus dados.

O **PROC** tem como parte central o processo **ETL**[2] (Extract, Transform, Load em inglês) que permite mover grandes massas de dados de um ou mais sistemas ou serviços, para o
destino final, o website, de forma eficiente e consolidada. Possibilitando também que quando chega novo conteúdo, é processado somente o conteúdo novo, reduzindo assim o tempo de
processamento, os recursos necessários, e disponibilizando o conteúdo novo rapidamente ao usuário final. Tudo começa com a fase de **extração** é a coleta dos dados de diferentes
fontes como por exemplo o serviço que fornece os metadados e os XMLs dos artigos, assim como os feeds RSS dos blogs, etc… À continuação vem a fase de **transformação**, a parte
mais delicada onde é feito um tratamento e uma limpeza nos dados para atender as necessidades do negócio. Finalmente temos a fase de **carga**, que consolida todos os dados já
processados nas fases anteriores e disponibiliza o conteúdo no banco de dados do website (interface pública).

Todos os sistemas desenvolvidos nesta nova plataforma: Interface (OPAC), PROC e SSM tem integração contínua[3] (que se refere a uma boa prática de engenharia onde cada conjunto de
mudanças feitas pelos desenvolvedores passa por uma série de testes para garantir maior seguridad na hora de juntar todas as mudanças à versão final do código) o que permite menor
tempo para resolver erros e implementar melhorias em cada componente de forma rápida e eficiente.

A nova plataforma está "empacotada" utilizando a tecnologia [Docker][docker] o que permite maior flexibilidade para escalar serviços, ou seja, aumentar a capacidade de processamento
em tempos de maior demanda e reduzir quando a demanda é menor. Contamos dessa forma com mais garantias na distribuição e na implantação de novas versões da plataforma em ambientes
heterogêneos como encontramos em alguns países membros da [Rede SciELO][rede-scielo].

Portanto, além de permitir uma instalação no formato clássico, é possível também utilizar hospedagem na nuvem por se tratar de um ecossistema de cloud native applications[4],
distribuído e fácil de escalar horizontalmente, isso significa que podemos aumentar a capacidade de processamento quando houver maior demanda e vice-versa, assim como maior
resiliência para contornar falhas ou problemas com os servidores.

Todos os sistemas desenvolvidos estão baixo licença open source e disponíveis na plataforma GitHub aqui: [https://github.com/scieloorg ][scielo-github].

Novas ideias e melhorias surgem a cada dia, como pode ser uma possível integração com o sistema **SciELO Preprints**[5], por exemplo mostrando preprints relacionados ao artigo
que o usuários está visualizando, ou listando preprints dos mesmos autores do artigo, etc.
Nós, os autores, estamos orgulhosos de ter trabalhado neste projeto e poder seguir melhorando esta plataforma.

## Referências:
1. Secure your site with HTTPS. Disponível em: https://support.google.com/webmasters/answer/6073543?hl=en Acesso em 21 de Fevereiro. 2018.
2. ETL - What is and why is important. Disponível em: https://www.sas.com/en_us/insights/data-management/what-is-etl.html Acesso em 19 de Fevereiro. 2018.
3. O que significa integração contínua?. Disponível em: https://aws.amazon.com/pt/devops/continuous-integration/ Acesso em 21 de Fevereiro. 2018.
4. Developing Cloud Native Applications. Disponível em: https://www.cncf.io/blog/2017/05/15/developing-cloud-native-applications/ Acesso em 21 de Fevereiro. 2018.
5. PACKER, A.L., et al. Os Critérios de indexação do SciELO alinham-se com a comunicação na ciência aberta [online]. SciELO em Perspectiva, 2018 [viewed 12 February 2018]. Available from: http://blog.scielo.org/blog/2018/01/10/os-criterios-de-indexacao-do-scielo-alinham-se-com-a-comunicacao-na-ciencia-aberta/



[scielo-portal]: http://scielo.org/
[scielo-blog]: http://blog.scielo.org/
[scielo-press]: https://pressreleases.scielo.org/
[linkedin-roberta]: https://www.linkedin.com/in/roberta-mayumi-takenaka-709399/
[linkedin-jamil]: https://www.linkedin.com/in/jamil-atta-junior-78b3a825/
[scielo-sp]: https://scielosp.org/
[python-org]: https://python.org
[http2]: https://developers.google.com/web/fundamentals/performance/http2/?hl=pt-br
[google-metrics]: https://www.optimizesmart.com/complete-guide-to-dimensions-and-metrics-in-google-analytics/
[h5]: https://www.scirp.org/journal/Journalcitationdetails.aspx?JournalID=1573
[scielo-analytics]: https://analytics.scielo.org/
[editor-web]: https://ckeditor.com/ckeditor-4/
[html]: https://www.w3schools.com/html/
[docker]: https://www.docker.com/
[rede-scielo]: http://blog.scielo.org/blog/tag/rede-scielo/#.Wo_-2xPwZTY
[scielo-github]: https://github.com/scieloorg
