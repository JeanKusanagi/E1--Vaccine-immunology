# E1-Vaccine-immunology
Trabalho final da disciplina Ciência e Visualização de Dados em Saúde.

Projeto - Estudo da evolução da cobertura vacinal coletiva para imunização e erradicação de doenças infecciosas.

Project - Stufy of the evolution of the collective vaccine coverage for immunization and eradication infectious diseases.


# Apresentação

O presente projeto foi originado no contexto das atividades da disciplina de pós-graduação Ciência e Visualização de Dados em Saúde, oferecida no primeiro semestre de 2021, na Unicamp.

    Incluir nome RA e foco de especialização de cada membro do grupo. Os grupos devem ter no máximo 5 integrantes e devem contar com pelo menos um aluno da área da saúde e um aluno de área afim à Computação (Ex.: Computação, Elétrica...)
    
Nome | RA | Especialização
----- | ----- | -----
Bruna Mezzari Carlos             | 235624 | Computação
Jean Antonio Ribeiro             | 265739 | Computação
Kellen Natalice Vilharva         | 235493 | Saúde
Roberto Junio de Almeida Candian | 214572 | Saúde
Tatiana Aparecida de Almeida     | | Computação

# Descrição Resumida do Projeto

    Descrição do tema do projeto, incluindo motivação e contexto gerador.
    
   <strong>Tema do projeto:</strong> Considerando a complexa interação do sistema imunológico com diversos patógenos, a utilização das vacinas para prevenir doenças infecciosas, representa um grande triunfo para a ciência. A imunização por meio das vacinas, permitiram redução significativa de incidência de doenças, além da erradicação de outras. O projeto visa entender como a cobertura vacinal no Brasil evoluiu ao longo das últimas décadas, e quais os efeitos dessa evolução nos níveis de controle de determinadas doenças.
   
   <strong>Motivação:</strong> O tipo de vacina mais comum é a utilização da versão atenuada do vírus ou bactéria, sendo que os primeiros indícios na história do uso desse tipo de imunização remontam ao século 10, na China. Nesta época a aplicação se dava de forma bem diferente da que conhecemos atualmente, e somente em 1798, pela experiência do cientista Edwar Jenner, que o termo "vacina" foi criado. Através da observação de que trabalhadores rurais que já tinham sido acometidos pela varíola bovina não eram contaminados pela variante que afetava humanos, Edwar Jenner realizou um experimento inoculando o vírus em uma criança de oito anos de idade. Dessa forma, foi possível atestar experimentalmente a eficácia desse procedimento para a imunização. A partir resultados satisfatórios consecutivos, o conceito da vacina foi reconhecido e generalizado para diversas doenças, sendo atualmente uma das principais e mais efetivas formas de imunização e prevenção de doenças no mundo.

Por meio da vacinação, a varíola, a poliomielite, o sarampo e a rubéola foram erradicadas nas últimas décadas no Brasil. Contudo, o sucesso das campanhas de vacinação pode ser uma das causas do surgimento de movimentos antivacina que podem levar a uma queda da cobertura vacinal. Adultos e possíveis idosos da na geração atual, que foram devidamente vacinados durante a infância, muitas vezes não tiveram contato com a realidade dessas doenças e acabam por não perceberem a importância da imunização. Apesar da baixa incidência, doenças como o sarampo ainda apresentam riscos para a sociedade, como ficou evidente após surtos durante os anos de 2018 e 2019 no Brasil e outros países. Além desses fatores, a pandemia do COVID-19 pode estar contribuindo para essa queda na cobertura de imunização, tendo em vista o risco de contrair o coronavírus SARS-CoV-2, pelas pessoas ficarem reclusas em casa, além de postos de vacinação com horários reduzidos ou até mesmo fechados durante o ano de 2020. Sendo assim, o país pode voltar a ser acometido por doenças imunopreveníveis que estavam controladas diante do comprometimento da cobertura vacinal. Portanto, a vacinação é um tema estratégico de extrema importância ao se tratar de saúde pública e bem estar da população, sendo uma das formas de prevenção mais segura e eficaz para redução da incidência de doenças contagiosas e também para o desafogamento dos sistemas de saúde.
   
   <strong>Contexto gerador:</strong> Percepção da diminuição da cobertura vacinal ao longo dos últimos anos, cuja causa pode estar associada aos movimentos antivacina e à pandemia gerada pelo SARS-CoV-2. 
    
# Vídeo do Projeto

    Link para vídeo de apresentação da proposta do projeto (máximo 3 minutos).



# Perguntas de Pesquisa

    Perguntas de pesquisa que o projeto pretende responder ou hipóteses a serem avaliadas, enunciadas de maneira objetiva e verificável.
    
Qual a porcentagem de crianças imunizadas, ao longo dos anos e regiões do Brasil? 

Qual a correlação entre incidência das doenças e a vacinação?

Como a pandemia do COVID-19 e movimentos antivacina podem ter afetado a taxa de imunização?

# Bases de Dados

    Elencar bases de dados candidatas a serem utilizadas no projeto.
    
|Database | Link|
|-----    | -----|
|Bigdata  | https://bigdata.icict.fiocruz.br |
|DATASUS  | http://tabnet.datasus.gov.br/cgi/dhdat.exe?bd_pni/cpnibr.def |    
|THE GLOBAL HEALTH OBSERVATORY | https://www.who.int/data/gho/data/themes/immunization |
        

# Metodologia

    Proposta de metodologia incluindo especificação de quais técnicas pretende-se explorar, tais como: aprendizagem de máquina, análise de redes, análise estatística, ou integração de uma ou mais técnicas. Para a primeira entrega, descreva de maneira mais genérica que tipo de abordagem seu grupo pretende realizar.
    
   O projeto será elaborado a partir do modelo CRISP-DM. Com a utilização de dados fornecidos pelas bases de dados, a modelagem será realizada por meio de gráficos, correlação entre os dados e séries temporais. Também serão utilizadas Árvore de Decisão e Métodos de Regressão para a predição de informações, ambas utilizando a linguagem de programação Python. 

# Ferramentas

    Ferramentas a serem utilizadas (com base na visão atual do grupo sobre o projeto).
    
   O projeto será elaborado com auxílio de gráficos, séries temporais e da linguagem de programação Python.
    
Ferramenta | Endereço na Web | Resumo descritivo e utilização
----- | ----- | -----
Google Colab | https://colab.research.google.com | Lista de células que podem conter textos explicativos ou códigos executáveis e suas respectivas saídas.
Matplotlib   | https://matplotlib.org            | Biblioteca do _Python_ para criação de gráficos e visualizações de dados.
Numpy        | https://numpy.org                 | Biblioteca do _Python_ orientada a operação de vetores e matrizes multidimensionais.
Pandas       | https://pandas.pydata.org         | Biblioteca do _Python_ orientada a manipulação e análise de dados.
Python 3.8.3 | https://www.python.org            | Linguagem de programação de propósito geral. Utilizada para a predição dos dados.


# Cronograma

    Proposta de cronograma. Procure estimar quantas semanas serão gastas para cada etapa do projeto.
    
Tarefas | março | abril | maio | junho | julho
----- | ----- | ----- | ----- | ----- | -----
Descrição inicial do projeto            | X |   |   |   |
Levantamento dos dados                  | X | X |   |   |
Análise dos dados                       |   |   | X |   |
Digitalização do projeto                |   |   | X | X | X
Entrega e apresentação final do projeto |   |   |   |   | X
