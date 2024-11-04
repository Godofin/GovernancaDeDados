# Governança de Dados: Conhecendo o Ciclos de Vida dos Dados

## Para que o Ciclo de Vida?

- Importância de estudar o ciclo de vida dos dados.
- Diferentes etapas com características e preocupações específicas.
- Facilita a compreensão dos atores e capacidades envolvidos em cada etapa.
- Desenvolve uma visão sistêmica, mesmo para quem foca em uma única etapa.
- Melhora a percepção dos atores sobre todas as etapas do ciclo.
- Enfatiza a contribuição de cada trabalho para a gestão do ciclo de vida dos dados.
- A gestão abrange desde a coleta até o descarte dos dados.

## Características Fundamentais

- Dados são coletanea de registros, sendo físicos(Revistas) ou digitais(Bases de Dados)
- **Dados como ativos**: 
  - Dados são ativos valiosos para organizações.
  - Diferente de ativos consumíveis (como dinheiro ou petróleo), dados podem ser reutilizados.
  - Essa reutilização permite que os dados tenham um ciclo de vida, passando por diferentes etapas sem serem consumidos.

- **Contextualidade dos dados**:
  - Dados são sempre dependentes do contexto.
  - O significado dos dados muda com o contexto em que são apresentados.
  - Contextualidade é essencial para interpretar e extrair valor dos dados.

- **Temporalidade dos dados**:
  - Dados têm uma forte relação com o tempo.
  - Valor dos dados depende de estarem disponíveis no momento necessário.
  - Relevância dos dados varia com o recorte temporal.
  - Compreensão dessas características é crucial para estudar o ciclo de vida dos dados.

## O Ciclo de Vida

### Coleta
- **Atores na coleta**:
  - Demandante: quem solicita os dados, seja uma pessoa ou sistema.
  - Governança de dados: assegura o papel de regulação na coleta.

- **Departamentos envolvidos**:
  - Engenharia de dados: cria pipelines para coleta.
  - Modelagem de dados: preocupa-se com a representação visual e computacional dos dados.

- **Competências**:
  - ETL (Extrair, Transformar, Carregar) e ELT (Extrair, Carregar, Transformar) como principais métodos de coleta automatizada.

- **Perguntas cruciais na coleta**:
  - Quais dados são necessários?
  - Como os dados serão coletados?
  - Existe direito ou permissão para coletar esses dados?

- **Governança de dados**:
  - Define a legalidade e regulamentação interna/externa na coleta de dados.

- **Conclusão**:
  - Coleta é a primeira etapa do ciclo de vida dos dados.
 
### Coleta

- **Armazenamento de dados coletados (áudio como exemplo)**:
  - Armazenar os dados em uma pasta é uma solução inicial.
  - Consideração de formas mais eficientes de armazenamento.

- **Atores envolvidos**:
  - Responsáveis por armazenar e garantir a segurança da informação.
  - Governança de dados.
  - Responsabilidades variam conforme o ambiente (nuvem ou on-premises).

- **Departamentos**:
  - Engenharia de dados, Modelagem de dados, Segurança da informação, Arquitetura de dados.
  - Colaboração entre departamentos para garantir segurança e eficiência no armazenamento.

- **Competências necessárias**:
  - Manter os dados seguros.
  - Escolher a infraestrutura correta para armazenamento.

- **Perguntas cruciais**:
  - Qual é o tipo de dado a ser armazenado?
  - Quais são as opções de armazenamento adequadas?
  - Usar banco de dados relacional ou não relacional?
  - Estrutura física e lógica dos dados.
  - Custo e riscos do armazenamento.
  - Facilidade de busca e acesso futuro.

- **Riscos de armazenamento**:
  - Avaliar riscos associados ao tipo de dados, especialmente dados sensíveis.

- **Conclusão**:
  - Importância de considerar segurança, eficiência e acessibilidade ao planejar o armazenamento de dados
  
### Recuperação

- **Recuperação de dados**:
  - Terceira etapa do ciclo de vida dos dados.
  - Exemplo simples: recuperar dados armazenados no próprio computador.
  - Exemplo complexo: acessar dados de outro departamento (e.g., marketing acessando dados de vendas).

- **Considerações na recuperação**:
  - Localizar se o dado existe.
  - Verificar se há direito de acesso ao dado.

- **Atores envolvidos**:
  - Interessado no dado (quem solicita).
  - Anuente do dado (owner, que concede ou nega acesso).
  - Governança de dados: mediação entre interessado e owner.

