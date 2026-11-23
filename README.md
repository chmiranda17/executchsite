# Executch no Render

Publique este pacote em um repositório Git e conecte o repositório ao Render como **Blueprint**. O arquivo `render.yaml` configura o site estático e os atalhos de URL.

Para configurar manualmente, crie um **Static Site**, deixe **Root Directory** vazio, use `true` em **Build Command** e `public` em **Publish Directory**. A landing abre em `/`, a página explicativa da integração em `/mcp.html` e a tela de login em `/login.html`.

O pacote contém HTML, CSS e recursos públicos. A autenticação, o manual e o servidor MCP operacional pertencem à instalação do Executch. Para incluir links para a instalação, gere um novo pacote a partir do projeto:

```sh
php tools/exportar_landing_render.php CAMINHO_DE_UMA_NOVA_PASTA https://seu-dominio/executch
```

Sem o endereço, a tela de login é demonstrativa e os links para Minha conta e Manual ficam ocultos. Com o endereço configurado, o botão de acesso e o link de recuperação levam ao sistema real. A tela estática não coleta senhas. O botão de demonstração pelo WhatsApp funciona nas duas versões.