# 7DaysCodeAlura-Python-Pandas
Desafio Alura - 7 Days of code


https://github.com/FranciscoFoz/7_Days_of_Code_Alura-Python-Pandas/tree/main/Dia_1-Importando_dados/Datasets

Links 
https://pandas.pydata.org/docs/user_guide/io.html
https://www.alura.com.br/artigos/arquivos-parquet
https://franciscofoz.medium.com/como-jogar-dados-fora-com-pandas-23a5be871aac

Dados baixados? Ok, mas são diversas tabelas diferentes e isso dificulta o trabalho. Portanto, o seu primeiro passo é unificar em um único Dataframe todos os dados pertinentes para a análise.

Comece pelos empréstimos e você terá os dados das transações. Depois, mescle com os dados do acervo, para que você possa entender, por exemplo, de qual biblioteca era o material emprestado ou a qual tema ele se referia. Elas se relacionam pela coluna de código de barras de cada material.

Lembre-se que é muito comum receber dados nulos ou duplicados, por isso não deixe de fazer a limpeza.

Você deve ter visto que tem uma coluna identificada como “localização” e diversos números nela, mas você sabe o que significam estes números?

"Os itens do acervo em uma biblioteca são organizados por um sistema de classificação de acordo com o respectivo tema. Existem diversos sistemas, mas este conjunto está de acordo com a CDU - Classificação Decimal Universal. Esta classificação é decimal, pois varia de acordo com a classe de cada assunto:

    000 a 099: Generalidades. Ciência e conhecimento.
    100 a 199: Filosofia e psicologia.
    200 a 299: Religião.
    300 a 399: Ciências sociais.
    400 a 499: Classe vaga. Provisoriamente não ocupada.
    500 a 599: Matemática e ciências naturais.
    600 a 699: Ciências aplicadas.
    700 a 799: Belas artes.
    800 a 899: Linguagem. Língua. Linguística.
    900 a 999: Geografia. Biografia. História."


Portanto, se um material tiver um código de localização 720, ele está dentro da classe geral de “Belas Artes”; ou se tiver um código 028, estará dentro da classe geral de “Generalidades. Ciência e conhecimento”.

Para isso, crie uma nova coluna com os valores da localização, para refletir a respectiva classe geral na CDU.

Você precisará ainda excluir alguns dados e modificar outros.  

A coluna "registro_sistema", por exemplo, não está fazendo sentido para essa análise, por isso você pode exclui-la.
Já a coluna da matricula (“matricula_ou_siape”) não está com um formato muito legível. Transforme-a em formato String. 



https://www.alura.com.br/artigos/adicionando-elementos-na-lista-do-python-append-ou-extend



#Desafio dia 3
A diretoria da biblioteca gostaria de entender se a quantidade de empréstimos está diminuindo, aumentando ou permanecendo igual ao decorrer dos últimos anos.

Para isso, verifique qual é a quantidade total de exemplares emprestados por cada ano e plote um gráfico de linhas.

Depois, faça uma análise em relação à visualização gerada.

Atente-se para a quantidade de exemplares emprestados, e não de empréstimos realizados.

A diretoria também gostaria de gerenciar melhor os recursos humanos da biblioteca de acordo com a demanda de trabalho existente. Por exemplo:

    gerenciar a programação de férias dos colaboradores de acordo com os meses de menor demanda;
    programar atividades que não sejam de atendimento ao usuário para períodos específicos de menor demanda.


Há uma suspeita interna de que os meses com maior número de exemplares emprestados sejam março e setembro, mas não foi realizada uma análise real sobre isso.

Portanto, gere uma tabela com a quantidade total de exemplares emprestados por mês e descubra quais meses são os que possuem a maior quantidade de empréstimos realizados. Plote um gráfico de linhas.

Traga suas análises em relação a quais meses poderiam ser as melhores opções.

Além do gerenciamento anual das atividades, a diretoria também necessita que seja planejada uma programação diária das atividades. Por este motivo, verifique quais foram os horários com maior quantidade de empréstimos ao longo de um dia inteiro.

Plote um gráfico de barras e analise quais seriam os melhores horários para alocar as demais atividades que não sejam de atendimento ao usuário. 


https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.Series.dt.date.html
https://www.alura.com.br/artigos/lidando-com-datas-e-horarios-no-python
https://www.alura.com.br/artigos/visualizando-informacoes-com-um-grafico
https://www.alura.com.br/artigos/analise-de-dados-analisando-minha-distribuicao-com-tres-alternativas-de-visualizacao


dica

 Verifique a quantidade de empréstimos pelos números de ID. Investigue pela relação deles com o ID dos exemplares.

O groupby poderá te ajudar nesse desafio.
https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.groupby.html
Transforme as datas em tipo Datetime.

Não deixe de caprichar nos gráficos:

    coloque um título adequado e objetivo;
    escolha cores adequadas e acessíveis para todas as pessoas;
    deixe apenas as informações relevantes, o excesso prejudica a visualização.