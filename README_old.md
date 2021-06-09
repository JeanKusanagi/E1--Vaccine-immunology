# Vaccine-immunology
Trabalho final da disciplina Ciência e Visualização de Dados em Saúde.

<strong>Projeto</strong> - Estudo da evolução da cobertura vacinal para imunização e erradicação de doenças infecciosas.

<strong>Project</strong> - Study of the evolution of the vaccine coverage for immunization and eradication infectious diseases.


~~~
├── README.md          <- apresentação do projeto
│
├── data
│   ├── processed      <- dados finais usados para a modelagem
│   └── raw            <- dados originais sem modificações
│
├── notebooks          <- Jupyter notebooks
│
├── images             <- iamgens geradas durante o desenvolvimento do projeto
    └── README.md      <- instruções básicas de instalação/execução
~~~


# Apresentação

O presente projeto foi originado no contexto das atividades da disciplina de pós-graduação Ciência e Visualização de Dados em Saúde, oferecida no primeiro semestre de 2021, na Unicamp.

   
Nome | RA | Especialização
----- | ----- | -----
Bruna Mezzari Carlos             | 235624 | Física Médica
Jean Antonio Ribeiro             | 265739 | Computação
Kellen Natalice Vilharva         | 235493 | Saúde
Roberto Junio de Almeida Candian | 214572 | Saúde
Tatiana Aparecida de Almeida     | 229136 | Computação

# Descrição Resumida do Projeto

    
   <strong>Tema do projeto:</strong> Considerando a complexa interação do sistema imunológico com diversos patógenos, a utilização das vacinas para prevenir doenças infecciosas, representa um grande triunfo para a ciência. A imunização por meio das vacinas, permitiram redução significativa de incidência de doenças, além da erradicação de outras. O projeto visa entender como a cobertura vacinal no Brasil evoluiu ao longo das últimas décadas, e quais os possíveis fatores que podem estar associados a essa evolução.
   
   <strong>Motivação:</strong> O tipo de vacina mais comum é a utilização da versão atenuada do vírus ou bactéria, sendo que os primeiros indícios na história da utilização desse tipo de imunização remontam ao século 10, na China. Nesta época a aplicação se dava de forma bem diferente da que conhecemos atualmente, e somente em 1798, pela experiência do cientista Edwar Jenner, que o termo "vacina" foi criado. Por meio da observação de que trabalhadores rurais que já tinham sido acometidos pela varíola bovina não eram contaminados pela variante que afetava humanos, Edwar Jenner realizou um experimento inoculando o vírus em uma criança de oito anos de idade. Dessa forma, foi possível atestar experimentalmente a eficácia desse procedimento para a imunização. A partir de resultados satisfatórios consecutivos, o conceito da vacina foi reconhecido e generalizado para diversas doenças, sendo atualmente uma das principais e mais efetivas formas de imunização e prevenção de doenças no mundo.

Por meio da vacinação, doenças como a varíola, a poliomielite, o sarampo e a rubéola foram erradicadas nas últimas décadas no Brasil. Contudo, o sucesso das campanhas de vacinação pode ser uma das causas do surgimento de movimentos antivacina que podem levar a uma queda da cobertura vacinal. Adultos e possíveis idosos da geração atual, que foram devidamente vacinados durante a infância, muitas vezes não tiveram contato com a realidade dessas doenças e acabam por não perceberem a importância da imunização. Apesar da baixa incidência, doenças como o sarampo ainda apresentam riscos para a sociedade, como ficou evidente após surtos durante os anos de 2018 e 2019 no Brasil e em outros países. Além desses fatores, a pandemia do COVID-19 pode estar contribuindo para essa queda na cobertura de imunização, tendo em vista o risco de contrair o coronavírus SARS-CoV-2, pelas pessoas ficarem reclusas em casa, além de postos de vacinação com horários reduzidos ou até mesmo fechados durante o ano de 2020. Sendo assim, o país pode voltar a ser acometido por doenças imunopreveníveis que estavam controladas diante do comprometimento da cobertura vacinal. Portanto, a vacinação é um tema estratégico de extrema importância ao se tratar de saúde pública e bem estar da população, sendo uma das formas de prevenção mais seguras e eficazes para redução da incidência de doenças contagiosas além de reduzir a utilização do sistema de saúde.
   
   <strong>Contexto gerador:</strong> Percepção da diminuição da cobertura vacinal ao longo dos últimos anos, cuja causa pode estar associada a diversos fatores socias, econômicos e de saúde global.
   
   <strong>Key words:</strong> 1. cobetura vacinal 2. imunização
    
