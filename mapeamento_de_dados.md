# Mapeando a origem e o destino com linhagem de dados

## **Resumo sobre Linhagem de Dados**  

### **1. Contexto da Aplicação**  
- Empresa de avaliação de ativos financeiros que coleta e analisa dados para recomendar investimentos.  
- Para **Fundos de Investimento Imobiliário (FIIs)**, utiliza dados internos e externos.  
- Principais fontes de dados:  
  - **Preço por metro quadrado** nas cidades do Brasil.  
  - **Quantidade de compras e vendas de imóveis** (dados de cartórios).  
  - **Análises anteriores** da empresa sobre o ativo.  

### **2. Conceito de Linhagem de Dados**  
- Identifica e gerencia **as origens e as transformações** dos dados.  
- No contexto da empresa, há **três origens** de dados que são combinadas e transformadas para gerar uma recomendação de investimento.  
- A estrutura resultante forma uma **base consolidada** com a recomendação para diferentes perfis de investidores.  

### **3. Outro Nome para Linhagem de Dados**  
- Também chamada de **Data Provenance** (Proveniência dos Dados).  
- O conceito é essencial para entender a **trajetória e confiabilidade dos dados**.  

### **4. Importância da Linhagem de Dados**  
- **Garante transparência** sobre as fontes e alterações nos dados.  
- **Melhora a governança** e rastreabilidade das informações.  
- **Facilita a análise e auditoria**, permitindo compreender como um dado foi transformado até o formato final.

### **Resumo sobre Linhagem de Dados e Transformações**  

#### **1. Definição de Linhagem de Dados**  
- Disciplina da **governança de dados** que rastreia as **origens e transformações** dos dados.  
- Mostra como os dados são processados para gerar novos dados.  

#### **2. Representação por Equação**  
- A equação **V = Q(D)** ilustra a relação entre os dados e suas transformações:  
  - **V** representa a **visão (view)** resultante.  
  - **Q** representa as **queries e transformações** aplicadas.  
  - **D** representa os **dados originais**.  
- Exemplo prático:  
  - No **SQL**, visões são criadas com **JOINs, GROUP BYs, ORDER BYs e SELECTs**.  

#### **3. Aplicação na Avaliação de Ativos Financeiros**  
- Equação expandida: **V = Q1(D1) + Q2(D2) + Q3(D3)**  
  - **V**: Base final com recomendações sobre fundos imobiliários.  
  - **Q1(D1)**: Transformações sobre preços por metro quadrado.  
  - **Q2(D2)**: Transformações sobre compras e vendas de imóveis.  
  - **Q3(D3)**: Transformações sobre análises anteriores.  

#### **4. Importância da Representação**  
- Forma **visual e genérica** para entender linhagem de dados.  
- Permite rastrear **quais dados foram transformados**, sem detalhar cada etapa.  
- Aplicável a **qualquer processo** em que dados originais passam por modificações para gerar novas bases.

### **Resumo sobre Níveis de Especialização da Informação e Reusabilidade dos Dados**  

#### **1. Problema na Organização dos Dados**  
- Novas bases de dados são criadas sucessivamente para atender demandas específicas.  
- Isso pode dificultar a organização e rastreabilidade dos dados.  
- A **linhagem de dados** ajuda a organizar e extrair valor da informação.  

#### **2. Níveis de Especialização da Informação**  
- **Source of Records (SOR) - Fonte de Registros:**  
  - Contém **todos os dados brutos**, sem transformação.  
  - Inclui clientes ativos, inativos e até registros com erros.  

- **Source of Truth (SOT) - Fonte da Verdade:**  
  - Remove erros e duplicações sem aplicar regras de negócio.  
  - Exemplo: Apenas usuários **ativos** na newsletter.  

- **Especializações (SPEC):**  
  - Aplicam regras de negócio para criar visões específicas.  
  - Exemplo: Clientes ativos há mais de seis meses.  
  - Permite criar **infinitos níveis de especialização**, adicionando novas regras.  

#### **3. Benefícios da Organização por Níveis de Especialização**  
- **Maior reusabilidade dos dados:**  
  - Diferentes equipes podem utilizar as camadas de dados sem refazer transformações.  
  - Exemplo: A equipe de vendas pode reutilizar a base criada pelo marketing.  
- **Evita erros e retrabalho:**  
  - Garante que os dados tratados sejam confiáveis e prontos para uso.  
  - Facilita o acesso a informações consistentes dentro da organização.  
- **Economiza tempo e melhora a eficiência:**  
  - Reduz a necessidade de validação e processamento repetitivo.  
  - Agiliza a tomada de decisões e análise de dados.
 
### **Resumo sobre Tipos de Linhagem de Dados**  

#### **1. Revisão da Linhagem de Dados**  
- A linhagem de dados rastreia **origens e transformações** dos dados.  
- Pode ser representada **matematicamente e visualmente**.  
- Existem diferentes formas de gerir a linhagem de dados dentro de uma organização.  

#### **2. Tipos de Linhagem de Dados**  

