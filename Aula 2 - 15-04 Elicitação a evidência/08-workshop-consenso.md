# Etapa 3: Workshop de Consenso e Desenho de Fluxo

O Workshop de Consenso é o rito final da fase de elicitação. É o momento onde o analista (ae3) e os principais stakeholders do órgão (Fiscal, TI, Usuários) sentam à mesma mesa para validar o que foi descoberto e desenhar o futuro.

---

## 1. Objetivos do Workshop
- **Unificação dos Fluxos:** Consolidar as versões finais do **AS-IS** e **TO-BE**, garantindo que todos concordam com o funcionamento atual e proposto.
- **Mapeamento de Dados:** Definir o **Dicionário de Dados** básico (quais campos são obrigatórios, quais são opcionais).
- **Tratamento de Exceções:** Listar todos os cenários de "e se..." que não foram previstos no TR mas que o SIGA deve gerenciar.

---

## 2. Entregas Técnicas do Workshop

### 2.1. Dicionário de Dados e Exceções
Nesta etapa, o nível de detalhamento aumenta. Não falamos apenas de "Alvará", falamos de campos específicos:

| Elemento | Tipo de Dado | Regra de Negócio |
| :--- | :--- | :--- |
| **CNPJ Matriz** | Alfanumérico | Deve ser validado via integração com a Receita. |
| **Área do Estabelecimento** | Numérico | Se > 500m², exige vistoria prévia (Exceção). |
| **Data de Vencimento** | Data | Calculada automaticamente (31/03 do ano seguinte). |

### 2.2. A Ata de Decisão (O Escudo do Analista)
Todas as definições feitas no workshop devem ser registradas em uma **Ata de Reunião**.
- **Fundamentação de UST:** Se o grupo decidir que o sistema deve validar a área manualmente em vez de automática, isso muda a estimativa de esforço. A Ata justifica essa mudança frente ao TR original.
- **Congelamento de Escopo:** O que foi decidido no workshop serve como a *baseline* para a implementação do SIGA.

---

## 3. Dinâmica no Estudo de Caso (Porto Real)

No workshop de Porto Real, uma decisão crítica deve ser tomada:
- **A Decisão:** "O sistema SIGA deve enviar notificações por WhatsApp para o cidadão?"
- **O Impacto:** Isso não estava no TR inicial.
- **A Ação:** Registrar em Ata como um item de "Melhoria" a ser faturado via **PES (Proposta de Execução de Serviço)** específica, evitando o aumento de escopo não remunerado.

---

> [!IMPORTANT]
> Sem uma Ata assinada, as decisões do workshop são apenas "disse-me-disse". A Ata é o documento que vincula o desenho técnico à execução financeira das USTs.