<!-- # Vídeo do Projeto

    Link para vídeo de apresentação da proposta do projeto (máximo 3 minutos).

   https://youtu.be/riO6BU0K5MU -->



# Perguntas de Pesquisa

 
Qual a cobertura vacinal das vacinas obrigatórias, ao longo dos anos e regiões do Brasil? 
Quais fatores regionais ou sociais podem estar associados ao aumento ou diminuição da cobertura vacinal?


# Bases de Dados e Evolução

### Bases Estudadas e Adotadas
    
Database | Endereço na Web|Resumo descritivo
----- | ----- | -----
|DATASUS  | http://tabnet.datasus.gov.br/cgi/dhdat.exe?bd_pni/cpnibr.def | Departamento de informática do Sistema Único de Saúde do Brasil, o Datasus administra informações de saúde e informações financeiras. |
<!--| Bigdata  | https://bigdata.icict.fiocruz.br | Lançada em 2016, a PCDaS é uma iniciativa do Laboratório de Informação em Saúde (Lis) e do Centro de Tecnologia da Informação e Comunicação em Saúde (Ctic), ambos do Instituto de Comunicação e Informação Científica e Tecnológica em Saúde (Icict) da Fundação Oswaldo Cruz (Fiocruz), em parceria com o Laboratório Nacional de Computação Científica (LNCC), tem como objetivo desenvolver e disponibilizar Plataforma de Ciência de Dados aplicada à Saúde pública e gratuita com utilização de ferramentas open source para armazenamento, gestão, análise e disseminação de grandes quantidades de dados de saúde e seus determinantes socioambientais para pesquisadores, docentes e discentes de instituições de ensino e pesquisa, bem como gestores governamentais. |-->
Todas as tabelas, armazenadas em arquivos 'csv', possuíam a mesma quantidade de valores em cada coluna, mesmo que seja o valor 0. Contudo, na última linha de cada tabela, possui um valor representando a soma total de todos os valores da respectiva coluna. As transformações e tratamentos necesssários para obter uma nova base de dados que possa ser manipulada, de forma que se possa obter informações úteis e, posteriomente, ser analisadas, foram:
   
   * Remoção de linhas com dados categóricos, no caso, somente a última linha de todas as tabelas foram retiradas. Nessa linha, havia as representações totais de cada coluna. No caso da última célula, na coluna de nome 'Ano', seu valor é do tipo string igual a 'Total'. O restante das células, para todas as tabelas, são do tipo numérico.
   * Alguns dos valores numéricos possuiam o caracter ',' e, por isso, foram trocados pelo caracter '.'. Essa abordagem foi realizada para que a biblioteca pandas pudesse ler os dados dos arquivos 'csv' e, em seguida, manipulá-los.
   * Para muitos imunizantes não haviam dados de todos os anos (1994-2020), pois a cobertura vacinal era 0. Foram considerados para as análises somente os imunizantes com nenhum ou poucos valores nulos. Para alguns anos e imunizantes, a cobertura vacinal é maior do que 100% (mais de 100% da população alvo estimada foi imunizada).

  Um formulário básico que deve ser capaz de orientar o leitor na estruturação de informações em etapas de entendimento dos dados são encontrados ([ver aqui](data/raw/vaccine-immunology/notatecnicaCobertura.pdf)) e ([ver aqui](data/raw/vaccine-immunology/info.txt)).
  
  A descrição de todas as operações realizadas, para reestruturação, e analíses realizadas durante o desenvolvimento deste projeto, podem ser conferidas no notebook gerador dos agrupamentos ([ver aqui](notebooks/E2_vaccine_immunology.ipynb)).
  
  Na análise exploratória inicial, foram feitos gráficos de correlação, boxplot e evolução temporal: 
   
   * Cobertura vacinal no Brasil 1994 - 2020:

   <figure>
	<img src="images/Cobertura vacinal no Brasil 1994 - 2020.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
   <figure>
	<img src="images/cobertura_br_evolucao.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
    
 
   * Cobertura BCG no Brasil 1994 - 2020:
   
   <figure>
	<img src="images/Cobertura BCG no Brasil 1994 - 2020.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   

   * Cobertura Poliomielite no Brasil 1994 - 2020:
   
   <figure>
	<img src="images/Cobertura Poliomielite no Brasil 1994 - 2020.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
   <figure>
	<img src="images/cobertura_polio_evolucao.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
   
   
   * Cobertura Hepatite B no Brasil 1994 - 2020:

   <figure>
	<img src="images/Cobertura Hepatite B no Brasil 1994 - 2020.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
   
   * Cobertura DTP no Brasil 1994 - 2016 (sem info no ano de 2003):

   <figure>
	<img src="images/Cobertura DTP no Brasil 1994 - 2016 (sem info no ano de 2003).png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
   



