# Olhar Fino — Shopify Theme (Online Store 2.0)

Tema mínimo e dark, pronto para GitHub + Shopify.

## Estrutura
- `layout/theme.liquid`: shell do tema
- `sections/`: header, footer, hero, product-grid
- `snippets/product-card.liquid`: card de produto com botão Comprar
- `assets/theme.css.liquid`: estilos com paleta dark
- `config/settings_schema.json`: configurações (menu, cor primária, redes)
- `locales/`: traduções PT-BR e EN
- `templates/index.json`: homepage com hero + grid

## Publicar via GitHub
1. Crie um repositório e suba esses arquivos (raiz do repo = raiz do tema).
2. Na Shopify: Online Store → Themes → Add theme → Connect from GitHub → selecione o repo/branch.
3. Abra **Customize** para configurar imagens/coleções.

## Dev local (opcional)
```bash
npm i -g @shopify/cli @shopify/theme
shopify login --store sua-loja.myshopify.com
shopify theme dev
```

## Dicas
- Use o **menu principal** em Settings do tema para popular a navegação do header.
- Troque a paleta pela `primary_color` nas configurações do tema.
- Na seção **Grade de produtos**, selecione a coleção (Feminino, Esportivo, etc.).
