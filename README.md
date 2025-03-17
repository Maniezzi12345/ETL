# ETL Base de Dados para Venda de Jogos


Esse código em M (Power Query) realiza uma série de transformações em uma planilha Excel, configurando um processo de ETL (Extract, Transform, Load). Aqui está a explicação passo a passo das alterações feitas:

##Alterações feitas na Tabela 

- Carrega os dados de um arquivo Excel ....
- Extrai a aba chamada "SAP-EXTRACT".
- Define os tipos de dados de várias colunas, como texto, inteiro e qualquer outro tipo.
- Remove a coluna "Package Id".
- Exclui linhas onde o valor na coluna "Game" é null ou contém padrões como "---", "----" e "-----".
- Divide a coluna "Game" em duas novas colunas ("Game.1" e "Game.2") com base no delimitador "-".
- Renomeia as colunas para "Game Name" e "Game Console".
- Substitui códigos de região ("EN", "PT", "JP") pelos respectivos nomes completos: "English", "Portuguese" e "Japanese".
- Remove o caractere "$" e troca pontos por vírgulas na coluna "Preço Unit Price".
- Converte a coluna "Stock Quantity" para número inteiro.
- Converte a coluna "Preço Unit Price" para o tipo moeda.
- Cria uma nova coluna chamada "Multiplicação" para calcular o preço total, multiplicando o preço unitário (Preço Unit Price) pela 
  quantidade de estoque (Stock Quantity).
- Ajusta a ordem das colunas para uma sequência específica.
- Renomeia "Preço Unit Price" para "Unit Price" e "Multiplicação" para "Total Price".
- Remove o prefixo "Batch-" da coluna "Batch


##Base de Dados para tratamento
![image](https://github.com/user-attachments/assets/dbd0a332-e191-49ed-b838-0f4222f85740)


##Base de Dados Tratada
![image](https://github.com/user-attachments/assets/c1eea99d-884e-4fd7-b69e-e1f0e3e706aa)






