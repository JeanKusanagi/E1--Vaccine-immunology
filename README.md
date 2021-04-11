# E1-Vaccine-immunology
Trabalho final da disciplina Ciência e Visualização de Dados em Saúde.

Projeto - Estudo da resposta imunológica coletiva da vacinação para imunização e erradicação de doenças infecciosas.

Project - Mass immunological response study of vaccination for immunization and eradication infectious diseases.


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
    
   <strong>Tema do projeto:</strong> Considerando a complexa interação do sistema imunológico com diversos patógenos, a utilização das vacinas para prevenir doenças infecciosas, representa um grande triunfo para a ciência. A imunização por meio das vacinas, permitiram redução significativa de incidência de doenças, além da erradicação de outras.
   
   <strong>Motivação:</strong> O tipo de vacina mais comum é a utilização da versão atenuada do vírus ou bactéria. E os primeiros indícios na história do uso desse tipo de imunização foi no século 10, na China, embora à aplicação se dava de forma bem diferente, pois os chineses trituravam as cascas das feridas, nas quais continham os antígenos e assopravam o pó sobre a face do indíviduo. Somente em 1798, pela experiência do cientista Edwar Jenner que o termo "vacina" foi denominado. Através da observação que trabalhadores rurais não pegavam varíola, porque já tinham sido acometidos pela varíola bovina, uma cepa de menor virulência para os humanos. Ele realizou um experimento inoculando os dois vírus em uma criança de oito anos de idade. Dessa forma, atestou experimentalmente com resultado satisfatório, assim o termo "vacina" originou-se do nome científico do vírus varíola bovina <i>Variolae vaccinae</i> e atualmente tornou-se uma das principais formas de imunização e prevenção de doenças no mundo.

Por meio da vacinação, a varíola, a poliomielite, o sarampo e a rubéola foram erradicadas nos últimos anos. Contudo, o sucesso das campanhas de vacinação pode ser uma das causas da queda da cobertura. Com a população amplamente vacinada durante a infância, com passar dos anos essas crianças se tornaram pais e mães que não conviveram com essas doenças, assim na maioria das vezes não percebem a importância da imunização. Apesar da baixíssima incidência, as doenças ainda existem, sendo essencial vacinar as crianças. Além disso, a pandemia do COVID-19, pode estar contribuindo para essa queda na cobertura de imunização, tendo em vista o risco de contrair o coronavírus SARS-CoV-2, pelas pessoas ficarem reclusas em casa, além de postos de vacinação com horários reduzidos ou até mesmo fechados. Sendo assim, o país pode voltar a ser acometido por doenças imunopreveníveis que estavam controladas, pelo comprometimento da cobertura vacinal. Outro fator que pode compometer a taxa de vacinação são os movimentos antivacina, nos quais fomentam ideias de que as vacinas sejam prejudiciais para a população. Portanto, a vacinação é um tema estratégico se tratando de saúde pública e bem estar da população, sendo uma das formas de prevenção mais segura e eficaz para redução de incidência de doenças.
   
   <strong>Contexto gerador:</strong> Resposta da vacinação coletiva para imunização e erradicação de doenças.
    
# Vídeo do Projeto

    Link para vídeo de apresentação da proposta do projeto (máximo 3 minutos).



# Perguntas de Pesquisa

    Perguntas de pesquisa que o projeto pretende responder ou hipóteses a serem avaliadas, enunciadas de maneira objetiva e verificável.
    
Qual a porcentagem de crianças imunizadas, ao longo dos anos e regiões do Brasil? 

Qual a correlação entre incidência das doenças e a vacinação?

Como a pandemia do COVID-19 e movimentos antivacina podem afetar a taxa de imunização (%)?

# Bases de Dados

    Elencar bases de dados candidatas a serem utilizadas no projeto.
    
Database | Link
-----    | -----
Bigdata  | https://bigdata.icict.fiocruz.br

         | http://tabnet.datasus.gov.br/cgi/dhdat.exe?bd_pni/cpnibr.def       
DATASUS  | http://www2.datasus.gov.br/DATASUS/index.php?area=060702
         | http://pni.datasus.gov.br/            

WHO      | https://www.who.int/health-topics/vaccines-and-immunization#tab=tab_1
         | https://ourworldindata.org/vaccination

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
