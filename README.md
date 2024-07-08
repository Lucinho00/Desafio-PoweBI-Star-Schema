# Desafio-PoweBI-Star-Schema

O que deve ser feito?

Criar a tabela Fato:
A tabela fato deve conter informações relevantes sobre o professor, incluindo:
ID do professor
ID do curso
ID do departamento
Data de oferta do curso
Número de cursos ministrados
Carga horária dos cursos
Avaliação dos cursos (caso disponível)
Criar as tabelas Dimensão:
Dimensão Professor:
ID do professor
Nome do professor
Título acadêmico
Tempo de casa
Especialidade
Dimensão Curso:
ID do curso
Nome do curso
Descrição do curso
Nível do curso (Graduação, Pós-Graduação)
Departamento responsável
Dimensão Departamento:
ID do departamento
Nome do departamento
Chefe do departamento
Localização
Dimensão Data:
Data (em diferentes granularidades, como dia, mês, ano)
Ano
Trimestre
Mês
Dia da semana
Semana do ano
Exemplo de Star Schema
Tabela Fato: Fact_Professor

ID_Professor	ID_Curso	ID_Departamento	Data_Oferta	Num_Cursos	Carga_Horária	Avaliação
1	101	10	2021-09-01	3	45	4.5
Tabela Dimensão: Dim_Professor

ID_Professor	Nome	Título	Tempo_Casa	Especialidade
1	João Silva	Doutor	10 anos	Engenharia de Dados
Tabela Dimensão: Dim_Curso

ID_Curso	Nome_Curso	Descrição	Nível	ID_Departamento
101	Análise de Dados	Curso de Análise...	Graduação	10
Tabela Dimensão: Dim_Departamento

ID_Departamento	Nome_Departamento	Chefe	Localização
10	Ciência da Computação	Dr. Maria Souza	Prédio Central, Sala 205
Tabela Dimensão: Dim_Data

Data	Ano	Trimestre	Mês	Dia	Dia_Semana	Semana_Ano
2021-09-01	2021	3º	Setembro	01	Quarta	36
Tarefas
Desenhar o diagrama Star Schema:

Use uma ferramenta de modelagem de dados, como Microsoft Visio, Lucidchart, ou até mesmo uma planilha de Excel/Google Sheets para desenhar o esquema estrela.
Conecte a tabela fato às suas dimensões com chaves estrangeiras.
Definir os campos da Tabela Dimensão de Datas:

Crie campos adicionais conforme necessário, considerando a granularidade de dados de oferta de cursos e outras necessidades analíticas.
Documentar:

Crie uma documentação breve explicando cada tabela, os campos selecionados e as relações entre as tabelas.
Entregáveis
Diagrama do esquema estrela.
Definições de cada tabela (fato e dimensões) com os campos.
Documentação explicativa.
