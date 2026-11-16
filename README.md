*Hugo Nunes* · **881942** · Licenciatura em Informática · 16/11/2026

# Módulo 02 — HTML e CSS

Projeto académico com a identidade visual da Saraiva Tech. Abrir [index.html](index.html) no navegador para consultar os nove exercícios. Não é necessário instalar dependências nem executar um servidor.

## Exercícios

| Pasta | Tema | Demonstração |
| --- | --- | --- |
| [ex01](ex01/index.html) | Seletores CSS | Seis seletores, estados hover e foco. |
| [ex02](ex02/index.html) | Box Model | Conteúdo, padding, borda e margem. |
| [ex03](ex03/index.html) | Typography | Hierarquia tipográfica e variáveis CSS. |
| [ex04](ex04/index.html) | Componentes | Cartões, botões, alertas, etiquetas e formulário. |
| [ex05](ex05/index.html) | Flexbox Playground | Seis experiências com os eixos e a distribuição de espaço. |
| [ex06](ex06/index.html) | Barra de navegação responsiva | Menu adaptável com Flexbox e details. |
| [ex07](ex07/index.html) | Galeria de fotografias | Fotografias locais e áreas nomeadas de CSS Grid. |
| [ex08](ex08/index.html) | Dashboard | Gestão fictícia de reparações organizada com Grid. |
| [ex09](ex09/index.html) | Landing page Mobile First | Layout para telemóvel, media queries e modo escuro. |

## Decisões de implementação

- Cada exercício tem o seu `index.html` e `styles.css`, ligados por um caminho relativo. Apenas HTML e CSS, sem frameworks, JavaScript de aplicação ou fontes externas.
- Os ficheiros de ex01, ex02 e ex03 foram preservados nesta conclusão do módulo. O ex04 não existia e foi criado de raiz.
- Azul-escuro, verde, fundos claros e tipos de letra do sistema mantêm a identidade da Saraiva Tech. As páginas novas incluem foco de teclado visível e estrutura semântica.
- Ex04: classes reutilizáveis `card`, `btn`, `alert`, `badge` e `field`. Todos os campos têm labels associados. O formulário é demonstrativo; o envio está desativado, o botão de limpar funciona e não há armazenamento.
- Ex05: seis layouts identificados demonstram direção, distribuição, alinhamento, quebra de linha, espaçamento, crescimento e encolhimento. A navegação adicional também usa Flexbox.
- Ex06: navegação completa a partir de 768px; abaixo disso, um menu nativo `details/summary` abre e fecha sem JavaScript. Os links apontam para secções reais.
- Ex07: quatro fotografias locais, texto alternativo, legendas e composição com `grid-template-areas` e `grid-area`. O destaque ocupa duas linhas em ecrãs largos. As fotografias são ilustrativas e não representam instalações ou serviços reais da empresa. Fontes em [ex07/FONTES.md](ex07/FONTES.md).
- Ex08: Grid organiza cabeçalho, barra lateral, conteúdo e rodapé. Os indicadores correspondem aos seis pedidos fictícios. Em ecrãs pequenos, as áreas ficam empilhadas e apenas a tabela tem deslocamento horizontal, com uma região focável por teclado.
- Ex09: estilos base para telemóvel e media queries a 768 e 1024px. O modo escuro usa `prefers-color-scheme: dark` e redefine variáveis de cor.
- O conteúdo é demonstrativo: não existem pedidos reais, envio de formulários ou gestão persistente de reparações.

## Verificação

Os resultados dos testes e os limites da verificação estão registados em [VERIFICACAO.md](VERIFICACAO.md).
