Este projeto contém os requisitos realizados por _[Scarlat Pereira](https://www.linkedin.com/in/scarlatpereira/)_ enquanto estudava na [Trybe](https://www.betrybe.com/) :rocket:

# Project Docker Todo List

Neste projeto criei soluções envolvendo os principais comandos e conceitos iniciais do SQL!

## Instalação do projeto localmente:

 Após cada um dos passos, haverá um exemplo do comando a ser digitado para fazer o que está sendo pedido, caso tenha dificuldades e o exemplo não seja suficiente, não hesite em me contatar em engcivil.scarlat@gmail.com

1. Abra o terminal e crie um diretório no local de sua preferência com o comando **mkdir**:
```javascript
  mkdir projetos
```

2. Entre no diretório que acabou de criar e depois clone o projeto:
```javascript
  cd projetos
  git clone git@github.com:scarlat-pereira/project-all-for-one-mysql.git
```

3. Acesse o diretório do projeto e depois utilize o comando **npm i** para instalar todas as dependências necessárias:
```javascript
  cd project-mysql-all-for-one
  npm i
```

- ✨ **Dica:** Caso queira utilizar _Docker_ para rodar os testes localmente e validar as queries criadas, basta executar o comando:
```javascript
docker run -p 3306:3306 --name mysql_57 -e MYSQL_ROOT_PASSWORD=1234 -d mysql:5.7 mysqld --default-authentication-plugin=mysql_native_password
```
- Depois de usar o comando acima, agora basta executar os testes digitando no terminal:
```javascript
MYSQL_USER=root MYSQL_PASSWORD=1234 HOSTNAME=localhost npm test
```

## Habilidades Desenvolvidas

Neste projeto, desenvolvi as seguintes habilidades:

 - Entender o que são bancos de dados;
 - Entender como a linguagem de consulta estruturada (SQL) é usada;
 - Compreender como as tabelas se encaixam no conceito de banco de dados;
 - Montar um ambiente de desenvolvimento local para praticar SQL;
 - Entender como usar o MySQL Workbench;
 - Compreender o que é uma query SQL e quais são seus tipos de comando;
 - Gerar valores com SELECT;
 - Selecionar colunas individualmente com SELECT;
 - Renomear e gerar colunas em uma consulta com AS;
 - Concatenar colunas e valores com CONCAT;
 - Remover dados duplicados em uma consulta com DISTINCT;
 - Contar a quantidade de resultados em uma consulta com COUNT;
 - Limitar a quantidade de resultados em uma consulta com LIMIT;
 - Pular resultados em uma consulta com OFFSET;
 - Ordernar os resultados de uma consulta com ORDER BY;
 - Filtrar resultados de consultas com o WHERE;
 - Utilizar operadores booleanos e relacionais em consultas;
 - Criar consultas mais dinâmicas e maleáveis com LIKE;
 - Fazer consultas que englobam uma faixa de resultados com IN e BETWEEN;
 - Encontrar e separar resultados que incluem datas;
 - Inserir dados em tabelas com INSERT;
 - Atualizar dados em tabelas com UPDATE;
 - Apagar dados em tabelas com DELETE.
 
 ## Escopo do Projeto
 
 **Desafios Iniciais**
 - Exiba apenas os nomes dos produtos na tabela products.
 - Exiba os dados de todas as colunas da tabela products.
 - Escreva uma query que exiba os valores da coluna que representa a primary key da tabela products.
 - Conte quantos registros existem na coluna product_name da tabela products.
 - Monte uma query que exiba os dados da tabela products a partir do quarto registro até o décimo terceiro.
 - Exiba os dados das colunas product_name e id da tabela products de maneira que os resultados estejam em ordem alfabética dos nomes.
 - Mostre apenas os ids dos 5 últimos registros da tabela products (a ordernação deve ser baseada na coluna id).
 - Faça uma consulta que retorne três colunas, respectivamente, com os nomes 'A', 'Trybe' e 'eh', e com valores referentes a soma de '5 + 6', a string 'de', a soma de '2 + 8'.
 
 **Desafios sobre filtragem de dados**
 - Mostre todos os dados da tabela purchase_orders em ordem decrescente, ordenados por created_by em que o created_by é maior ou igual a 3.
 - Exiba os dados da coluna notes da tabela purchase_orders em que seu valor de Purchase generated based on Order é maior ou igual a 30 e menor ou igual a 39.
 - Mostre as submitted_date de purchase_orders em que a submitted_date é do dia 26 de abril de 2006.
 - Mostre o supplier_id das purchase_orders em que o supplier_id seja 1 ou 3.
 - Mostre os resultados da coluna supplier_id da tabela purchase_orders em que o supplier_id seja maior ou igual a 1 e menor ou igual 3.
 - Mostre somente as horas (sem os minutos e os segundos) da coluna submitted_date de todos registros da tabela purchase_orders.
 - Exiba a submitted_date das purchase_orders que estão entre 2006-01-26 00:00:00 e 2006-03-31 23:59:59.
 - Mostre os registros das colunas id e supplier_id das purchase_orders em que os supplier_id sejam tanto 1, ou 3, ou 5, ou 7.
 - Mostre todos os registros de purchase_orders que tem o supplier_id igual a 3 e status_id igual a 2.
 - Mostre a quantidade de pedidos que foram feitos na tabela orders pelo employee_id igual a 5 ou 6, e que foram enviados através do método(coluna) shipper_id igual a 2.
 
 **Desafios de manipulação de tabelas**
 - Adicione à tabela order_details um registro com order_id: 69, product_id: 80, quantity: 15.0000, unit_price: 15.0000, discount: 0, status_id: 2, date_allocated: NULL, purchase_order_id: NULL e inventory_id: 129.
 - Adicione com um único INSERT, duas linhas à tabela order_details com os mesmos dados do requisito 20.
 - Atualize os dados de discount do order_details para 15. (Não é necessário utilizar o SAFE UPDATE em sua query).
 - Atualize os dados da coluna discount da tabela order_details para 30, onde o valor na coluna unit_price seja menor que 10.0000.
 - Atualize os dados da coluna discount da tabela order_details para 45, onde o valor na coluna unit_price seja maior que 10.0000 e o id seja um número entre 30 e 40.
 - Delete todos os dados em que a unit_price da tabela order_details seja menor que 10.0000.
 - Delete todos os dados em que a unit_price da tabela order_details seja maior que 10.0000.
 - Delete todos os dados da tabela order_details.
