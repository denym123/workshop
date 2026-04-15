# Etapa 0: Preparação e Análise Preliminar

Antes de qualquer interação direta com os usuários, o analista deve realizar uma análise "de mesa" para chegar à reunião com domínio do contexto jurídico e técnico, evitando perguntas básicas cujas respostas já estão nos documentos oficiais.

---

## 1. Análise de TR e Contrato
Esta etapa consiste em dissecar o instrumento convocatório e o contrato administrativo para identificar:
- **Verbos Imperativos:** Mapear termos como *"deve permitir"*, *"deve garantir"*, *"deve registrar"*. Eles sinalizam as obrigações contratuais que o sistema não pode ignorar.
- **Parâmetros de Execução:** Identificar prazos de SLA, critérios de aceite das entregas e obrigações acessórias (backups, segurança, manuais).

## 2. Mapeamento de Ambiguidades
Nesta fase, o analista lista pontos omissos, obscuros ou contraditórios no TR/Edital.
- **Exemplo:** O TR pede "integração com o sistema X", mas não especifica se é via API, banco de dados ou troca de arquivos.
- **Ação:** Estes pontos devem ser os primeiros a serem esclarecidos com a gestão do contrato.

## 3. Introdução ao Mapeamento AS-IS (Documental)
O mapeamento do processo atual é fundamental para estabelecer uma base de comparação. Veremos os detalhes técnicos, objetivos e benefícios deste mapeamento no módulo dedicado à Modelagem AS-IS.

## 4. Roteiro de Investigação
Com base na análise anterior, elabora-se um roteiro de perguntas específicas para cada perfil:
- **Perfil Gestor:** Foco em indicadores, prazos e conformidade.
- **Perfil Operador:** Foco em usabilidade, exceções do processo e dores do dia a dia.
- **Perfil TI/Suporte:** Foco em infraestrutura, segurança e legados.

---

> [!TIP]
> Uma boa Etapa 0 reduz em até 40% o tempo das reuniões de elicitação e evita a descoberta tardia de requisitos contratuais "esquecidos".