- **Departamentos envolvidos**:
  - Departamento que detém o dado.
  - Departamento que solicita o dado.

- **Competências necessárias**:
  - Técnicas de extração: via API, SQL, ou outras linguagens.
  - Possibilidade de duplicar dados para acesso indireto.

- **Perguntas importantes**:
  - Quais dados serão recuperados?
  - O acesso será direto ou indireto?
  - É necessário replicar os dados?
  - Quem poderá acessar os dados?
  - Acesso será pontual ou contínuo?
  - Finalidade do acesso (conformidade com LGPD).
  - Tempo de acesso permitido.
  - Riscos associados à recuperação dos dados.

- **Conclusão**:
  - Fase crucial do ciclo de vida, com muitos fatores a considerar, embora nem sempre seja destacada em todas as versões do ciclo de vida dos dados.
 
### Uso
- **Uso de dados**:
  - Fase com ampla variedade de atores: analistas de dados, cientistas de dados, analistas de negócio, pesquisadores, entre outros.
  - Departamentos diversos, dependendo de quem extrai valor dos dados.

- **Competências necessárias**:
  - Conhecimento técnico para transformar dados em formato usável.
  - Capacidade de responder questões de negócio utilizando os dados.
  - Habilidade de trabalhar em tempo hábil para garantir relevância.

- **Perguntas importantes**:
  - Qual é o objetivo do uso dos dados?
  - Quais insights esperamos extrair?
  - Os dados por si só são suficientes ou precisam ser combinados com outras fontes?
  - O uso pretendido é ético?

- **Considerações éticas e de eficiência**:
  - Garantir alinhamento com princípios éticos e padrões organizacionais.
  - Entregas devem ser feitas dentro de prazos razoáveis para manter a relevância.

- **Conclusão**:
  - Passamos pelos principais pontos a considerar no uso dos dados, que não é a última fase do ciclo de vida.

### Descarte
- **Competência crucial no descarte de dados**:
  - Capacidade de excluir completamente os dados necessários.
  - Garantir que os dados não existam mais na organização.

- **Desafios no descarte de dados**:
  - Excluir apenas determinados períodos ou todos os dados.
  - Garantir a exclusão de todas as cópias do dado na instituição.
  - Verificar se algum processo depende do dado a ser excluído, para evitar falhas.

- **Complexidade do processo**:
  - Identificar e expurgar todas as cópias de um dado.
  - Notificar usuários e owners sobre a exclusão iminente dos dados.
  - Redefinir processos para evitar dependências críticas de dados a serem descartados.

- **Conclusão**:
  - Ciclo de vida dos dados concluído: coleta, armazenamento, recuperação, uso e descarte.
  - Próximos vídeos mostrarão um exemplo prático do ciclo completo de um dado.
 
## Benefícios do ciclo de vida dos dados

- Qualidade dos dados é tratada em várias etapas do ciclo de vida.
- Sendo:

### Melhoria no Controle de Custos
- **Controle de custos no ciclo de vida dos dados**:
  - Dados inativos e desatualizados podem aumentar custos sem gerar valor.
  - Armazenamento, embora barato, gera custos contínuos, especialmente para dados sem uso.

- **Descarte de dados**:
  - Descarte é crucial para reduzir custos e aumentar eficiência.
  - Dados que não são mais usados ou atualizados são candidatos ao descarte.

- **Otimização de armazenamento**:
  - Mover dados para armazenamento mais barato com maior latência pode reduzir custos.
  - Dados acessados com menor frequência podem ser armazenados em soluções mais econômicas.

- **Desafios de dados antigos**:
  - Dados acumulados ao longo dos anos podem gerar ineficiências.
  - Necessidade de gerenciar ativamente o ciclo de vida para evitar custos excessivos.

- **Conclusão**:
  - Usar o ciclo de vida dos dados ajuda a controlar custos e gerir ativos de dados de forma eficiente, contribuindo para a sustentabilidade financeira da organização.

### Melhoria na Usabilidade dos Dados
- **Usabilidade no ciclo de vida dos dados**:
  - Melhor qualidade dos dados reduz o tempo necessário para identificar e corrigir problemas.
  - Dados com qualidade adequada são mais rapidamente utilizáveis para modelos de Machine Learning e IA.

- **Benefício prático**:
  - Exemplo: localizar dados específicos, como de sapatilhas de atletismo, pode ser desafiador.
  - Governança de dados facilita a usabilidade com boas descrições e tags.

