# Verificação do Módulo 02

Data: 16/11/2026. Testes automatizados no Microsoft Edge, com controlo pelo protocolo DevTools e um servidor HTTP local temporário. Não foram acrescentados scripts às páginas.

## Resultados

- As dez páginas (índice e nove exercícios) abriram no navegador com a respetiva folha de estilos carregada.
- Verificados 81 caminhos e referências locais em HTML, incluindo folhas de estilos, imagens, ligações entre exercícios e destinos internos. Todos os caminhos novos são válidos.
- Os seis ficheiros de ex01, ex02 e ex03 mantêm exatamente os hashes SHA-256 registados antes do trabalho.
- Ex04: todos os labels estão associados a campos; o botão de limpar repôs os valores; o envio está desativado. Uma tecla Tab moveu o foco de Nome para Email, com contorno azul de 3px confirmado no estilo calculado.
- Ex05: confirmados os estilos calculados das seis demonstrações. No teste a 1024px, o cartão de crescimento duplo ficou maior do que os restantes; no encolhimento, A mediu 213px e B 159px, partindo ambos de 240px.
- Ex06: a 320px, o menu abriu e fechou com a tecla Espaço no summary. A 1024px, o menu móvel estava oculto e a navegação completa usava Flexbox.
- Ex07: as quatro fotografias locais foram descodificadas pelo navegador e têm texto alternativo. Dimensões: 1400×933, 1100×733, 1100×732 e 1100×733px. Composição da galeria inspecionada numa captura do Edge a 1024px.
- Ex08: a 320px, as áreas Grid ficaram empilhadas. A tabela manteve 740px dentro de uma região deslocável, sem alargar a página. Depois de focada, a tecla de seta para a direita deslocou a tabela 40px. Os seis pedidos correspondem aos indicadores: dois em diagnóstico, dois em reparação e dois concluídos.
- Ex04 a ex08: verificados a 320, 768, 1024 e 1440px, sem deslocamento horizontal da página.
- Ex09: oito verificações, quatro larguras em cada tema. Em todas, a largura de deslocamento do documento não excedeu a área útil da janela. Confirmada a alteração de fundo e a reorganização das colunas; inspecionadas capturas do layout móvel e do tema escuro em ecrã largo.

| Largura da janela | Tema claro | Tema escuro |
| --- | --- | --- |
| 320px | Sem deslocamento horizontal | Sem deslocamento horizontal |
| 768px | Sem deslocamento horizontal | Sem deslocamento horizontal |
| 1024px | Sem deslocamento horizontal | Sem deslocamento horizontal |
| 1440px | Sem deslocamento horizontal | Sem deslocamento horizontal |

As larguras foram simuladas no Edge; não equivalem a testes em dispositivos físicos.

## Problemas anteriores preservados

No ex01, os links originais para `#inicio`, `#seletores` e `#contactos` não têm elementos com esses IDs. Foram identificados durante a verificação e preservados, porque o pedido exige manter ex01 sem alterações.

## Limites e pontos não testados

- Não foram testados Firefox, Safari, dispositivos físicos, leitores de ecrã ou ampliação da página.
- Não foi feita uma auditoria completa de acessibilidade nem uma inspeção visual de todas as secções em todas as larguras. Foram verificados os comportamentos e medidas descritos acima.
- Não foi possível validar em direto todas as páginas externas de atribuição: algumas consultas ao Unsplash devolveram HTTP 401 ou erro de acesso. As quatro fotografias foram descarregadas, os ficheiros locais carregam e as fontes estão registadas em ex07/FONTES.md. As páginas de Luca Bravo, Florian Olivo e a licença foram consultadas quando acessíveis.
- Não existe envio real de formulários, gravação de pedidos ou servidor de aplicação; são páginas demonstrativas em HTML e CSS.
