# Garantindo Qualidade de Dados com Pydeequ

- **Qualidade de Dados como Sub-área da Governança de Dados**:
  - Faz parte das disciplinas da DAMA (Data Management Association).
  
- **Definição de Qualidade de Dados**:
  - Dados que representam fielmente a realidade.
  - Dados que estão disponíveis no momento necessário.

- **Problemas com Qualidade de Dados**:
  - Dados não representam a realidade:
    - Exemplo: vendas duplicadas que não ocorreram de fato.
  - Dados não estão disponíveis:
    - Exemplo: informações não consolidadas porque equipes ainda não finalizaram o registro nos bancos de dados.

- **Aspectos Importantes da Qualidade de Dados**:
  - Fidelidade à realidade.
  - Disponibilidade no momento necessário.
 
  - ### Resumo em tópicos:

- **Contexto e Problema Inicial**:
  - Discutido anteriormente a qualidade de dados e sua importância para o negócio.
  - Problema específico: vendas não correspondem ao relatório de faturamento mensal.

- **Pergunta Central**:
  - Quem é responsável pela qualidade dos dados dentro da organização?

- **Responsabilidade pela Qualidade de Dados**:
  - Não é responsabilidade de uma única área, mas de uma **tríade**:
    1. **Governança de Dados**:
       - Área com mais conhecimento sobre qualidade de dados.
       - Define processos, ferramentas e regras necessárias.
    2. **Entidade Proprietária dos Dados**:
       - Detém o conhecimento de negócio para criar boas regras de qualidade.
       - Exemplo: regras de negócio específicas como o DDD da compra por telefone.
    3. **Usuários dos Dados**:
       - Interessados diretos na qualidade, pois impacta diretamente nas análises.
       - Contribuem com regras práticas baseadas no uso cotidiano.

- **Exemplo Prático**:
  - Diretores de vendas conhecem bem os canais e podem sugerir regras, como:
    - Inclusão de coluna com o canal de venda.
    - Garantia de que a coluna de canal nunca esteja vazia.

- **Benefícios de Regras de Qualidade**:
  - Reduzem o tempo gasto na resolução de problemas.
  - Tornam o processo de análise mais eficiente.
 
## Framework FMI

- **Introdução ao Tema**:
  - Qualidade de dados é uma preocupação antiga, com soluções desde os anos 2000.
  - O Framework do FMI é uma dessas soluções, focado em princípios para garantir qualidade de dados.

- **Objetivo do Framework**:
  - Auxiliar na validação e qualidade de bases de dados, como uma de balança comercial do Brasil.
  - Estabelecer princípios fundamentais para alcançar a qualidade.

- **Princípios do Framework do FMI**:
  1. **Pré-requisitos de Qualidade**:
     - Ambiente legal e institucional:
       - Exemplo: LGPD para dados pessoais.
     - Necessidade de recursos e investimentos:
       - Ferramentas, profissionais capacitados e áreas como governança de dados.
     - Foco nos dados mais relevantes:
       - Garantir que esforços e custos sejam direcionados para dados estratégicos.

  2. **Garantias de Integridade**:
     - **Profissionalismo**:
       - Processos claros e bem definidos na coleta e transformação dos dados.
     - **Transparência**:  
       - Abertura em relação aos métodos e processos.
     - **Ética no uso dos dados**:
       - Respeito às normas e boas práticas organizacionais.
      
### Metodologia do FMI

#### **Solidez Metodológica**:
- Foco nos métodos para selecionar e validar ativos de dados que gerem valor para a organização.
- **Princípios principais**:
  1. **Conceitos e definições**:
     - Definir claramente os nomes de colunas e informações, facilitando o entendimento para outros usuários.
  2. **Escopo do projeto**:
     - Escopo bem definido é essencial para garantir valor no final do processo.
  3. **Classificação e setorização**:
     - Identificar quais partes da organização serão mais interessadas nos dados disponibilizados.
  4. **Tratamento de vieses**:
     - Prevenir e corrigir influências preconcebidas para garantir fidelidade e ética nos dados.

#### **Precisão e Confiabilidade**:
- **Objetivo**: Garantir que os processos sejam transparentes, corretos e produzam dados confiáveis para a tomada de decisão.
- **Princípios importantes**:
  1. **Manutenibilidade**:
     - Processos devem ser fáceis de manter e atualizar, caso necessário.
     - Analogias com engenharia de software:
       - Código/documentação deve ser claro para facilitar modificações futuras.
  2. **Processos bem definidos**:
     - Coleta e tratamento devem ser documentados e confiáveis.

