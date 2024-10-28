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
- Os tipos de base legais estão nesse [link](https://github.com/Godofin/GovernancaDeDados/blob/main/Tipos%20de%20Bases%20Legais%20da%20LGPD.md)

### Finalidade
- Para todo dado coletado, ele precisa ter uma finalidade;
- Exemplo, se somos uma empresa de ecommerce, precisamos dos dados do cliente para emissão de nota fiscal e envio de produtos, e não para outras finalidades;

## Privacy by Design

- Princípios:
    1. Privacidade Incorporada ao Design: A proteção de dados deve ser integrada à estrutura do sistema desde o início, considerando a privacidade em todas as etapas do desenvolvimento. No exemplo, isso significa definir desde já como os dados dos pacientes serão protegidos, aplicando criptografia e controles de acesso para manter a segurança.

    2. Soma Positiva e Não de Soma Zero: Assegura que investir em privacidade não significa comprometer a eficiência ou funcionalidade. Privacidade e inovação podem coexistir, garantindo que as soluções de proteção de dados beneficiem todas as partes envolvidas, sem prejuízo.

    3. Visibilidade e Transparência: As práticas de privacidade devem ser visíveis e compreensíveis para os usuários, promovendo transparência sobre as medidas de proteção e criando uma relação de confiança. A proteção de dados não deve ser um “segredo”, mas algo que fortalece a confiança entre o usuário e a empresa.

    4. Respeito pela Privacidade do Usuário: O uso dos dados deve respeitar a privacidade do usuário, aplicando o princípio da minimização de dados – coletando apenas o necessário e usando-os para os fins legítimos. Isso garante que o uso dos dados esteja sempre alinhado com as normas de proteção, como a LGPD, promovendo confiança e conformidade.
