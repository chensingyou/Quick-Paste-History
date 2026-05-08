# Suporte técnico do Quick Paste History

---

## 📧 Contatar o desenvolvedor

- **E-mail**: chensingyou@126.com

Ao enviar um e-mail, inclua o seguinte:
1. Sua versão do iOS
2. O modelo do seu dispositivo
3. Uma descrição detalhada do problema ou uma captura de tela
4. Etapas para reproduzir (se aplicável)

---

## ❓ Perguntas frequentes

### 1. A área de transferência não está registrando automaticamente?

Esta é uma restrição de permissão do iOS. Certifique-se de:
1. Quick Paste History foi executado em primeiro plano pelo menos uma vez
2. Na primeira inicialização, você tocou em "Permitir colagem" (janela de permissão do sistema)
3. Se você recusou anteriormente, vá em **Ajustes do sistema → Quick Paste History → Colar de outros Apps** → altere para **Permitir**
4. O histórico da área de transferência é atualizado apenas quando o aplicativo está ativo em primeiro plano. A cada colagem, abra a interface do aplicativo ou sua extensão de teclado.

---

### 2. Como usar a extensão de teclado?

1. Vá em **Ajustes do sistema → Geral → Teclado → Teclados → Adicionar novo teclado**
2. Selecione **Quick Paste History**
3. Toque no nome do teclado Quick Paste History → **Permitir acesso total**
4. Em qualquer campo de entrada de texto, pressione e segure a tecla de alternância de teclado e deslize para cima, depois mude para o teclado Quick Paste History para navegar e colar conteúdo histórico

---

### 3. A sincronização do iCloud não está funcionando?

1. Certifique-se de que todos os seus dispositivos estejam conectados ao mesmo Apple ID
2. Certifique-se de que o iCloud esteja ativado (Ajustes do sistema → Perfil → iCloud → o status deve mostrar "Conectado")
3. Abra o Quick Paste History em diferentes dispositivos e aguarde cerca de 30 segundos — os dados serão sincronizados automaticamente
4. Se a sincronização não ocorrer após muito tempo, tente reiniciar o aplicativo

> A sincronização é baseada em `NSUbiquitousKeyValueStore`. A Apple não fornece uma interface de atualização manual, e a sincronização geralmente é concluída em dezenas de segundos.

---

### 4. Como limpar todo o histórico?

Na página principal do aplicativo, toque no ícone de configurações no canto superior direito → no menu de configurações, selecione "Limpar todos os registros". Esta ação não pode ser desfeita.

---

### 5. Como comprar e usar os recursos Pro?

1. Toque no ícone de configurações no canto superior direito da tela principal → **Atualização Pro**
2. Selecione a versão Pro e faça uma compra no aplicativo
3. Os recursos são desbloqueados automaticamente após a compra
4. Dispositivos com o mesmo Apple ID podem restaurar compras (toque em "Restaurar compra" na página de compra)

---

### 6. O que é Quick Fill (Preenchimento rápido)?

O Quick Paste History permite adicionar informações usadas com frequência ao Quick Fill com antecedência, fornecendo um ponto de entrada rápido na extensão de teclado para colar conteúdo comum rapidamente.

---

### 7. Como usar o recurso de pesquisa?

Na parte superior da página principal, há uma barra de pesquisa. Digite palavras-chave para pesquisar conteúdo textual em seu histórico. Os resultados são classificados por relevância.

---

### 8. Meus dados estão seguros?

- Todos os dados da área de transferência são armazenados apenas localmente no seu dispositivo e no seu espaço privado do iCloud
- O desenvolvedor não pode acessar o conteúdo da sua área de transferência
- Não existe nenhum servidor backend recebendo seus dados
- Consulte a política de privacidade para obter detalhes

---

## 🐛 Relatar um bug

Se encontrar um bug, envie um e-mail para chensingyou@126.com com **[Bug]** no assunto.

Inclua em seu e-mail:
- Versão do iOS
- Modelo do dispositivo
- Etapas para reproduzir (quanto mais detalhado, melhor)
- Capturas de tela ou gravações de tela (se disponíveis)

---

## 💡 Sugestões de recursos

Tem novas ideias? Sinta-se à vontade para enviar um e-mail para discutir, com **[Sugestão]** no assunto. Lerei cada feedback com atenção.
