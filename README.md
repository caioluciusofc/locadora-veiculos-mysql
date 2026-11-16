Locadora de Veículos MySQL

Projeto acadêmico de modelagem de um banco de dados para uma locadora de veículos com várias sedes.

Estrutura do banco de dados

Tabela Finalidade

`sedes` Registra as unidades da locadora.
`classesCarro` Define as categorias dos veículos e o valor da diária.
`clientes` Armazena o cadastro dos clientes e os dados da CNH.
`carros` Registra os veículos, suas categorias, sedes de origem e localizações atuais.
`reservas` Vincula cada reserva a um cliente, um veículo e às sedes de retirada e devolução.

O modelo permite registrar a retirada de um veículo em uma sede e a devolução em outra. As chaves estrangeiras preservam os vínculos entre as tabelas, e as restrições `UNIQUE` evitam o cadastro repetido de placas e CPFs.

Como executar

1. Conecte-se a um servidor MySQL pelo MySQL Workbench.
2. Abra e execute o script [`locadora.sql`](locadora.sql) para criar o banco `db_locar` e suas cinco tabelas.
3. Execute `SHOW TABLES;` para conferir se as tabelas foram criadas. O script cria a estrutura do banco com as tabelas vazias.

Se você já tiver um banco `db_locar` com essas tabelas, use outro nome nas instruções `CREATE DATABASE` e `USE` para testar em um banco separado.
