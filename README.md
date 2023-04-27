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