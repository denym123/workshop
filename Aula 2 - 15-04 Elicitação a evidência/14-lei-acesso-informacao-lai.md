# Lei de Acesso à Informação (LAI)

A **LAI (Lei 12.527/2011)** estabelece que o acesso à informação é a regra, e o sigilo, a exceção. Em projetos B2G, o sistema deve ser desenhado para suportar a transparência sem gerar sobrecarga operacional.

---

## 1. Transparência Ativa vs. Passiva

- **Transparência Ativa:** O sistema deve disponibilizar automaticamente informações de interesse público no Portal da Transparência (ex: número de alvarás emitidos por mês).
- **Transparência Passiva:** O sistema deve prover ferramentas para que o órgão responda a solicitações específicas de cidadãos dentro dos prazos legais.

---

## 2. Requisitos Técnicos Mandatórios

### 2.1. Registros e Relatórios de Tramitação
O sistema deve gerar históricos detalhados de cada processo administrativo.
- **Histórico Completo:** Registro de cada etapa, data, hora e responsável.
- **Integridade Documental:** Garantia de que os documentos anexados não foram alterados ou excluídos sem rastro.

### 2.2. Exportação de Dados (Formatos Abertos)
A LAI exige que os dados sejam fornecidos em formatos que permitam o processamento automatizado.
- **Funcionalidade:** O SIGA deve permitir a extração de dados em **CSV, JSON ou XML**, além do PDF.
- **Objetivo:** Atender a solicitações de pesquisadores, jornalistas e órgãos de controle de forma rápida.

### 2.3. Trilha de Decisões
Cada despacho, parecer técnico ou decisão do Secretário deve ser registrado formalmente.
- **Despachos:** Registro do texto do despacho, data e assinatura eletrônica.
- **Fundamentação:** Link direto entre a decisão e o parecer técnico que a embasou.

---

## 3. Mecanismos de Atendimento a Pedidos
O sistema deve possuir módulos ou integrações para gerenciar o fluxo de resposta:
1.  **Recebimento:** Interface para entrada do pedido de informação.
2.  **Triagem:** Encaminhamento automático para o setor responsável.
3.  **Resposta:** Interface para o servidor anexar as informações e enviar ao cidadão, com protocolo de recebimento.

---

### Dinâmica no Estudo de Caso (Porto Real)
Imagine que um cidadão solicite via LAI a lista de todos os alvarás emitidos para postos de combustíveis nos últimos 12 meses.
- **Sem LAI no Requisito:** O servidor teria que abrir processo por processo, copiar os dados em uma planilha e enviar (Trabalho manual, alto custo, risco de erro).
- **Com LAI no Requisito (SIGA):** O gestor aplica um filtro por "CNAE" e "Data", clica em **"Exportar CSV"** e anexa ao pedido. O processo leva 2 minutos e garante a conformidade legal.

---

> [!IMPORTANT]
> A falha em prover mecanismos de transparência previstos na LAI pode levar ao bloqueio de certidões do órgão e sanções graves ao gestor, impactando diretamente a percepção de qualidade do serviço prestado pela contratada.
