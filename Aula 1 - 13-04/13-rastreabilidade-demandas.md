## 13. Rastreabilidade de Demandas

No ambiente de contratações públicas B2G, a rastreabilidade não é apenas uma boa prática de engenharia de software, mas uma **premissa jurídica inegociável**.

### 13.1. Origem Documental Comprovável
Cada requisito funcional, regra de negócio ou alteração técnica desenvolvida e entregue pela **AE3** deve ter uma origem documental clara.
- **Onde começa:** Todo desenvolvimento deve estar lastreado no **ETP**, no **TR** ou em um **Aditivo Contratual**.
- **Formalização:** Demandas que surgem em reuniões informais ou conversas de "corredor" devem ser formalizadas via Ordem de Serviço ou e-mails oficiais antes de entrarem no ciclo de desenvolvimento.

### 13.2. Proteção Contra Glosas
A "glosa" ocorre quando o órgão público se recusa a pagar por um serviço por considerá-lo fora do escopo ou sem comprovação adequada.
- **Defesa Técnica:** A rastreabilidade é o "escudo" da empresa. Se um fiscal questionar uma entrega, o analista deve ser capaz de apontar exatamente em qual documento aquela demanda foi solicitada e aprovada.
- **Transparência:** Garantir que o faturamento seja liberado sem atritos, pois todas as evidências (logs, relatórios, códigos) estão vinculadas a um requisito formal.

### 13.3. O Ciclo da Rastreabilidade
1.  **Fundamento:** Requisito presente no TR/Contrato.
2.  **Autorização:** Ordem de Serviço ou demanda formalizada.
3.  **Execução:** Desenvolvimento com registro de esforço (UST).
4.  **Entrega:** Relatório de Atividades com evidências materiais.
5.  **Aprovação:** Termo de Aceite assinado.

### 13.4. Exemplo Prático de Rastreabilidade
Para ilustrar como o analista deve conduzir o processo:

1.  **A Origem (TR/Contrato):** O documento base exige, por exemplo, a criação de "Notificações Automáticas de Status".
2.  **A Tradução (Requisito):** O Analista de Negócios traduz essa exigência genérica em um requisito funcional: "O sistema deve enviar notificações por e-mail e push para o cidadão e o servidor sempre que o status do benefício for alterado".
3.  **O Desenvolvimento (História do Usuário):** Esse requisito é desdobrado em uma *User Story* no Jira, com critérios de aceite técnicos e funcionais claros para a equipe de desenvolvimento.
4.  **A Comprovação (Evidência):** A entrega só é considerada comprovada quando há provas irrefutáveis (ex: logs de disparo de e-mail, capturas da tela de notificação e código-fonte no repositório) anexadas ao Relatório de Atividades.

---
**Conclusão:** Sem rastreabilidade, a empresa assume um risco jurídico e financeiro altíssimo. O papel do analista é garantir que nenhum esforço técnico seja "órfão" de documento.
