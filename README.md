# Utilização de Views no Banco de Dados

Uma **VIEW** é uma tabela virtual ou uma consulta armazenada. Essa tabela virtual é criada através de um conjunto de resultados de uma consulta. Em vez de executar sempre uma query complexa, que pode consumir mais recursos do banco de dados, você cria uma **VIEW** com esse comando, onde uma tabela virtual é criada com o resultado dessa consulta.

## Vantagens de Usar uma VIEW

A principal vantagem de utilizar uma **VIEW** é que, ao invés de sempre rodar uma consulta complexa, você pode realizar um **SELECT** mais simples na **VIEW**, que já contém os dados armazenados na tabela virtual. Isso ajuda a otimizar o desempenho e reduzir o uso de recursos ao realizar consultas frequentes.

## Segurança no Banco de Dados

Além de otimizar o desempenho, uma **VIEW** também pode ser usada para implementar segurança em banco de dados. Você pode ocultar informações sensíveis de determinados grupos de usuários, permitindo que apenas dados específicos sejam acessados, conforme a necessidade.

## Características de uma VIEW

- **Não existe fisicamente**: Uma **VIEW** é considerada uma tabela virtual.
- **Limitações nas operações de atualização**: Há limitações em relação às operações de atualização que podem ser aplicadas.
- **Sem limitações nas consultas**: Não há limitações quanto às operações de consulta.
- **Tabelas definidoras de visão**: As tabelas utilizadas na definição de uma **VIEW** são chamadas de **tabelas definidoras de visão**.

## Exemplo de Criação de uma VIEW

```sql
CREATE VIEW nome_da_view AS
SELECT coluna1, coluna2
FROM tabela
WHERE condição;

