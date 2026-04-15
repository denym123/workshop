# Modelagem AS-IS: Objetivo e Baseline

O mapeamento do processo "como ele é" (AS-IS) é o ponto de partida para qualquer transformação digital no B2G. Não se trata apenas de desenhar fluxos, mas de estabelecer uma verdade compartilhada.

---

## 1. Objetivo do AS-IS
Descrever como um processo funciona hoje no cliente para criar um entendimento compartilhado entre o analista (ae3) e o órgão. 

Muitas vezes, diferentes departamentos do mesmo órgão possuem visões conflitantes sobre o mesmo processo. O analista atua como o mediador que consolida essa visão única.

## 2. Por que investir tempo no AS-IS?
- **Identificação de Gargalos:** Descobrir onde o processo trava, onde há redundância de dados e onde ocorrem falhas de comunicação.
- **Mapeamento de Riscos:** Identificar pontos onde a conformidade legal pode estar sendo violada ou onde há risco de perda de dados.
- **Base Sólida (Baseline):** Estabelecer o marco zero para o desenho do projeto no futuro (**TO-BE**). Sem saber onde estamos, não podemos medir o sucesso de onde queremos chegar.
- **Subsolo da Elicitação:** O AS-IS fornece a base para a elicitação de requisitos funcionais e, principalmente, as regras de negócio que o sistema deve herdar ou transformar.

## 3. Abordagem Preliminar (AS-IS Documental)
Ao iniciar o AS-IS na Etapa 0, o analista foca na documentação disponível para criar um modelo de alto nível.
- **Validação:** Este modelo é levado para as entrevistas para ser confrontado com a realidade operacional (Processo Real vs. Teórico).
- **Ajustes:** O modelo é refinado à medida que novas evidências (logs, prints, planilhas) são coletadas.

## 4. Estudo de Caso Prático: Prefeitura de Porto Real

Neste cenário, aplicaremos as técnicas de mapeamento AS-IS focadas no projeto **SIGA (Sistema Integrado de Gestão de Alvarás)**.

### 4.1. Definição do Escopo
Um erro comum em B2G é tentar mapear "o mundo todo". Aqui, delimitaremos as fronteiras do nosso trabalho de elicitação:

> [!TIP]
> **IN (O que está incluído):**
> - Todas as etapas desde a solicitação inicial do cidadão no **balcão de atendimento** até a entrega final do **alvará impresso**.
> - Fluxos que percorrem as áreas de: **Protocolo**, **Análise Técnica** e **Gabinete do Secretário**.

> [!WARNING]
> **OUT (O que NÃO está incluído):**
> - O processo de **fiscalização pós-emissão** do alvará (visitas de fiscais de rua).
> - A **Arrecadação de Taxas**, visto que este processo ocorre em um sistema externo legado e o SIGA apenas receberá a confirmação do pagamento.

### 4.2. Pontos de Atenção para o Analista
Ao mapear este processo, o analista deve focar em descobrir como a informação "viaja" entre o Protocolo e o Gabinete:
- Existem pastas físicas?
- O Gabinete precisa de uma assinatura manuscrita ou digital?
- Quais critérios a Análise Técnica usa para aprovar ou indeferir?

### 4.3. Inventário de Evidências Coletadas
Para validar o AS-IS de Porto Real, o analista deve organizar as fontes conforme o padrão abaixo. Este registro garante a rastreabilidade absoluta do requisito.

