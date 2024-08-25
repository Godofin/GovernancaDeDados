# Governança De Dados

## Conceitos Fundamentais

### Conceito

- Origem no processo de dados: Envolve as etapas de coleta, organização e armazenamento de dados de forma estruturada e eficiente.
- Integração de processos, princípios e decisões: Combina processos bem definidos, princípios sólidos e decisões estratégicas para agregar valor e promover a eficiência organizacional.
- Processos + princípios + Decisões = Valores e eficicência
- Objetivos principais: Visa garantir a privacidade, qualidade, disponibilidade e segurança dos dados, assegurando conformidade com regulamentações e práticas recomendadas.
- Enfoque estratégico: Atua de forma estratégica na definição de políticas e diretrizes para o gerenciamento eficaz de dados, alinhando a governança aos objetivos de negócio.

### DAMA e a Roda de Disciplinas

- DAMA = Data MAnagement Association (Associação de Gestão de Dados)
- Segundo a DAMA, as disciplinas que compõem a governança de dados incluem:
    - Arquitetura de dados;
    - Modelagem de dados;
    - Operação e armazenamento;
    - Segurança de dados;
    - Integração e interoperabilidade;
    - Gestão de documentos e conteúdo;
    - Dados referências e dados mestres;
    - Business Intelligence e Data Warehousing;
    - Metadados;
    - Qualidade de dados;

- Visa sempre extrair valor e eficiência com os dados.

### Por que organizações se interessam em governança de dados?

- Existem 4 principais motivos:
  - Conformidade
  - Eficiência
  - Decisão orientada por dados (Data Driven Decisions)
  - Monetização

#### Conformidade

- **Regulamentações crescentes**: Países, tanto internacionalmente quanto nacionalmente, estão criando mais leis para regular o uso de dados.
- **Foco em dados pessoais**: As regulamentações, como a LGPD no Brasil e o Marco Civil da Internet, visam proteger dados pessoais.
- **Necessidade de conformidade**: Empresas precisam garantir que suas práticas estejam em conformidade com essas leis.
- **Investimento em governança**: A conformidade com a legislação é o principal motivo para empresas investirem em governança de dados.

#### Eficiência

- Redução de retrablho.
- Extração de dados com menos recursos.

#### Decisão orientada por dados

- Modelos de decisão que se baseia em dados.
- Confronta o modelo antigo que é o modelo de decisão tomado pela intuição.
- Importante garantir a qualidade, veracidade e integridade dos dados

#### Monetização

- Criação de produtos de dados para extração de valor.
- Venda de dados para outras empresas.

### Governança é uma responsabilidade mais ligada ao negócio ou tecnologia?

- Governança de dados deve ser um tema central da cultura das organizações
- Deve estar presente em todos os níveis empresariais:
    - Estratégico (Chief Data Officer)
    - Tático (Data Governance Officer)
    - Operacional (Engenheiros, cientistas, analistas, usuarios)
- Necessário ter o Data Literacy (Letramento de dados)

### 5 P's da Governança de Dados

#### Princípios
- Grande objetivos que norteiam as questões de governança
- Conhecimento dos ativos de dados: Conhecer as bases de dados da organização
- Acesso mínimo: Menor nível de acesso possível. Exemplo: Bases de RH, só pessoas do RH acessam

#### Processos
- Conjuntos de etapas adotadas pela organização para implementar os princípios
- Processo de ingestão de bases: Criação de modelos lógico, relacional, dicionário de dados e regras de qualidade

#### Procedimentos
- Maneiras específicas de realizar uma ação relacionada a dados
- Modelagem lógica: Time de modelage
- Dicionário de dados e Regras de qualidade: Time de negócios
- Modelo relacional: Engenharia de dados
- Pode-se utilizar a lib ```pydq``` para validar governança
  
#### Padrões
- Normas e especificações que tentam garantir a consistência nas ações de dados
- Definidos sempre externamente como COBIT, ITIL, Etc
  
#### Papéis
- Conjunto de responsabilidade atreladas a uma pessoa ou área, esses papéis incluem:
    - Data Owner:
          - Profissional de negócio
          - Responsável por tomar decisões
          - Precisar ter conhecimento sobre os dados
          - Responsável em definir quem acessa os dados e sobre sua qualidade
    - Data Stewards
          - Conhece os dados em profundidade e serve à organização com esse conhecimento
          - Business ou Technical Data Stewards
    - Data governance officer
          - Desenvolvimento de Políticas e Normas
          - Garantia da Qualidade dos Dados
          - Educação e Treinamento
          - Gerenciamento de Metadados
    - Usuário de dados
          - Cliente final de governança
          - Data literacy (Alfabetização de dados)
