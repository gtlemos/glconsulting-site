# GL Consulting — site institucional

Site estático, responsivo e bilíngue (português/inglês), feito com HTML, CSS e JavaScript puro.

## Arquivos

- `index.html` — estrutura e conteúdo do site
- `styles.css` — identidade visual e layout responsivo
- `script.js` — alternância PT/EN, menu mobile e formulário
- `config.js` — e-mail e WhatsApp que você deve configurar

## 1. Configuração antes de publicar

Abra `config.js` e preencha:

```js
window.GL_CONFIG = {
  email: "seu-email-real@glconsultingbr.com",
  whatsapp: "5542999999999"
};
```

Use um e-mail que já esteja criado e recebendo mensagens. O WhatsApp deve conter código do país + DDD + número, apenas dígitos. Se não quiser WhatsApp ainda, deixe `whatsapp: ""`.

O formulário é estático: ele prepara uma mensagem no aplicativo de e-mail do visitante. Não armazena dados em servidor.

## 2. Testar localmente

Basta abrir `index.html` no navegador. Para testar de forma mais fiel, use a extensão Live Server do VS Code ou rode um servidor local simples.

## 3. Publicar gratuitamente no GitHub Pages

1. Crie ou entre em uma conta em https://github.com.
2. Crie um repositório público chamado `glconsulting-site`.
3. Envie os quatro arquivos deste pacote para a raiz do repositório.
4. No GitHub, abra **Settings → Pages**.
5. Em **Build and deployment**, escolha **Deploy from a branch**.
6. Selecione a branch `main` e a pasta `/ (root)` e salve.
7. Aguarde o GitHub publicar o endereço temporário `https://SEU-USUARIO.github.io/glconsulting-site/`.
8. Em **Settings → Pages → Custom domain**, informe `glconsultingbr.com` e salve.
9. No painel do registrador onde o domínio está, configure os registros DNS indicados pela documentação atual do GitHub Pages. Para domínio raiz, normalmente são registros A para os endereços IPv4 publicados pelo GitHub; também é possível configurar `www` com CNAME para `SEU-USUARIO.github.io`.
10. Depois que o DNS propagar, volte a **Settings → Pages** e habilite **Enforce HTTPS** quando a opção estiver disponível.

Documentação oficial: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site

## 4. Alternativa: Cloudflare Pages

Também é possível importar o repositório do GitHub em https://pages.cloudflare.com/ e conectar o domínio. O plano gratuito atende sites institucionais estáticos; confira os limites atuais do plano antes de publicar.

## Observações importantes

- O domínio `glconsultingbr.com` precisa continuar registrado e renovado.
- Hospedagem gratuita não inclui caixa de e-mail. E-mail profissional é um serviço separado (por exemplo, Google Workspace ou outro provedor).
- Não publique dados privados, senhas ou chaves em repositório público.
- O site usa Google Fonts. Se preferir não depender de um serviço externo, remova os imports de fontes no `<head>` e o CSS usará fontes alternativas.
- Revise os textos, e-mail e telefone antes de divulgar o endereço publicamente.