| ID | Tipo | Descrição | Origem | Data | Link/Anexo |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **EV1** | Documento | Termo de Referência do Pregão | Compras | 15/10/2025 | [Link](#) |
| **EV2** | Formulário | Requerimento de Abertura de Protocolo | Protocolo | 16/10/2025 | [Link](#) |
| **EV3** | Observação | Shadowing no Balcão de Atendimento | Protocolo | 17/10/2025 | [Link](#) |
| **EV4** | Documento | Registro de Protocolo (Sist. Legado) | Protocolo | 18/10/2025 | [Link](#) |
| **EV5** | Parecer | Parecer Técnico de Viabilidade | Análise Téc. | 20/10/2025 | [Link](#) |
| **EV6** | Alvará | Alvará de Funcionamento Assinado | Gabinete | 22/10/2025 | [Link](#) |
| **EV7** | Recibo | Livro de Carga / Protocolo de Entrega | Protocolo | 23/10/2025 | [Link](#) |

> [!NOTE]
> **Tipos Aceitos:** Documento, Observação, Formulário, Entrevista, Log de Sistema.
> **Origens Comuns:** Compras, Protocolo, Gabinete, TI.

### 4.4. Fluxo Detalhado do Processo (AS-IS)
Abaixo, detalhamos cada etapa do processo atual, ancorando cada atividade em sua respectiva evidência material.

| Passo | Atividade | Responsável | Canal / Ferramenta | Entrada | Saída | SLA | Evidência |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **0** | Cidadão preenche e entrega o requerimento | Cidadão | Balcão de Atendimento | Requerimento | Requerimento preenchido | N/A | **EV3** |
| **1** | Registro e autuação do processo | Protocolo | Sist. Legado / Físico | Requerimento preenchido | Capa de Processo / ID | 24h | **EV4** |
| **2** | Análise de documentos e viabilidade | Analista Téc. | Pasta Física + Check-list | Processo Autuado | Parecer Técnico | 5 dias | **EV5** |
| **3** | Revisão e Assinatura do Alvará | Secretário | Gabinete (Pasta suspensa) | Parecer Favorável | Alvará assinado | 2 dias | **EV6** |
| **4** | Entrega do Alvará ao cidadão | Protocolo | Balcão de Atendimento | Alvará assinado | Alvará entregue | Imediato | **EV7** |

> [!TIP]
> **Dica para o Analista:** No Passo 0, observe se o cidadão recebe algum comprovante de entrega (Protocolo). Isso pode ser uma evidência **EV4** a ser coletada.

### 4.5. Métricas Atuais do Processo (Indicadores)
Conhecer os números atuais é vital para medir o sucesso do SIGA no futuro. Estes dados foram coletados através da triangulação de fontes técnicas e humanas:

| Indicador | Valor Atual | Observação / Evidência |
| :--- | :--- | :--- |
| **Tempo Médio Total** | 45 Dias | Do protocolo à entrega final do alvará impresso. |
| **Taxa de Pendência/Indeferimento** | Alta (Não medida) | Percepção de alto retrabalho por falta de validação inicial. |
| **Volume Mensal** | ~150 Processos | Média constante de solicitações no balcão de atendimento. |
| **Custo Estimado** | Não Medido | Envolve papel, transporte físico e horas-homem de 3 secretarias. |

---

## 5. Gargalos, Dores e Retrabalhos

Identificar os pontos de fricção no AS-IS é o que justifica a criação do novo sistema (SIGA). Abaixo, listamos os principais gargalos mapeados no processo da Prefeitura de Porto Real:

| | Dor/Gargalo | Onde ocorre | Causa Provável | Efeito | Indicador Atual | Evidência |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| **G-01** | Perda de tempo no transporte | Entre os passos 2 e 3 | O transporte por malote entre secretarias é lento e ocorre apenas 2 vezes por semana. | O processo fica parado por até 3 dias. | 45 dias (tempo médio total) | **EV-02** |
| **G-02** | Erros de preenchimento | No passo 1 | O formulário físico é complexo e não tem validação, gerando erros que só são vistos no passo 4. | Alta taxa de pendências (estimada em 40%). | N/A | **EV-02** |
| **G-03** | Falta de rastreabilidade | No passo 2 | O processo é físico e não há registro centralizado de quem está com a pasta. | O cidadão liga para o protocolo e ninguém sabe informar o status real. | 10 ligações/dia | **EV-03** |

---

> [!IMPORTANT]
> Um AS-IS mal feito gera um TO-BE que não resolve os problemas reais do cliente ou, pior, que automatiza a ineficiência.
