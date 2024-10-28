# Governança de Dados e Privacidade dos Dados

## Identificando bases com dados pessoais

- Esse trabalho necessita de duas etapas
    - Entender quais bases contém registros sobre os usuários
    - Entender se os dados estão de acordo com a LGPD
- É possível analisarmos se os dados são pessoais ou não, utilizando a lib ```dataprofiler```
- Necessário a partir do PII, identificar os PII Diretos e Indiretos dentro das bases

## O que são Dados Pessoais?

- São dados de pessoais naturais;
- Dados que identificam ou permitem identificar uma pessoa;

### Entendendo o conceito de Personal Identifiable Information

1. A primeira é o PII direto, que é como o CPF: uma informação identifica uma pessoa. Um e-mail também pertence a uma pessoa, então novamente temos uma identificação direta;
2. A segunda é o PII indireto, como o caso do RH comentado anteriormente, em que uma série de informações e do contexto permitem identificar exatamente uma pessoa. Vários dados levam para uma única pessoa; logo, esses dados também são dados pessoais.

## Pilares da LGPD

### Titularidade
- Quem tem escolha sobre o que pode ou não ocorrer com o dado é o : **titular do dado**
- Titular do dado: Pessoa a quem o dado se refere (Clientes/Usuários);
- Controlador do dados: permissão momentânea de acesso para alguma finalidades (Corporações);
- ANPD: Identifica as empresas se elas estão respeitando os dados, realiza a fiscalização;

### Bases legais
- Motivadores e situações específicas onde a empresa poderá fazer uso dos dados pessoais para diversos tipos de usos

### Finalidade
- Para todo dado coletado, ele precisa ter uma finalidade;
- Exemplo, se somos uma empresa de ecommerce, precisamos dos dados do cliente para emissão de nota fiscal e envio de produtos, e não para outras finalidades;