- **Tags e descrições**:
  - Tags automáticas podem ser geradas na fase de coleta.
  - Usuários experientes podem adicionar tags úteis durante a fase de uso.

- **Facilidade de localização e uso**:
  - Tags como "Equipamentos esportivos" e "Equipamentos de atletismo" facilitam encontrar dados.
  - Dados encontrados rapidamente e com boa qualidade aumentam a eficiência no uso.

- **Conclusão**:
  - Usabilidade melhora com dados acessíveis e de alta qualidade.
  - Ciclo de vida dos dados traz ganhos significativos em eficiência e qualidade no uso dos dados.

### Conformidade e Accountability
- **Relação entre ciclo de vida dos dados e governança de dados**:
  - Governança visa atingir conformidade com legislações e regulações específicas.
  - Ciclo de vida dos dados estabelece etapas e responsabilidades claras, auxiliando na conformidade.

- **Conformidade e segurança**:
  - Exemplo de segurança: um hacker precisa solicitar acesso ao owner da base de dados, que pode negar o acesso.
  - Etapas do ciclo de vida ajudam a prevenir e identificar problemas de segurança.

- **Accountability e rastreabilidade**:
  - Identificação de erros e brechas através da rastreabilidade.
  - Foco na melhoria contínua: entender, mitigar e prevenir erros futuros.

- **Medidas corretivas**:
  - Melhor treinamento para responsáveis pelos dados.
  - Substituição de responsáveis quando necessário.
  - Reforço de medidas de segurança para acesso aos dados.

- **Conclusão**:
  - Ciclo de vida dos dados apoia os objetivos da governança, como conformidade e segurança.

## Good/Smart Data

- **Cenário sem o ciclo de vida**:
  - Processo demorado para localizar dados.
  - Múltiplas consultas a diferentes bases.
  - Correção de problemas de qualidade antes do uso.
  - Ineficiência e tempo gasto antes de extrair valor dos dados.

- **Cenário com o ciclo de vida**:
  - Dados facilmente localizados usando tags.
  - Garantia de qualidade já tratada em várias etapas.
  - Acesso facilitado ao solicitar ao owner.
  - Processo mais rápido e eficiente para extrair valor dos dados.

- **Impacto do Good Data**:
  - Transição de Big Data (grande volume, variedade e velocidade) para Good Data (eficiência e qualidade).
  - Facilidade e eficiência no uso dos dados.
  - Boa infraestrutura e cultura organizacional são fundamentais.

- **Características do Good Data**:
  1. **Qualidade dos dados**: Essencial para eficiência e rapidez no uso.
  2. **Facilidade de localização**: Base de dados deve ser facilmente encontrada, auxiliada por metadados de qualidade, como descrições e tags.
  3. **Facilidade de acesso**: Dados devem ser acessíveis para pessoas com finalidades legítimas, com metadados claros para identificar proprietários e ferramentas eficientes para comunicação.

- **Facilidade na interpretação**:
  - Dados devem ser fáceis de interpretar após encontrados.
  - **Ferramentas e métodos**:
    - Perfis estatísticos (profiles) ajudam a entender comportamento e tipo de dados.
    - **Data stewards**: especialistas que auxiliam na compreensão técnica ou de negócio.
    - Colaboração com usuários experientes para validar interpretações.
  
- **Interoperabilidade**:
  - Capacidade de trabalhar facilmente com dados de diferentes bases.
  - Exemplos de bases: comportamento de compra, informações de clientes, vendas e pedidos.
  - Uso de **IDs únicos** para integrar dados de várias tabelas.
  - Depende de:
    - Qualidade dos dados e metadados.
    - Padronização na arquitetura de dados (nomes de IDs, estruturação, modelagem).

- **Relembrando as cinco características do Good/Smart Data**:
  1. **Qualidade dos dados**: Precisos e refletem a realidade.
  2. **Facilmente encontrados**: Localização simplificada com metadados de qualidade.
  3. **Facilmente acessados**: Acesso eficiente a quem tem finalidade legítima.
  4. **Facilmente interpretáveis**: Apoio de perfis estatísticos, data stewards e colaboração.
  5. **Interoperabilidade**: Integração de dados facilitada por padrões e IDs únicos.

- **Conclusão**:
  - O objetivo do ciclo de vida dos dados é alcançar o estado de **Good/Smart Data**, onde dados são eficientes, úteis e próximos à extração de valor para o negócio.
