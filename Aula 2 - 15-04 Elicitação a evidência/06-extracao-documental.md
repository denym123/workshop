# Etapa 1: Extração Documental

Após a preparação (Etapa 0), o analista inicia a **Extração Documental**. O objetivo é transformar textos jurídicos e técnicos complexos (Leis, TRs, Decretos) em requisitos estruturados e compreensíveis.

---

## 1. A Fórmula da Extração: A+O+C+R

Para garantir que nenhum requisito seja ambíguo, utilizamos a estrutura **Ação-Objeto-Condição-Regra**.

| Elemento | Definição | Exemplo no SIGA |
| :--- | :--- | :--- |
| **Ação** | O verbo imperativo (o que o sistema deve fazer). | **Emitir** |
| **Objeto** | O alvo da ação (sobre o que a ação atua). | **Alvará de Funcionamento** |
| **Condição** | O gatilho ou estado necessário para a ação. | **Após deferimento da análise técnica** |
| **Regra** | A fundamentação legal ou de negócio (O "porquê"). | **Conforme Lei Municipal nº 1.234/2020** |

---

## 2. Evento Prático (Mão na Massa)

A extração não é apenas "copiar e colar". O analista deve interpretar o **Evento Prático** por trás do texto.

### Exemplo de Extração do TR (EV1)
> **Texto Original no TR:** *"A contratada deverá prover meio eletrônico para que o fiscal do gabinete possa assinar os documentos de licenciamento sem a necessidade de deslocamento físico, respeitando a hierarquia administrativa."*

**Requisito Estruturado:**
- **Ação:** Assinar eletronicamente.
- **Objeto:** Alvará de Funcionamento.
- **Condição:** Após parecer favorável da Análise Técnica.
- **Regra:** Hierarquia administrativa do Gabinete (Secretário).

**Evento Prático:** O Secretário recebe uma notificação no SIGA, visualiza o PDF do alvará e o parecer técnico, e realiza a assinatura digital em lote ou individual.

---

## 3. Benefícios desta Técnica
- **Elimina Ambiguidade:** "Ação-Objeto" define o que deve ser construído sem margem para interpretação.
- **Facilita o Teste:** Cada condição e regra se torna um cenário de teste automático ou manual.
- **Rastreabilidade:** A "Regra" aponta diretamente para a fonte da hierarquia de autoridade.

---

> [!IMPORTANT]
> Se você não consegue definir a **Regra** (a base legal), o requisito pode ser apenas um "desejo" subjetivo do usuário e deve ser tratado com cautela para evitar desvios de escopo.
