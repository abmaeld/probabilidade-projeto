# PROB
Trabalho de Probabilidade, 2018.2
Repositório para guardar o trabalho de probabilidade com Ivanovitch para a segunda unidade

Endereço para o Vídeo: 

Insights acerca da disciplina de Probabilidade (IMD0033) nos semestres 2016.2, 2017.1 & 2017.2

A principal ideia era a de analisar as diferentes turmas de Probabilidade ao longo dos semestres, checar a taxa de aprovação de cada uma delas, e tentar encontrar padrões para explicar comportamentos encontrados.

Bibliotecas: pandas, matplotlib.pyplot, seaborn e numpy

Inicialmente buscamos dados referentes às turmas, notas, disciplinas e discentes dos 3 demestres no banco de dados que nos é disponibilizado pela UFRN. Armazenamos todas estas informações em variáveis com os mesmos nomes. (turmas, notas, disciplinas e discentes)

São realizadas então alterações no dataframe para facilitar(e permitir) a utilização dos dfs em merges.

Fazemos então um merge entre os dados dar turmas e suas disciplinas, podemos à partir desse ponto saber qual turma exatamente é aquela, tendo em vista que anteriormente só tínhamos códigos. Esse merge é fundamental para permitir um melhor entendimento dos dados.

Os dataframes possuem dados de todas as turmas, então filtramos por somente turmas do IMD, e em seguida somente por turmas de probabilidade.

Novamente é feito um merge, dessa vez entre os dataframes turmas_imd e docentes, com a coluna id_servidor como base.

Definimos uma funcao para colocar uma flag nos alunos aprovados para que possamos fazer a contagem destes posteriormente e utilizarmos o dado em análises futuras.

Neste ponto a maioria dos dados estão tratados e prontos para serem utilizados em diversas análises(que explicamos em vídeo).
