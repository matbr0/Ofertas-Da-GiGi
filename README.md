# Ofertas da Gigi — Site de Ofertas

Site estilo "linktree" para divulgar as ofertas da conta **Ofertas da Gigi**, mantendo a identidade visual (fundo escuro, tom coral, logo e banner) usada nas redes sociais.

## Estrutura

```
ofertasdagigi/
├── index.html          ← página principal (todo o site)
└── assets/
    ├── logo.jpg         ← logo circular
    ├── banner.jpg        ← banner (não usado na página, guardado como referência)
    ├── produto1-escova.jpg
    └── produto2-potes.jpg
```

## Como publicar no GitHub Pages

1. Crie um repositório novo no GitHub (ex: `ofertasdagigi`).
2. Suba os arquivos desta pasta (`index.html` e a pasta `assets/`) para a raiz do repositório.
3. No repositório, vá em **Settings → Pages**.
4. Em "Source", selecione a branch `main` e a pasta `/root`, depois clique em **Save**.
5. Em alguns minutos o site estará disponível em:
   `https://SEU-USUARIO.github.io/ofertasdagigi/`

## Como adicionar uma nova oferta

Abra o `index.html` e, dentro da `<div class="offers">`, copie um bloco `<a class="offer-card">...</a>` inteiro, cole logo abaixo do último, e troque:

- o `href` pelo link da Shopee;
- a imagem em `src="assets/..."` (adicione a nova imagem na pasta `assets/`);
- o texto do `offer-title`;
- os preços em `price-old` / `price-new` (apague o `price-old` se não houver preço "de");
- o `alt` da imagem.

Não é necessário mexer em nenhuma outra parte do código.