Database | Endereço na Web|Resumo descritivo
----- | ----- | -----
THE GLOBAL HEALTH OBSERVATORY | https://www.who.int/data/gho/data/themes/immunization | Iniciativa da Organização Mundial da Saúde para compartilhar dados sobre saúde global, incluindo estatísticas por país e informações sobre doenças específicas e medidas de saúde. O site da GHO é organizado em torno de temas. Para cada tema, as principais estatísticas são apresentadas na página da Web associada, e dados e relatórios mais detalhados estão disponíveis para download.
        
Com essa base de dados, foi possível obter os dados de cobertura vacinal de diversos imunizantes dos anos de 1980 a 2019. Foram pesquisados dados das vacinas BCG, Poliomielite, Hepatite B e DTP. A base fornece os dados por país, mas os datasets também possuem uma coluna indicando o continente ou macro-região global a qual o país pertence. Como o objetivo da análise era comparar o Brasil com índices gerais, escolhemos trabalhar com a média de cobertura entre continentes (países da Ásia e Oceania estavam divididos em regiões menores, então fizemos a média somente para Americas, África e Europa). Entre os dados escolhidos não haviam dados faltantes, e os valores de cobertura vacinal (porcentagem da população-alvo corretamente imunizada) variam de 1 a 100.

A análie exploratória foi feita de forma integrada com os dados do DATASUS (item Integração entre Bases)

    

Database | Endereço na Web|Resumo descritivo
----- | ----- | -----
HDR | http://hdr.undp.org/en/data | Dataset com compilado de dados obtidos de diversas fontes para desenvolvimento em termos de pesquisa e análise, debate econômico, opções de políticas e advocacy. Nessa base são fornecidas informações sobre saúde, economia, educação e índices como o idh de diversos países do mundo.

Com essa base de dados, foi possível obter indicadores sociais e de saúde do Brasil para diferentes anos. Muitos dos indicadores escolhidos não possuem registros em todos os anos considerados pela base de dados, ou possuem somente registros periódicos (a cada 5 anos). Dos possíveis indicadores que poderiam estar relacionados com a cobertura vacinal e que possuíam registros no período 1994-2019, escolhemos para analisar os seguintes:

 * IDH : medida de desenvolvimento humano, em especial nos setores de educação (education index), renda (PIB per capita) e longevidade (expectativa de vida). Varia entre 0 e 100, sendo 100 correspondente a um país bastante desenvolvido. 
 * Education index: leva em conta o número médio de anos escolares de pessoas com mais de 25 anos. Varia entre 0 e 1, sendo que um índice 1 indicaria que todos os adultos acima de 25 anos receberam 18 ou mais anos de educação formal.

A análie exploratória foi feita integrada com os dados do DATASUS (item Integração entre Bases)


