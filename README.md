# Web_Up — página da bio

Página pública: https://i73282137-rgb.github.io/mota-links/

Painel: https://i73282137-rgb.github.io/mota-links/admin.html

O painel edita o nome, a descrição da bio, os projetos, a ordem dos links, a visibilidade e o contato. A prévia acompanha as alterações. Rascunhos ficam somente no navegador.

Em **Publicar alterações**, há duas opções:

- Baixar `site.json`, abrir o envio de arquivos no GitHub e confirmar **Commit changes** na conta que administra o repositório.
- Informar um acesso GitHub com permissão de conteúdo neste repositório e publicar diretamente. A credencial fica somente em memória nesta aba, é enviada apenas para `api.github.com` e é apagada do campo após a tentativa. Ela nunca é gravada no projeto ou no armazenamento do navegador.

A edição da página pública é protegida pelas permissões do próprio GitHub. Abrir o painel sem esse acesso permite apenas preparar um rascunho local.

`site.json` é a configuração pública. `bio.js` valida os campos e atualiza a página usando texto e elementos DOM, sem executar conteúdo digitado. Uma atualização concorrente no GitHub interrompe a publicação direta para evitar sobrescrever outra edição.

Prévia local: `python -m http.server 3033 --bind 127.0.0.1` nesta pasta.
