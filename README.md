# Financial_Sample_Modelo
> Processo de Importação e Modelagem de Dados no Power BI

>>> Importei o arquivo Financial Sample.xls para o Power BI.

Criação da Tabela de Produtos (d_produtos)
Dupliquei a tabela original de produtos.
Removi as duplicatas.
Criei uma coluna índice id_produto, numerando de 1 a 6.
Criação da Tabela de Segmentos (d_segmento)

Dupliquei a tabela original de segmentos.
Removi as duplicatas.
Criei um índice id_segmento.
Criação da Tabela de Países (d_pais)

Dupliquei a tabela original de países.
Removi as duplicatas.
Criei um índice id_pais.

>>>Mesclagem de Tabelas

Mesclei a tabela f_vendas com d_produtos para incluir o id_produto.
Removi a coluna product da tabela f_vendas deixando ID
Mesclei a tabela f_vendas com d_segmento para incluir o id_segmento.
Removi a coluna segmento de f_vendas deixando ID
Mesclei a tabela f_vendas com d_pais para incluir o id_pais.
Removi a coluna pais de f_vendas deixando o ID


Desativei a carga da tabela bk_financials (original).

Criação da Tabela Calendário (d_calendario)

Criei a tabela d_calendario para facilitar a análise temporal.
Relacionamentos

Estabeleci os seguintes relacionamentos:
d_calendario (1) - (*) f_vendas
d_pais (1) - (*) f_vendas
d_segmento (1) - (*) f_vendas
d_produtos (1) - (*) f_vendas