#### **Acessibilidade**:
- **Foco**: Tornar os dados compreensíveis e acessíveis para os interessados.
- Exemplos de boas práticas:
  - Usar a língua predominante da organização para facilitar a interpretação (evitar termos em inglês quando o ambiente usa português).
- Benefício: Aumentar a acessibilidade e utilidade dos dados para um público mais amplo.

## Framework DAMA

#### **Framework DAMA: Dimensões de Qualidade de Dados**:
- Avalia a qualidade dos dados através de **seis dimensões**.
- Dados de qualidade atendem **todas as dimensões**.

#### **Introdução e Aplicação Prática**:
- Cenário utilizado: Diretora de vendas de uma empresa de distribuição de filmes.
- Cada dimensão pode ser traduzida em **regras específicas** para garantir a qualidade.

#### **Dimensão da Acurácia**:
- Avalia quão próximos os dados estão da **realidade material**.
- **Exemplo prático**:
  - Base de dados informa que o filme *Titanic* dura 132 minutos.
  - Cronometragem real revela 145 minutos.
  - Conclusão: Problema de acurácia, pois os dados não refletem a realidade.

#### **Dimensões do Framework DAMA**:
O framework DAMA apresenta **seis dimensões de qualidade de dados**, cada uma com foco específico na avaliação da qualidade:

1. **Acurácia**:
   - Mede a proximidade dos dados com a **realidade material**.
   - Exemplo: Informações incorretas sobre a duração de um filme (Titanic dura 132 minutos na base, mas 145 na realidade).

2. **Completude**:
   - Avalia se os dados estão **completos ou faltando informações**.
   - Exemplo:
     - Base de dados com 100 filmes e 9 sem a pessoa diretora registrada = 91% de completude.
     - Regras podem exigir 100% de completude, dependendo da necessidade.
   - Pode ser analisada em todo o dataset ou em colunas específicas.

3. **Consistência**:
   - Verifica se os dados são **coerentes ao longo do tempo** ou em relação ao banco de dados como um todo.
   - Exemplo:
     - Filmes iranianos com média de 240 minutos (4 horas) destoam dos dados prévios, indicando possível erro.
     - Consistência ajuda a validar se os dados seguem padrões esperados.

4. **Unicidade**:
   - Garante que **dados únicos permaneçam únicos**.
   - Exemplo:
     - IDs duplicados para filmes em um catálogo representam um problema de unicidade.

5. **Validade**:
   - Verifica se os dados estão **dentro de limites e valores aceitáveis**.
   - Exemplo:
     - Um filme não pode ter 0 atores (inválido).
     - Dados fora da realidade, como um filme com 8 bilhões de atores, também são inválidos.

#### **Dimensão da Temporalidade**:
- Avalia a **disponibilidade da informação no momento necessário**.
- Foco em dados que precisam estar disponíveis dentro de **prazos definidos**, especialmente em processos recorrentes.

#### **Exemplos de Problemas de Temporalidade**:
1. **Envio de dados para a Ancine**:
   - Prazo: Dia 5 de cada mês.
   - Se os dados não chegam até o prazo, não é possível enviá-los, causando problemas regulatórios.

2. **Recebimento de novos filmes das distribuidoras**:
   - Expectativa: Dados chegam todo terceiro dia útil do mês.
   - Falha no envio desses dados atrasa o processo de avaliação e inclusão de filmes no catálogo.

#### **Impacto da Temporalidade**:
- A ausência de dados dentro do prazo pode:
  - Comprometer o cumprimento de **requisitos legais e regulatórios**.
  - Atrasar **processos internos críticos**, como análise ou tomada de decisão.

#### **Conclusão**:
- Garantir a temporalidade significa assegurar que as informações estão **disponíveis no momento certo** para atender às demandas organizacionais e regulatórias.

#### **Aplicação das Dimensões**:
- **Criação de regras específicas**:
  - Regras como exigir completude de 100% ou limitar valores dentro de intervalos válidos.
- **Impacto na análise e decisões**:
  - Cada dimensão contribui para que os dados sejam confiáveis, consistentes e úteis para as análises organizacionais.
