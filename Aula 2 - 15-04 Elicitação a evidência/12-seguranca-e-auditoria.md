# Segurança e Auditoria: A Blindagem do Processo

Em projetos B2G, a segurança não é apenas técnica, é **jurídica**. A integridade dos dados e a rastreabilidade total são requisitos mandatórios para garantir que a gestão pública seja transparente e auditável.

---

## 1. Controle de Acesso Baseado em Papéis (RBAC)
O sistema deve garantir que cada ator acesse apenas o que é necessário para sua função.
- **Princípio do Menor Privilégio:** Ninguém deve ter mais acesso do que o estritamente necessário.
- **Vínculo Funcional:** O perfil no sistema deve refletir a portaria de nomeação ou a função real do servidor no processo.

---

## 2. Trilha de Auditoria (Audit Trail)
O registro detalhado de eventos é a evidência primária em caso de investigações ou auditorias externas (TCU/TCE). Cada ação relevante no sistema deve registrar:

| Campo | Descrição | Exemplo |
| :--- | :--- | :--- |
| **Quem** | Identificação única do usuário (CPF/Login). | *analista.silva@prefeitura* |
| **Qual Ação** | O que foi feito (Criar, Editar, Excluir, Visualizar). | *Edição de Parecer Técnico* |
| **Quando** | Data e hora com precisão de milissegundos (Timezone UTC). | *15/10/2026 14:32:05.123* |
| **Sobre qual Objeto** | O alvo da ação (ID do Processo, Nome do Cidadão). | *Processo nº 456/2026* |

---

## 3. Logs de Acesso e Alteração
- **Logs de Acesso:** Registram tentativas de login (sucesso e falha), IPs de origem e horários.
- **Logs de Alteração (Histórico):** Devem armazenar o **"Antes"** e o **"Depois"** de cada modificação de dado sensível, permitindo o rollback ou a verificação de integridade.

---

## 4. Segregação de Perfis (Consulta vs. Edição vs. Homologação)

Para garantir a integridade e evitar conflitos de interesse, os perfis devem ser segregados:

- **Perfil Consulta:** Acesso apenas para leitura de dados e relatórios. Ideal para órgãos de controle externo ou munícipes.
- **Perfil Edição:** Destinado aos técnicos e analistas que processam a demanda (ex: Análise Técnica do SIGA).
- **Perfil Homologação/Assinatura:** Exclusivo para autoridades com poder de decisão (ex: Secretário). **Quem edita não pode ser o único a homologar**, garantindo o princípio da segregação de funções.

---

### Dinâmica no Estudo de Caso (Porto Real)
No sistema **SIGA**, a auditoria é o que valida o faturamento das USTs de suporte técnico:
- **Cenário:** Houve uma alteração inesperada no status de um alvará para "Deferido" fora do horário comercial.
- **Uso da Trilha:** O analista acessa a **Trilha de Auditoria** e identifica que a ação foi realizada por um usuário com perfil de "Edição", mas sem o parecer técnico obrigatório.
- **Resultado:** O log serve de evidência para corrigir o erro, identificar a falha de processo e reportar ao fiscal do contrato.

---

> [!IMPORTANT]
> A trilha de auditoria é o seu "seguro de vida" técnico. Sem ela, é impossível provar a integridade das ações e o cumprimento fiel das regras de negócio do contrato.
