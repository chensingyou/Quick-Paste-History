# Política de Privacidade do Quick Paste History

**Última atualização: 8 de maio de 2026**

---

## 1. Coleta e Uso de Informações

Quick Paste History é uma ferramenta de gerenciamento de área de transferência cuja função principal é registrar, gerenciar e recuperar o conteúdo da área de transferência localmente no seu dispositivo.

### 1.1 Informações que **não** coletamos

- Informações de identificação pessoal (nome, número de identidade, endereço, etc.)
- Informações confidenciais, como senhas de contas, números de cartão bancário, etc.
- Identificadores de dispositivo (IDFV, IDFA, etc.)
- Histórico de navegação, informações de localização
- Contatos, álbum de fotos, microfone, dados da câmera
- Estatísticas de comportamento de uso ou dados analíticos

### 1.2 Informações às quais **acessamos**

O Quick Paste History acessa apenas as seguintes informações localmente no seu dispositivo, conforme necessário para suas funções principais:

| Tipo de dado | Finalidade | Upload para servidor |
|--------------|------------|:--------------------:|
| **Conteúdo da área de transferência** | Registra texto/links copiados pelo usuário, suporta pesquisa, favoritos e preenchimento rápido | Apenas armazenamento local |
| **iCloud** | Sincroniza o histórico entre seus dispositivos via NSUbiquitousKeyValueStore | Apenas sincronização privada do iCloud |
| **Compra no App Store** | Verifica o status de compra dos recursos Pro (apenas verificação de recibo) | Nenhum detalhe de compra coletado |

> Todo o processamento de dados da área de transferência é feito localmente no dispositivo e **não será enviado para nenhum servidor externo**.

---

## 2. Armazenamento de Dados

### 2.1 Armazenamento Local

- Os históricos da área de transferência são armazenados em um banco de dados SwiftData dentro do sandbox do aplicativo
- O banco de dados não é criptografado (o mecanismo de sandbox da Apple fornece isolamento em nível de sistema)
- Os usuários podem limpar manualmente todo o histórico

### 2.2 Sincronização do iCloud (Funcionalidade Opcional)

- Quando ativada, o histórico é sincronizado via `NSUbiquitousKeyValueStore` em sua própria conta do iCloud
- Os dados são protegidos pelos mecanismos de segurança do iCloud e não podem ser acessados pelo desenvolvedor
- A sincronização pode ser desativada a qualquer momento nas configurações
- Desativar a sincronização não excluirá os dados locais

### 2.3 Retenção de Dados

- O histórico é mantido por padrão; os usuários podem excluir manualmente entradas individuais ou limpar tudo
- A exclusão entra em vigor imediatamente e é irreversível

---

## 3. Compartilhamento de Dados

O Quick Paste History **não compartilha dados do usuário com terceiros**, incluindo, mas não se limitando a:

- Não vende dados do usuário
- Não usa dados para publicidade ou criação de perfil de usuário
- Não envia conteúdo da área de transferência para APIs de terceiros
- Não incorpora SDKs de análise de terceiros

---

## 4. Extensão de Teclado e Permissões

O Quick Paste History fornece uma Extensão de Teclado (Keyboard Extension) para colar rapidamente o conteúdo do histórico em qualquer aplicativo:

- **Acesso**: A extensão de teclado só é executada quando ativada e lê apenas o conteúdo da área de transferência
- **Rede**: A extensão de teclado não tem permissão de acesso à rede
- **Isolamento de dados**: A extensão de teclado compartilha dados do sandbox com o aplicativo principal, mas não os expõe externamente

---

## 5. Leitura da Área de Transferência

O Quick Paste History lê a área de transferência nas seguintes ocasiões:
- Quando o aplicativo está em execução em primeiro plano, ele detecta alterações na área de transferência e registra novo conteúdo
- Quando o usuário compartilha ativamente conteúdo com o Quick Paste History

De acordo com os requisitos do sistema iOS, a primeira leitura da área de transferência acionará um diálogo de permissão em nível de sistema. Os usuários podem gerenciar essa permissão a qualquer momento nas Configurações do Sistema.

---

## 6. Privacidade Infantil

O Quick Paste History não coleta informações pessoais de crianças.

---

## 7. Alterações na Política de Privacidade

Se a política de privacidade for alterada, atualizaremos a data de "Última atualização" no topo da página e notificaremos os usuários por meio de avisos no aplicativo ou notas de atualização de versão.

---

## 8. Entre em Contato

Se você tiver dúvidas sobre a política de privacidade, entre em contato conosco através dos seguintes canais:

- **Desenvolvedor**: 陈修
- **E-mail**: chensingyou@126.com
- **App**: Quick Paste History (Desenvolvedor: Singyou)

---

> **Resumo: Seus dados pertencem a você.** O Quick Paste History não envia conteúdo para servidores, não rastreia o comportamento do usuário e não incorpora SDKs de terceiros. Todos os dados da área de transferência são processados apenas localmente no dispositivo e no espaço privado do iCloud.
