# Acessibilidade Digital: eMAG e WCAG

No cenário **Business to Government (B2G)**, a acessibilidade digital transcende a mera recomendação de boas práticas. Ela é um requisito mandatório com profundo impacto na conformidade legal, na inclusão social e na governança de projetos.

---

## 1. O Mandato Legal
A negligência aos padrões de acessibilidade pode resultar em sanções legais e inviabilização de faturamento.
- **Lei Brasileira de Inclusão (Lei 13.146/2015):** Torna obrigatória a acessibilidade em sítios da web mantidos por órgãos de governo e por empresas que prestam serviços públicos.
- **Impacto em USTs:** Um sistema que não atende aos padrões de acessibilidade é considerado um produto com **vício técnico**, o que permite ao fiscal do contrato recusar a homologação e o faturamento das USTs de desenvolvimento.

---

## 2. Padrões Adotados
O analista deve garantir que o sistema siga os dois principais frameworks:
- **eMAG (Modelo de Acessibilidade em Governo Eletrônico):** É o referencial normativo obrigatório para a acessibilidade digital no governo federal brasileiro, assegurando autonomia e equidade no acesso aos serviços públicos. Para o analista de negócios, ele representa um conjunto de requisitos não negociáveis que devem ser integrados ao projeto desde a sua concepção, convertendo-se em critérios de aceite auditáveis que fundamentam tanto as especificações técnicas quanto as validações das USTs.
- **WCAG (Web Content Accessibility Guidelines):** Desenvolvido pelo W3C, é o padrão internacional que serve de base técnica global para a acessibilidade. Em contratos B2G, a exigência do nível **AA (Double-A)** é o padrão de mercado para mitigar riscos de exclusão digital. Ele fornece diretrizes específicas para tornar o conteúdo da web acessível a pessoas com uma ampla gama de deficiências, incluindo visuais, auditivas, físicas, de fala, cognitivas, de linguagem, de aprendizagem e neurológicas.

---

## 3. Os 4 Pilares da Acessibilidade
Para que um sistema seja considerado acessível, ele deve ser:

1.  **Perceptível:** As informações e componentes da interface devem ser apresentados de forma que todos possam perceber (ex: textos alternativos para imagens).
2.  **Operável:** Os componentes da interface e a navegação devem ser operáveis (ex: navegação total via teclado).
3.  **Compreensível:** A informação e a operação da interface devem ser compreensíveis (ex: mensagens de erro claras e linguagem cidadã).
4.  **Robusto:** O conteúdo deve ser robusto o suficiente para ser interpretado por diversas tecnologias assistivas (ex: leitores de tela).

---

## 4. Checklist para o Analista (Validação)
Antes de enviar para homologação, verifique:
- [ ] Existe contraste suficiente entre o texto e o fundo?
- [ ] O sistema permite aumentar a fonte sem quebrar o layout?
- [ ] Todos os campos de formulário possuem rótulos (labels) claros?
- [ ] A ordem de tabulação (tecla Tab) segue o fluxo lógico da tela?

---

### Dinâmica no Estudo de Caso (Porto Real)
No Portal do Cidadão do **SIGA**, a acessibilidade é o que garante que o morador com deficiência visual possa solicitar seu alvará sem ajuda de terceiros.
- **Risco:** Se o botão de "Enviar Requerimento" não tiver um rótulo legível por softwares assistivos, o processo para no portal, gerando uma demanda de atendimento presencial e violando a meta de digitalização do contrato.

---

> [!CAUTION]
> Retrabalho em acessibilidade após o sistema estar pronto é extremamente caro e complexo. O analista deve inserir esses critérios já nas Etapas 1 (Extração) e 5 (Prototipação).
