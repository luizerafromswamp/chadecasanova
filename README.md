# Chá de Casa Nova - Site de Lista de Presentes

Este é um site estático simples para gerenciar uma lista de presentes de chá de casa nova.

## Como Editar o Site

### Editando Informações Básicas

1. Abra o arquivo `index.html` em um editor de texto
2. Procure pelos comentários marcados com `<!-- EDITAR: -->`
3. Modifique os seguintes elementos:
   - Nomes do casal (dentro da tag `<h1 class="couple-names">`)
   - Mensagem de boas-vindas (dentro da tag `<p class="header-message">`)

### Adicionando Novos Presentes

1. Localize o bloco de código que começa com `<div class="gift-item">`
2. Copie todo o bloco até o `</div>` correspondente
3. Cole o bloco copiado onde está o comentário `<!-- EDITAR: Adicione mais itens aqui -->`
4. Modifique no novo bloco:
   - Link da imagem (`src` na tag `<img>`)
   - Nome do presente (`<h3 class="gift-name">`)
   - Descrição (`<p class="gift-description">`)
   - Link de compra (`href` no botão "Comprar")
   - Link e mensagem do WhatsApp (`href` no botão "Avisar")

### Marcando um Item como Reservado

1. Adicione a classe `reserved` à `<div class="gift-item">`:
   ```html
   <div class="gift-item reserved">
   ```
2. Substitua os botões por:
   ```html
   <a href="#" class="button buy-button" style="pointer-events: none;">Reservado</a>
   ```

## Como Hospedar o Site

### Opção 1: GitHub Pages (Gratuito)

1. Crie uma conta no GitHub (github.com)
2. Crie um novo repositório
3. Faça upload dos arquivos
4. Ative o GitHub Pages nas configurações do repositório

### Opção 2: Netlify (Gratuito)

1. Crie uma conta no Netlify (netlify.com)
2. Arraste a pasta do site para a área de upload do Netlify
3. O site estará disponível em um subdomínio `.netlify.app`

## Personalizando Cores

Para mudar as cores do site, edite as variáveis CSS no início do arquivo `index.html`:

```css
:root {
    --primary-color: #f5d7db;    /* Cor do cabeçalho */
    --secondary-color: #f7e1e5;  /* Cor dos cartões de presente */
    --text-color: #4a4a4a;       /* Cor do texto */
    --reserved-color: #d3d3d3;   /* Cor dos itens reservados */
}
```
