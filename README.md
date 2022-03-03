# Trabalho de Probabilidade, 2018.2

Repositório para guardar o trabalho de probabilidade com Ivanovitch para a terceira unidade do semestre 2018.2

Endereço para o Vídeo: https://youtu.be/Ix-5Gw2pcXs

Insights acerca da disciplina de Probabilidade (IMD0033) nos semestres 2016.2, 2017.1 & 2017.2

A ideia inicial foi de analisar as taxas de aprovações e reprovações na disciplina de probabilidade ofertadas pelo IMD no período de 2016.2 a 2017.2. Além disso, verificar qual a correlação dessas taxas de acordo com o semestre ofertado, com o turno e também com o professor(a) no qual foi ministrada, com o intuito de encontrar padrões ou discrepâncias nos percentuais coletados.  

Bibliotecas: pandas, matplotlib.pyplot, seaborn e numpy. 

Inicialmente buscamos dados referentes às turmas, notas, disciplinas, docentes e discentes dos semestres 2016.2, 2017.1 e 2017.2 no banco de dados que nos é disponibilizado pela UFRN. Armazenamos todas estas informações em variáveis com os mesmos nomes. (turmas, notas, disciplinas e discentes). 

Em seguida, fazemos as adaptações necessárias nos dataframes para que ele possa ser utilizado no merge. 

Depois, é feito o merge entre os dataframes turmas e disciplinas. Utilizamos como base a coluna id_componente(passo necessário pois as turmas estavam com IDs, dessa forma, não sabíamos de quais disciplinas se tratavam as turmas). 

Nosso novo dataframe possui dados referentes à todas as turmas, então filtramos, ficando somente com turmas consolidadas do IMD. 

Novamente é feito um merge, dessa vez entre os dataframes turmas_imd e docentes, com a coluna id_servidor como base. 

Uma vez mais, filtramos somente as turmas do IMD. 

Fazemos uma definição de aprovado, sendo estes, tanto os alunos aprovados, quanto os aprovados por nota, e atribuímos uma flag nos alunos aprovados em cada semestre. 

Em seguida, ainda separamos e tratamos os alunos que estão armazenados como Lato Sensu, Indeferidos, Cancelados ou Excluídos. 

Posteriormente, com as turmas do IMD filtradas, separamos somente as turmas de probabilidade de cada semestre e por fim, realizamos os cálculos da taxa de aprovação de cada um dos semestres, por horário e também pelo professor(a). 

Com os dados dos percentuais de aprovação tratados, utilizamos as bibliotecas matplotlib.pyplot e a seaborn para gerar gráficos referente ao objetivo inicial, que era a análise dos percentuais de aprovação, além de informação sobre realização da reposição de cada turma, com os insights explicados em vídeo. 
