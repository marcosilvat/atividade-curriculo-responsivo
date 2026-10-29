# Atividade: Currículo Responsivo com `<aside>`, Classes CSS e `@media`

Este repositório contém a versão estilizada e responsiva do currículo de **Marco Antonio Teodoro da Silva**, desenvolvida a partir da análise dos arquivos de referência `curriculo.html` e `curriculo.css`.

## Recursos Utilizados

1. **Tag `<aside class="perfil-info">`**:
   - Utilizada para estruturar a coluna lateral esquerda com foto de perfil, informações de contato, habilidades técnicas e idiomas.
   - Em conjunto com `<main class="curriculo-container">` (`display: flex`), divide o layout proporcionalmente entre a barra lateral (`flex: 1`) e o conteúdo principal `<section class="main-content">` (`flex: 2`).

2. **Media Queries (`@media`)**:
   - `@media (max-width: 900px)`: Ajusta margens e espaçamentos internos e altera o esquema de cores da barra lateral antes de empilhar as colunas.
   - `@media (max-width: 768px)`: Altera `flex-direction: column` em `.curriculo-container`, empilhando o `<aside>` acima do conteúdo principal em tablets e telas médias, além de aplicar destaque visual na borda inferior.
   - `@media (max-width: 600px)`: Reduz os espaçamentos (`padding`) de `body`, `.perfil-info` e `.main-content` para melhor aproveitamento de tela em smartphones.

3. **Classes CSS Aplicadas**:
   - `.curriculo-container`: Contêiner principal Flexbox com largura máxima, bordas arredondadas e sombra.
   - `.perfil-info`, `.header`, `.contato`, `.habilidades`, `.idiomas`: Formatação da coluna lateral e suas listas.
   - `.main-content`, `.resumo`, `.experiencia`, `.item-experiencia`, `.periodo`, `.educacao`, `.item-educacao`, `.ods`: Estruturação e tipografia fluida (`clamp()`) da coluna principal.

## Arquivos Principais

- `curriculo.html` (e `index.html`): Estrutura HTML do currículo.
- `curriculo.css`: Folha de estilos com diretrizes de formatação e responsividade.
- `imagens/` e `icones/`: Foto de perfil e ícones em SVG das tecnologias e redes de contato.
