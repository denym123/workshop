# Proposta TO-BE: Sistema Integrado de Gestão de Alvarás (SIGA)

O processo TO-BE visa mitigar os gargalos identificados no fluxo AS-IS através da digitalização, automação e integração de mecanismos de governança e gestão por USTs.

---

## 1. Soluções Propostas para os Gargalos Mapeados

Com a implementação do SIGA na Prefeitura de Porto Real, resolvemos as dores crônicas do processo:

- **G-01 (Transporte):** Eliminação total do malote físico entre secretarias. A tramitação ocorre instantaneamente via workflow digital, garantindo agilidade e rastreabilidade total do processo.
- **G-02 (Erros de Preenchimento):** Implementação de formulários eletrônicos inteligentes no Portal do Cidadão. O sistema realiza validações em tempo real (campos obrigatórios, formato de CNPJ, anexos necessários), reduzindo drasticamente a taxa de pendências e o retrabalho na análise técnica.
- **G-03 (Rastreabilidade):** Dashboards de gestão que mostram exatamente onde cada processo está parado, permitindo que o protocolo informe o status real ao cidadão em segundos.

---

## 2. Metas de Melhoria (Novas Métricas)

| Indicador | Valor AS-IS | Meta TO-BE (SIGA) | Impacto Esperado |
| :--- | :--- | :--- | :--- |
| **Tempo Médio Total** | 45 Dias | **7 Dias** | Redução de 84% no tempo de espera do cidadão. |
| **Taxa de Pendência** | Alta (Percebida) | **< 10%** | Maior assertividade na entrada do processo. |
| **Volume Mensal** | ~150 Processos | **~300 Processos** | Dobro da capacidade de vazão sem aumentar a equipe. |
| **Custo por Processo** | Elevado (Físico) | **Reduzido (Digital)** | Economia de papel, transporte e otimização de HH. |

---

## 3. Fluxo Detalhado do Processo (TO-BE)

O novo fluxo utiliza o SIGA como a única fonte da verdade, integrando as áreas de Protocolo, Análise Técnica e Gabinete de forma digital.

| Passo | Atividade | Responsável | Canal / Ferramenta | Entrada | Saída | SLA | Evidência |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **0** | Cidadão preenche solicitação no Portal | Cidadão | Portal SIGA (Web/Mobile) | Formulário Inteligente | Solicitação Digital | N/A | Log de Submissão |
| **1** | Validação automática de documentos | SIGA (Sistema) | Motor de Regras SIGA | Solicitação Digital | Processo Autuado | Instantâneo | Relatório de Validação |
| **2** | Análise técnica digital | Analista Téc. | Dashboard do Analista | Fila de Trabalho Digital | Parecer Digital | 3 Dias | Assinatura Digital Parecer |
| **3** | Assinatura eletrônica do Alvará | Secretário | Assinador Digital SIGA | Parecer Favorável | Alvará Digital Assinado | 1 Dia | Hash de Autenticidade |
| **4** | Disponibilização do Alvará | SIGA (Sistema) | Portal do Cidadão / E-mail | Alvará Assinado | Alvará em PDF / QR Code | Instantâneo | Log de Download |

## 4. Governança B2G e Integração de UST no TO-BE

O SIGA não é apenas uma ferramenta de automação, mas um mecanismo de governança que garante a conformidade do contrato B2G.

- **Formalização de Requisitos (PES):** Qualquer nova funcionalidade ou melhoria no SIGA que esteja explicitamente no TR será formalizada via **PES (Proposta de Execução de Serviço)** antes de entrar em desenvolvimento.
- **Rastreabilidade e Auditoria:** O sistema registrará automaticamente todas as ações (quem, o quê, quando). Esses logs servirão como **evidência primária** para auditorias e medições precisas de USTs.
- **Transparência e Satisfação:** O Portal do Cidadão permitirá o acompanhamento online do status do alvará em tempo real, reduzindo drasticamente a demanda por atendimento presencial e aumentando a satisfação do munícipe.
- **Evidência de Entrega e Faturamento:** A emissão do alvará eletrônico e os logs de conclusão do workflow são as evidências incontestáveis para o faturamento das USTs relacionadas à automação e manutenção do processo.

## 5. Validação do Mapeamento e Proposta

Este documento representa o entendimento da **ae3** sobre o processo atual (AS-IS) e a proposta de otimização (TO-BE). Ele **deve ser validado** pelo responsável no órgão para servir como base sólida para as próximas fases do projeto e para a formalização de USTs para a implementação do SIGA.

- **Responsável pela Validação (Cliente):** Nome do Fiscal ou Gestor do Contrato.
- **Data da Validação:** ____/____/2026

### Evidência do Aceite:
- [ ] Ata de Reunião (Anexar ID/Link)
- [ ] E-mail de Aprovação (Anexar PDF)
- [ ] Assinatura no Documento Físico

---

> [!TIP]
> **Dica de Governança:** No TO-BE, a finalização do Passo 3 (Assinatura) pode gatilhar automaticamente a contagem de USTs para faturamento, uma vez que a evidência (Hash de Autenticidade) é gerada pelo sistema.

> [!CAUTION]
> A implementação do TO-BE sem a validação formal do Gestor do Contrato pode resultar em glosas futuras e desvios de finalidade técnica. Garanta o aceite antes de iniciar o desenvolvimento.