### Integração entre Bases

 * Integração entre a base GLOBAL HEALTH OBSERVATORY e DATASUS: nessa etapa da análise, integramos as médias de cobertura vacinal dos continentes às coberturas vacinais do Brasil e regiões do Brasil (Sul, Norte, Sudeste, ...), criando datasets 'imuno_mundo_br' com todos os dados de 1994 a 2019. Como a cobertua vacinal na base de dados internacional assume valores de 1 a 100, os valores de cobertura acima de 100 oriundos da base Brasileira foram redefinidos como 100. Na análise exploratória inicial, foram feitos gráficos de correlação, boxplot e evolução temporal, como exemplificado a seguir

   <figure>
	<img src="images/cobertura_polio_mundo_box.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
   <figure>
	<img src="images/cobertura_polio_mundo_evolucao.png" alt="Doenças no Brasil", height="400" width="600">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
 * Integração entre a base HDR e DATASUS: nessa etapa da análise, integramos os índices IDH e Education Index (obtidos da base HDR) aos dados de número total de óbitos de crianças abaixo de 1 ano, expectativa de vida (em anos) e cobertura vacinal dos imunizantes BCG, Poliomielite, Hepatie B, DTP e Febre Amarela (obtidos do DATASUS) no período de 1994-2019. Na base HDR, as linhas representam os países e as colunas, os anos. Para manter a formatação utilizada dos demais dataframes, invertemos as matrizes de dados oriundas da HDR para o formato ano x país e, em sequência, selecionamos somente a coluna com os dados do Brasil. Na análise exploratória inicial, foram feitos gráficos de correlação e evolução temporal como exemplificado a seguir

   <figure>
	<img src="images/polio_indices.png" alt="Doenças no Brasil", height="400" width="600">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
      <figure>
	<img src="images/br_indices.png" alt="Doenças no Brasil", height="400" width="1200">
	<!--<figcaption>Legenda para a imagem impressionante</figcaption>-->
   </figure>
   
A descrição de todas as operações realizadas nesta etapa também podem ser conferidas no notebook gerador dos agrupamentos ([ver aqui](notebooks/E2_vaccine_immunology.ipynb)).   

# Metodologia

<!--    Proposta de metodologia incluindo especificação de quais técnicas pretende-se explorar, tais como: aprendizagem de máquina, análise de redes, análise estatística, ou integração de uma ou mais técnicas. Para a primeira entrega, descreva de maneira mais genérica que tipo de abordagem seu grupo pretende realizar. -->
    
   O projeto será elaborado a partir do modelo CRISP-DM. Com a utilização de dados fornecidos pelas bases de dados, a modelagem será realizada por meio de gráficos, correlação entre os dados e séries temporais. Também serão utilizadas Árvore de Decisão e Métodos de Regressão para a predição de informações, ambas utilizando a linguagem de programação Python.

# Ferramentas

   
   O projeto será elaborado com auxílio de gráficos, séries temporais e da linguagem de programação Python.
    
Ferramenta | Endereço na Web | Resumo descritivo e utilização
----- | ----- | -----
Google Colab 	 | https://colab.research.google.com | Lista de células que podem conter textos explicativos ou códigos executáveis e suas respectivas saídas.
Jupyter Notebook | https://jupyter.org/ | Documento que permite execução de rotinas usuais de programação e documentação de todo o processo de produção do código.
Matplotlib   	 | https://matplotlib.org            | Biblioteca do _Python_ para criação de gráficos e visualizações de dados.
Numpy        	 | https://numpy.org                 | Biblioteca do _Python_ orientada a operação de vetores e matrizes multidimensionais.
Pandas      	 | https://pandas.pydata.org         | Biblioteca do _Python_ orientada a manipulação e análise de dados.
Python 3.8.3 	 | https://www.python.org            | Linguagem de programação de propósito geral. Utilizada para a predição dos dados.


# Cronograma

    
Tarefas | março | abril | maio | junho | julho
----- | ----- | ----- | ----- | ----- | -----
Descrição inicial do projeto            | X |   |   |   |
Levantamento dos dados                  | X | X | X |   |
Análise dos dados                       |   | X | X |  |
Digitalização do projeto                |   |   | X | X | X
Entrega e apresentação final do projeto |   |   |   |   | X

# Referências

[1] **Brito WI, Souto FJD.** Universal hepatitis A vaccination in Brazil: analysis of vaccination coverage and incidence five years after program implementation. Revista Brasileira de Epidemiologia = Brazilian Journal of Epidemiology. 2020;23:e200073. DOI: 10.1590/1980-549720200073.