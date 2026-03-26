## Sobre o projeto

Este projeto é um pequeno sistema front-end em HTML/CSS que simula um compêndio para mestres e jogadores de RPG (D&D). Inclui páginas de navegação, cadastro de personagem, listagem, dashboard de estatísticas e consulta de raças.

- Linguagens: HTML, CSS
- Framework CSS: Bootstrap 5 (via CDN)
- Biblioteca de gráfico: Chart.js (no dashboard)

## Navegação e estrutura

Arquivos:
- `index.html` - página inicial com cards de introdução e links.
- `cadastro.html` - formulário de cadastro de personagem.
- `listagem.html` - listagem de itens/monstros com tabela responsiva.
- `dashboard.html` - cards de métricas + gráfico de barras.
- `racas.html` - cards das raças disponíveis.

## Componentes Bootstrap usados e explicação por página

### Navegação comum (todas as páginas)
- `navbar navbar-expand-lg navbar-dark bg-dark`: barra de navegação responsiva com tema escuro.
- `container-fluid`: container fluido para mantê-la esticada na largura.
- `navbar-toggler` + `collapse navbar-collapse`: botão hambúrguer + painel expansível em telas pequenas.
- `navbar-nav ms-auto`: menu alinhado à direita.

### index.html
- `container`, `row`, `col-md-6`: grid de cards principais.
- `card`, `card-body`, `card-title`: cartões informativos.
- `btn btn-primary` e `btn btn-secondary`: botões com estilo Bootstrap.

### cadastro.html
- `row justify-content-center` + `col-md-6`: formulário centralizado em telas médias e grandes.
- `form-control`, `form-label`, `form-select`, `btn btn-primary`: campos e botão estilizados.

### listagem.html
- `row`, `col-12 col-md-8`, `col-12 col-md-4`: layout de filtro e busca adaptável.
- `table-responsive`: torna a tabela rolável em telas menores.
- `table table-hover align-middle` e `table-light`: tabela com estilo e interatividade.

### dashboard.html
- `row`, `col-md-4`: cards de métricas em 3 colunas (empilhadas em móvel).
- `card text-white bg-primary`, `bg-success`, `bg-warning`: indicadores com cores.
- `canvas` + Chart.js: gráfico de barras gerado dinamicamente.

### racas.html
- `row`, `col-md-4`: cards de raças com layout em grade.
- `card`, `card-header`, `card-body`, `list-group`: informações estruturadas de cada raça.

## Responsividade

O projeto usa o sistema de grid do Bootstrap para adaptar o layout a diferentes larguras:

- `col-md-*`: define colunas em telas >= 768px e empilha em telas menores.
- `navbar-expand-lg`: o menu vira hambúrguer em telas menores que 992px.
- `table-responsive`: barras de rolagem horizontais em tabelas longas em telas pequenas.
- `container` e `container-fluid` mantém espaçamento adequado em dispositivos móveis.

## Observações

- A maior parte do conteúdo é estática e demonstra layout e componentes Bootstrap.