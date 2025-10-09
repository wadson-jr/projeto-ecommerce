# ecommerce-syntaxwear

Projeto de estudo: layout estático de um e-commerce (loja de tênis / sneakers) chamado SyntaxWear.

Este repositório contém o HTML, CSS e ativos (imagens/ícones) usados para construir a interface estática do site. É um projeto voltado para estudos e prática de layout responsivo, sem backend.

## Tecnologias
- HTML5
- CSS3 (estrutura modular com arquivos em `css/components/`)

## Estrutura do projeto

Raiz resumida:

- `index.html` - página principal
- `css/` - estilos
	- `reset.css`, `variables.css`, `base.css`
	- `components/` — estilos por componente (header, hero, product-grid, footer, etc.)
- `images/` - imagens e ícones usados no layout

## Como abrir e testar localmente

1. Abra o diretório do projeto em um editor (recomendado: VS Code).
2. Use uma extensão de servidor estático (ex.: Live Server) para servir os arquivos e evitar problemas de caminhos relativos.

Exemplo (VS Code):

- Instale a extensão "Live Server".
- Clique com o botão direito em `index.html` → "Open with Live Server".

Alternativamente, você pode rodar um servidor simples com Python (se tiver Python instalado):

```bash
# Python 3
python -m http.server 5500
# então abra http://localhost:5500 no navegador
```

## Notas de desenvolvimento
- Os estilos estão organizados em `css/components/` para facilitar manutenção.
- Os caminhos de imagens usam referências relativas (por exemplo `./images/...`). Se imagens não carregarem, verifique nomes, maiúsculas/minúsculas e se o servidor está servindo os arquivos (evite abrir via `file://`).
- Para adicionar ícones, prefira SVGs inline ou sprites para melhor controle de cor e acessibilidade.

## Próximos passos
- Ajustar e completar a responsividade (breakpoints menores).
- Adicionar interações JS (menu mobile, filtros, carrinho simulado).
- Refatorar caminhos de imagens removendo espaços/acentos nos nomes (recomendado para evitar problemas em servidores case-sensitive).

---