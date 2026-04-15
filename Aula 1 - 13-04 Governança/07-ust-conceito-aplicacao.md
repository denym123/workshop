## 7. UST: Unidade de Serviço Técnico

A Unidade de Serviço Técnico (UST) é um dos modelos mais utilizados para a contratação e remuneração de serviços de TI no setor público, servindo como a base para a evolução contínua das plataformas B2G.

### 7.1. Conceito e Propósito

A UST é um mecanismo de mensuração de esforço e complexidade que permite viabilizar a evolução contínua do projeto dentro da conformidade legal.

> **Nota de Contexto AE3:** Atualmente, a **AE3** utiliza exclusivamente o modelo de **UST** em suas operações e contratos, pela versatilidade e foco no esforço técnico completo. Embora o modelo de Ponto de Função possa ser adotado futuramente conforme a necessidade de novos editais, a base atual de entrega e precificação de serviços de excelência da empresa fundamenta-se na UST.

- **Foco em Resultados:** Diferente do modelo de "horas trabalhadas", a UST foca na entrega de atividades específicas e resultados mensuráveis.
- **Complexidade:** Permite que o órgão público remunere de forma justa a complexidade das tarefas realizadas, garantindo que requisitos técnicos avançados sejam devidamente valorizados.
- **Flexibilidade Controlada:** Oferece agilidade para evoluir o sistema conforme novas necessidades surgem, sem ferir o escopo contratual original, desde que as atividades estejam catalogadas.

### 7.2. Aplicação no B2G

No contexto de Business to Government, a UST é a ferramenta que permite que o software não se torne obsoleto. Ela é aplicada para:

- Desenvolvimento de novas funcionalidades.
- Manutenção evolutiva e corretiva.
- Integrações complexas com outros sistemas governamentais.

### 7.3. Como Medir: A Visão do TCU

O **Tribunal de Contas da União (TCU)**, por meio de diversas orientações e guias de boas práticas, recomenda o uso de métricas objetivas para a mensuração de serviços de TI.

- **Objetividade:** A métrica não pode ser subjetiva. Deve haver uma tabela clara (Catálogo de Serviços) onde cada atividade corresponde a uma quantidade específica de USTs.
- **Independência:** A medição deve ser verificável de forma independente pelo fiscal do contrato.
- **Rastreabilidade:** Cada UST paga deve estar vinculada a uma evidência de entrega (ex: documentação técnica, código no repositório, homologação da área usuária).

### 7.4. Estrutura da Tabela de UST (Catálogo de Serviços)

Para dar transparência e segurança jurídica, as atividades devem ser catalogadas com critérios claros de pontuação. Abaixo, um exemplo de estrutura:

| Atividade                 | Descrição                                                        | Unidade de Medida             | Esforço (UST)         |
| :------------------------ | :--------------------------------------------------------------- | :---------------------------- | :-------------------- |
| **Desenvolvimento**       | Criação de nova funcionalidade, módulo ou integração de sistema. | Funcionalidade / Complexidade | Variável (ex: 5 a 20) |
| **Manutenção Corretiva**  | Identificação e correção de bugs ou falhas de execução.          | Ticket / Severidade           | 2 a 8                 |
| **Documentação Técnica**  | Criação ou atualização de manuais, ETPs, TRs ou diagramas.       | Documento / Artefato          | 3 a 10                |
| **Suporte Especializado** | Atuação em problemas técnicos de alta complexidade.              | Chamado / Hora Técnica        | 1 a 4                 |

---

**Nota Importante:** A coluna "Esforço (UST)" deve ser acompanhada por uma **Matriz de Complexidade** (Baixa, Média, Alta) que defina exatamente o que justifica cada pontuação dentro do intervalo.

**Nota Importante:** O uso de UST sem um catálogo de serviços bem definido é um dos principais pontos de risco em auditorias. A clareza no que compõe cada unidade é essencial para a segurança jurídica de ambas as partes.

### 7.5. Referências e Exemplos Reais

Para uma compreensão mais profunda de como um órgão público estrutura seu catálogo de serviços, consulte o exemplo oficial:

- [Catálogo de Serviços de TI - Exemplo CNEN (gov.br)](https://www.gov.br/cnen/pt-br/assunto/tecnologia-da-informacao/catalogo.pdf)

### 7.6. Comparativo: UST vs. Ponto de Função

É comum surgir a dúvida entre o uso de UST e Pontos de Função (PF). Embora ambos sejam métricas de mensuração, eles partem de premissas diferentes:

- **Ponto de Função (PF):**
  - **Foco na Entrega Final:** É uma métrica de "resultado funcional". Mede o software pela ótica do usuário (telas, arquivos, consultas).
  - **Visão Limitada:** Muitas vezes é interpretado apenas como o desenvolvimento de funcionalidades, tendendo a ignorar o processo completo e a complexidade de análise envolvida.
- **UST (Unidade de Serviço Técnico):**
  - **Foco no Esforço e Processo:** É vinculado primordialmente ao **esforço** necessário para realizar uma atividade técnica de ponta a ponta (desde a análise de requisitos até a implementação e testes).
  - **Cobertura Abrangente:** Diferente do PF, a UST engloba atividades que não resultam em novas funções, mas são cruciais, como:
    - Sustentação e manutenção de código existente.
    - Processos de análise técnica e arquitetural.
    - Suporte, infraestrutura e segurança.

- **Fórmula de Conversão Estipulada:**
  Em muitos modelos de precificação e editais, utiliza-se uma paridade para converter o esforço de desenvolvimento (medido em PF) para a métrica de serviço (UST). Para este workshop, consideraremos a relação:
  > **1 PF = 12 UST**

**Conclusão:** O Ponto de Função mede o "O Quê" (funcionalidades), enquanto a UST mede o **"Como"** e o **"Quanto"** (esforço, análise e complexidade técnica) de todo o ecossistema B2G.
