# aprovacao-ufrn
repositório para análise de quais as taxas de aprovação dos professores de determinado dpto.


# Como utilizar?

Os dados vêm do site http://dados.ufrn.br/ disponibilizados pela UFRN para análise interna, são necessários 4 fontes de dados diferentes da parte de Ensino: turmas, componentes curriculares presenciais, docentes e matrícula-componente .

turmas e matrícula-componente são atualizados semestralmente, portanto a cada semestre que deseja-se analizar adicionalmente é necessário baixar o seu dataset respectivo no site.

Ps: sempre com um atraso de 1 período letivo entre a adição de um novo semestre nos dados abertos portanto em 2021.1 os dados disponíveis ainda serão até 2020.1 .

O dataset de professores e de componentes devem ser alterados em código para o respectivo departamento que está sendo buscado. ( são inúmeros registros no dataset, então é necessário esta filtragem inicial ).

O notebook deverá rodar N vezes dependendo da quantidade N de semestres que está procurando checar a taxa de aprovação dos professores, portanto você irá exportar N csv's por semestre com seus resultados. ex: 20191_resultado.csv, 20202_resultado.csv ; sempre alterando os nomes dos arquivos exportados com o semestre.

O notebook só deverá rodar até a célula dos csv_export antes de realizar a análise, uma vez que todos os semestres estiverem reunidos, então só aí a última célula deverá ser rodada para plotagem dos gráficos mudando sempre a lista de 'names' que contêm os nomes dos professores do departamento.

c'est ça.