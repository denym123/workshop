# Requisitos Brutos vs. Estruturados

O sucesso de um projeto B2G depende da capacidade do analista de traduzir a "vontade do usuário" (Requisito Bruto) em uma "especificação técnica e auditável" (Requisito Estruturado).

---

## 1. O Requisito Bruto
É a fala direta do stakeholder, muitas vezes carregada de subjetividade e lacunas.
> **Exemplo (Porto Real):** *"O cidadão precisa conseguir pedir o alvará pelo site pra gente não ter que atender todo mundo no balcão."*

---

## 2. O Requisito Estruturado
É a transformação da fala em um artefato de engenharia de software e governança.

### 2.1. Template de User Story
Utilizamos o padrão para definir o **Quem**, o **O que** e o **Porquê**:
- **Como** [Perfil / Papel]
- **Eu quero** [Ação / Funcionalidade]
- **Para** [Benefício / Valor de Negócio]

> **Exemplo Estruturado:** Como **Cidadão de Porto Real**, eu quero **solicitar o alvará de funcionamento via Portal SIGA** para **evitar o deslocamento físico ao balcão de atendimento**.

### 2.2. Critérios de Aceite (BDD - Given/When/Then)
Definem o limite do que será entregue e como será testado.
- **Dado que** [Contexto / Pré-condição]
- **Quando** [Ação do usuário]
- **Então** [Resultado esperado]

> **Cenário de Sucesso:**
> - **Dado que** o cidadão preencheu todos os campos obrigatórios do formulário.
> - **Quando** clicar no botão "Enviar Requerimento".
> - **Então** o sistema deve gerar um número de protocolo e enviar um e-mail de confirmação.

---

## 3. Matriz de Fontes e Evidências

Para cada requisito estruturado, o analista deve mapear sua linhagem:

| Elemento | Descrição | Exemplo no SIGA |
| :--- | :--- | :--- |
| **Fonte** | Onde está escrito que isso é necessário? | **TR (EV1) / Lei Municipal 123** |
| **Evidência Esperada** | O que prova que o requisito foi cumprido? | **Print da Tela / Log de Envio de E-mail** |
| **Formalização** | Documento que validou o entendimento. | **Ata de Workshop (Etapa 3)** |

---

### Dinâmica Prática
Ao estruturar o requisito, o analista garante que:
1.  O desenvolvedor sabe exatamente o que construir.
2.  O fiscal sabe exatamente o que testar (Critérios de Aceite).
3.  A auditoria sabe exatamente qual lei justifica aquela funcionalidade (Fonte) e qual arquivo prova a entrega (Evidência).

---

> [!TIP]
> **Dica de Governança:** Nunca inicie o desenvolvimento de uma User Story sem que seus Critérios de Aceite tenham sido validados pelo Fiscal do Contrato. Isso evita o retrabalho por "falha de interpretação".
