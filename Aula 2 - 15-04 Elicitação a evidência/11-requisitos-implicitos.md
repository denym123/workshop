# Requisitos Implícitos: O "Radar" do Analista

No contexto B2G, nem tudo o que o sistema **deve** fazer está escrito no Termo de Referência. Requisitos implícitos são obrigações mandatórias por força de lei, normas técnicas ou boas práticas de governança.

---

## 1. O Conceito
Requisitos implícitos representam obrigações não explicitadas formalmente no instrumento convocatório (TR), mas que são indispensáveis para a entrega. 

> [!WARNING]
> A falha em identificar e formalizar esses requisitos é uma das principais causas de **retrabalho**, **glosas financeiras** e **questionamentos** por órgãos de controle (CGU, TCU, controladorias internas).

---

## 2. Categorias de Requisitos Implícitos

### 2.1. Jurídica e Conformidade
Mesmo que o TR não cite, o sistema deve respeitar:
- **LGPD (Lei Geral de Proteção de Dados):** Criptografia de dados sensíveis, logs de acesso e gestão de consentimento.
- **LAI (Lei de Acesso à Informação):** Disponibilização de dados públicos em formatos abertos e acessíveis.
- **Marcos Legais:** Leis específicas do setor (Saneamento, Saúde, Educação).

### 2.2. Técnica e Interoperabilidade
- **Segurança:** Padrões de autenticação, firewalls e backups.
- **Integração:** O sistema deve "falar" com outros sistemas do governo (ex: barramento de serviços).
- **Desempenho:** Tempos de resposta que garantam a continuidade do serviço público.

### 2.3. Social e Acessibilidade
- **eMAG (Modelo de Acessibilidade em Governo Eletrônico):** O sistema deve ser utilizável por pessoas com deficiência, independentemente de o TR exigir explicitamente.

---

## 3. Estratégia de Identificação
O analista atua como o **Radar de Conformidade**:
1.  **Cruzar o TR com a Hierarquia de Autoridade:** Se o TR pede um cadastro, a LGPD (Lvl 1) impõe que o aceite de privacidade seja implícito.
2.  **Questionar no Workshop de Consenso:** "O TR não cita auditoria de logs, mas como faremos para atender à norma interna de segurança do órgão?"
3.  **Formalizar via PES:** Requisitos implícitos descobertos devem ser formalizados como itens de escopo para garantir que a equipe técnica os implemente e que as USTs sejam aplicadas corretamente.

---

### Exemplo no Estudo de Caso (Porto Real)
O TR do sistema **SIGA** não exigia a exportação de dados em formato CSV para o Portal da Transparência.
- **Requisito Implicito:** Pela **LAI**, o órgão é obrigado a fornecer dados abertos.
- **Custo do Erro:** Se não identificado, o órgão pode sofrer uma multa ou advertência do Ministério Público, e a empresa teria que fazer um retrabalho de emergência (não faturado) para evitar a glosa do contrato.

---

> [!IMPORTANT]
> Tornar o implícito em **explícito** através da documentação é o que separa um analista júnior de um especialista em B2G.