- **Linhagem por nível de tabela:**  
  - Considera apenas **as origens gerais dos dados**.  
  - Exemplo: No caso das recomendações de FIIs, temos três fontes:  
    - **Preço por metro quadrado** das cidades.  
    - **Compras e vendas de imóveis** registradas em cartórios.  
    - **Análises anteriores** da empresa.  

- **Linhagem por nível de coluna:**  
  - Rastreia **a origem e as transformações de cada coluna individualmente**.  
  - Exemplo: A coluna que indica a variação da quantidade de negócios em uma cidade no último mês:  
    - Baseia-se na **quantidade de compras e vendas do cartório**.  
    - Compara-se com **a análise do mês anterior**.  
  - Demonstra como os dados se relacionam e quais transformações foram aplicadas.  

#### **3. Diferenças e Aplicação**  
- **Quando usar linhagem por tabela?**  
  - Para bases menos críticas, onde é suficiente saber de **onde os dados vieram**.  
- **Quando usar linhagem por coluna?**  
  - Para bases mais importantes, onde é necessário rastrear **como cada dado foi transformado**.  

#### **4. Conclusão**  
- Não há uma **regra fixa** para escolha do nível de linhagem.  
- Quanto mais **crítica** for a base de dados para o negócio, mais detalhada deve ser a linhagem.  
- **Combinar diferentes níveis** pode otimizar a governança e rastreabilidade dos dados.


### **Resumo sobre Implementação da Linhagem de Dados**  

#### **1. Primeiros Passos para Implementar a Linhagem de Dados**  
- Definir os principais aspectos da gestão da linhagem:  
  - **Como será feita na organização?**  
  - **Qual o objetivo da implementação?**  
  - **Quais são as responsabilidades das equipes?**  
- Criar uma **política de governança de dados** que estabeleça:  
  - **O que deve ser feito** (definição do processo).  
  - **Como deve ser feito** (métodos e ferramentas).  
  - **Quem são os responsáveis** (equipes envolvidas).  

#### **2. Importância da Educação e Capacitação**  
- A política de linhagem de dados precisa ser compreendida pelas equipes.  
- Capacitação das pessoas-chave (engenheiros de dados e times de dados em geral).  
- Treinamentos e cursos internos para demonstrar a importância da linhagem.  

#### **3. Seleção das Bases de Dados**  
- Não faz sentido exigir linhagem de dados para **todas as bases**, mas sim para as mais estratégicas.  
- Bases **Source of Records (SOR)**, por serem dados brutos, podem não precisar de linhagem.  
- Bases **Source of Truth (SOT)** e especializações exigem registro das origens e transformações.  

#### **4. Definição dos Responsáveis**  
- Engenheiros de dados são geralmente responsáveis pela criação da linhagem.  
- Importante garantir **capacitação técnica** para que saibam documentar a linhagem corretamente.  

#### **5. Estabelecendo o Nível da Linhagem de Dados**  
- **Linhagem por tabela:** usada para bases comuns no **data lake**.  
- **Linhagem por coluna:** recomendada para bases críticas, como aquelas enviadas a órgãos reguladores.  
- Definir **quais bases exigem maior detalhamento** e quais podem ter um nível mais genérico.  

#### **6. Conclusão da Implementação**  
- Criar uma **política estruturada**, com objetivos claros e responsáveis definidos.  
- Garantir a documentação correta para facilitar a rastreabilidade dos dados.  
- Próximo passo: escolher **ferramentas adequadas** para a implementação.  

---

### **Ferramentas para Linhagem de Dados**  

#### **1. Padronização do Processo**  
- Necessário garantir que a linhagem de dados seja **consistente entre diferentes áreas** (fraude, vendas, investimentos).  
- A padronização depende de **boas ferramentas** para gerenciamento da linhagem.  

#### **2. Ferramenta Open Metadata**  
- Muitas ferramentas de linhagem estão **integradas a catálogos de dados e gestão de metadados**.  
- Melhor abordagem: registrar a **linhagem dentro dos metadados** das bases utilizadas.  

#### **3. Características da Open Metadata**  
- **Código aberto (open source):** permite contribuições da comunidade.  
- **Gratuita:** ideal para aprendizado e implementação em organizações de diferentes portes.  
- **Vai além da gestão de metadados:**  
  - Facilita a **colaboração entre equipes de dados**.  
  - Permite rastrear **a linhagem de dados de forma prática e visual**.  

#### **4. Benefícios da Open Metadata**  
- Unifica **gestão de metadados, catálogo de dados e linhagem** em uma única ferramenta.  
- Permite implementar a linhagem de dados sem necessidade de grandes infraestruturas.  
- Facilita **visualizar a linhagem e as dependências entre bases de dados**.  

---

### **Conclusão**  
- A **implementação da linhagem de dados** exige **políticas bem definidas, capacitação das equipes e escolha das bases certas**.  
- A **ferramenta Open Metadata** será utilizada por ser open source, gratuita e fácil de integrar com diferentes áreas da organização.  
- Próximo passo: **praticar a aplicação da linhagem de dados utilizando a Open Metadata** para melhorar a governança e rastreabilidade dos dados.
