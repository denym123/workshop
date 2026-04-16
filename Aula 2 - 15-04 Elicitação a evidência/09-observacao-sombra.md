# Etapa 4: Observação Sombra (Shadowing)

A técnica de **Observação Sombra** permite ao analista identificar o que acontece no "mundo real" que muitas vezes é omitido em entrevistas ou workshops. É o momento de ver o processo em ação, sem filtros.

---

## 1. O que buscar na Observação?
- **Atalhos e Gambiarras:** Soluções improvisadas pelos servidores para contornar falhas de sistemas antigos ou processos burocráticos.
- **Retrabalhos Silenciosos:** Atividades que o servidor faz repetidamente (ex: digitar o mesmo dado em duas telas diferentes) e que não foram citadas como um problema formal.
- **Dependências Informais:** "Eu só ando com o processo quando o fulano do outro setor me dá um OK pelo WhatsApp".

## 2. Riscos de Segurança e Integridade
Observar o ambiente de trabalho permite detectar riscos que geram **passivos para o órgão**:
- **Falhas de Acesso:** Senhas anotadas em post-its colados no monitor.
- **Vulnerabilidade de Dados:** Documentos sensíveis (RG, CPF) deixados em mesas de livre acesso ao público.
- **Integridade:** Uso de planilhas locais "paralelas" ao sistema oficial, o que gera divergência de informações.

---

## 3. O Roteiro de Registro
O registro da observação deve ser técnico e focado em fatos:

1.  **Telas Utilizadas:** Quais campos o servidor realmente preenche? Quais ele ignora?
2.  **Pontos de Espera:** Quanto tempo o servidor fica "parado" aguardando o sistema carregar ou uma resposta de terceiros?
3.  **Soluções Adotadas:** Como o servidor resolve um erro de sistema no momento do atendimento?

---

### Exemplo no Estudo de Caso (Porto Real)
Durante o shadowing no balcão de Porto Real, o analista notou que o servidor utiliza uma planilha de Excel pessoal para controlar os prazos, pois o sistema legado não emite alertas.
- **Impacto no SIGA:** O novo sistema deve obrigatoriamente ter um painel de alertas de SLA para eliminar essa planilha paralela e mitigar o risco de perda de dados.

---

> [!CAUTION]
> A observação deve ser passiva. O analista não deve interferir no trabalho do servidor, mas sim documentar a realidade para que o sistema TO-BE seja uma solução e não mais um estorvo.
