# Etapa 2: Entrevista de Contexto de Validação

A entrevista no B2G não é apenas um bate-papo; é um instrumento de **Triangulação de Fontes**. Ela serve para confrontar o que a lei diz (Teórico) com o que realmente acontece no balcão (Real).

---

## 1. Objetivos Metodológicos
1.  **Instrumento de Triangulação:** Cruzar a fala do stakeholder com os requisitos extraídos na Etapa 1. Se o TR diz "A" e o usuário diz "B", o analista deve buscar a evidência material (**EV**) para decidir a verdade.
2.  **Elucidação do Processo Real:** Descobrir os "puxadinhos" operacionais e regras de negócio não escritas que não constam na documentação formal (TR/Contrato).
3.  **Preenchimento de Lacunas:** Utilizar a conversa para definir as **Condições** e **Regras** que ficaram ambíguas na extração documental.

---

## 2. Estratégia de Abordagem

### 2.1. Foco Adaptativo
O analista deve adaptar sua linguagem ao perfil do entrevistado, mas sem perder o rigor técnico.
- **No Protocolo:** Foco na dor operacional e volume de papel.
- **No Gabinete:** Foco em controle, prazos e segurança jurídica (assinaturas).

### 2.2. Entendimento Auditável (Anti-disse-me-disse)
A entrevista só tem valor se puder ser auditada futuramente. 
- **Não aceite:** "Sempre fizemos assim."
- **Pergunte:** "Onde está a portaria ou o manual que descreve esse 'sempre'?" or "Pode me mostrar um exemplo de um caso onde isso aconteceu?"

### 2.3. Principais Atores e seus Focos
Cada perfil exige um conjunto de perguntas voltado para sua responsabilidade no contrato B2G:

- **Fiscal e Gestor do Contrato:** Foco em **Conformidade**. Estão preocupados se o sistema segue o TR e as cláusulas contratuais para evitar glosas.
- **Usuário Final (Servidor):** Foco na **Dor Operacional**. É o ator que revela as exceções que interrompem o fluxo e propõe soluções práticas (ou "contornos").
- **TI e Segurança:** Foco em **Restrições Técnicas**. Estão atentos a padrões de arquitetura, infraestrutura, segurança de dados e interoperabilidade.
- **Jurídico:** Foco na **Legalidade**. Garantem que o fluxo proposto não viola leis municipais, estaduais ou federais (ex: LGPD, Lei 14.133).

---

## 3. Dinâmica no Estudo de Caso (Porto Real)

Durante a entrevista com o funcionário do Protocolo de Porto Real, o objetivo é validar o **G-01** (transporte por malote):

- **A pergunta adaptativa:** *"Como o processo chega até o gabinete do Secretário hoje? Existe algum livro de carga que você assina?"*
- **A busca pela lacuna:** *"O TR diz que a análise deve ser rápida, mas vimos que leva 5 dias. O que acontece entre a sua triagem e o parecer técnico?"*

---

## 4. Pacote de Perguntas Sugeridas

### 4.1. Para o Fiscal ou Gestor do Contrato
Estas perguntas visam blindar o analista e a empresa contra glosas e problemas de auditoria:

- **Sensibilidade de Auditoria:** *"Atualmente, qual parte do TR ou do processo é considerada a mais sensível para uma auditoria (CGU/TCU/TCE)?"*
- **Fluxo de Homologação:** *"Como vocês pretendem realizar a homologação das entregas e qual o rito formal para registrar o aceite (Assinatura, Portal, Sistema)?"*
- **Evidências Mensais:** *"Quais relatórios ou evidências materiais vocês precisam receber mensalmente para processar o faturamento sem pendências?"*
- **Cláusulas Inegociáveis:** *"Para este projeto, o que é absolutamente inegociável por contrato (prazos, segurança, LGPD, funcionalidade específica)?*

### 4.2. Para TI e Segurança
Foco em restrições técnicas e interoperabilidade:

- **Integrações:** *"Quais integrações (APIs, Banco de Dados, Webservices) já existem no ecossistema da prefeitura e quem é o responsável por liberar o acesso?"*
- **Gestão de Acesso:** *"Como é feito o controle atual de perfis de usuário e a geração de logs? Existe um padrão de Single Sign-On (SSO) ou LDAP?"*
- **Infraestrutura:** *"Quais padrões de rede, servidores e segurança de infraestrutura o órgão exige para a instalação do novo sistema?"*

### 4.3. Jurídico / Controle Interno
Foco em conformidade legal e mitigação de riscos:

- **Normativas Internas:** *"Existem leis municipais, decretos ou portarias internas específicas que regulem este processo e que não estavam citadas no TR original?"*
- **Privacidade de Dados (LGPD):** *"Quais dados manipulados neste fluxo são considerados sensíveis e exigem cautela especial ou níveis de acesso restritos?"*

---

> [!TIP]
> **Dica de Ouro:** Saia da entrevista sempre com uma nova evidência (**EV**) na mão ou no e-mail. Uma entrevista sem registro de prova material é apenas uma conversa informal e não sustenta o faturamento de UST.
