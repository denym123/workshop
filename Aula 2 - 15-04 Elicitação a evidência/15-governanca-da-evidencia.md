# Registro e Validação: Governança da Evidência

A governança da evidência é o processo de garantir que cada requisito elicidado não seja apenas uma "ideia", mas sim um item faturável, auditável e defensável perante qualquer órgão de controle.

---

## 1. Os 4 Pilares da Requisito Governança

Para que uma funcionalidade no **SIGA** seja considerada "governada", ela deve cumprir quatro critérios:

1.  **Registrado:** O requisito deve estar documentado em uma ferramenta oficial (ou repositório central), com identificação única (ID).
2.  **Validado:** Deve possuir um aceite formal (Ata, E-mail, Assinatura) do stakeholder com autoridade para decidir.
3.  **Rastreável:** Deve ser possível identificar sua origem (Ex: Art. 5º da LAI) e seu destino (Ex: Módulo de Exportação CSV).
4.  **Auditável:** O conjunto de documentos (Evidências materiais) deve ser suficiente para provar a terceiros (Auditores) que o requisito foi elicidado e implementado conforme o contrato.

---

## 2. O Fluxo de Validação e Registro

O analista deve seguir este rito para transformar uma conversa em evidência governada:

| Etapa | Ação do Analista | Artefato Gerado |
| :--- | :--- | :--- |
| **Descoberta** | Elicitação técnica (Etapas 0-5). | Notas de reunião / Rascunhos. |
| **Formalização** | Redação no padrão A+O+C+R. | Dossiê de Requisito. |
| **Validação** | Workshop de Consenso com o Cliente. | **Ata de Reunião Assinada**. |
| **Registro** | Inclusão na Matriz de Rastreabilidade. | **Snapshot do Repositório**. |

---

## 3. Rastreabilidade: Do TR ao Faturamento de UST

A governança da evidência protege o faturamento. Se a empresa implementa algo que não é rastreável a uma origem legal ou contratual, o risco de glosa é de 100%.

- **Origem (Source):** Termo de Referência, Lei ou Norma Técnica.
- **Processo (Elicitação):** Ata do Workshop de Consenso.
- **Evidência de Aceite:** Documento de aceite do protótipo/análise.
- **Faturamento (UST):** A soma das evidências acima justifica a nota fiscal.

---

### Dinâmica no Estudo de Caso (Porto Real)
Imagine que o Tribunal de Contas questione o pagamento das USTs referente ao desenvolvimento da "Trilha de Auditoria" do SIGA, alegando que não estava explícito no TR original.
- **A Defesa (Governança):** O analista apresenta a **Ata do Workshop de Consenso** (Validado), onde o Jurídico do órgão exigiu o log conforme a norma interna X (Rastreável), e o **Parecer do Fiscal** aceitando a análise (Auditável).
- **Resultado:** O pagamento é mantido sem ressalvas.

---

> [!IMPORTANT]
> Um requisito bem elicidado, mas mal governado (sem registro e validação), é invisível para o contrato e inexistente para o faturamento.
