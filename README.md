# academico.kovags.com

Porta de entrada da área **Acadêmico** do portal kovags.com, publicada pelo GitHub Pages com domínio próprio.

As páginas **não ficam aqui**: continuam no cPanel, em `kovags.com/academico/` (inclusive o que é publicado pelo
`publicar.php`). O `index.html` (e o `404.html`, para os demais caminhos) busca a página do caminho pedido
em `https://kovags.com/academico/<caminho>/index.html?carregar=1` e a abre neste endereço, com um `<base>` que faz
os links e arquivos apontarem para o kovags.com.

No kovags.com, o `.htaccess` libera CORS para este endereço e redireciona `kovags.com/academico/` para cá
(o parâmetro `carregar=1` evita o redirecionamento quando a página é buscada por esta porta).
