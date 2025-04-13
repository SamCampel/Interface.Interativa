# Interface Interativa Atualizando CSS com JavaScript

Este projeto demonstra como atualizar variáveis CSS em tempo real utilizando JavaScript. Ele permite que o usuário ajuste dinamicamente o espaçamento, o desfoque e a cor base de uma imagem através de controles interativos.
Foi desenvolvido juntamente ao curso JavaScript30.

## Funcionalidades

- **Controle de Espaçamento**: Ajusta o espaçamento ao redor da imagem.
- **Controle de Desfoque**: Aplica um efeito de desfoque na imagem.
- **Controle de Cor Base**: Altera a cor de fundo da imagem.

## Estrutura do Projeto

O projeto é composto por um único arquivo HTML que contém:

- **HTML**: Estrutura da página, incluindo os controles e a imagem.
- **CSS**: Estilização da página e uso de variáveis CSS para propriedades dinâmicas.
- **JavaScript**: Lógica para atualizar as variáveis CSS com base nos valores dos controles.

## Pré-visualização

A interface inclui:

- Um título descritivo.
- Controles deslizantes para ajustar o espaçamento e o desfoque.
- Um seletor de cor para alterar a cor base.
- Uma imagem que reflete as alterações em tempo real.

## Como Usar

1. Faça o download ou clone este repositório.
2. Abra o arquivo `CSSVariables_&JS.html` em qualquer navegador moderno.
3. Use os controles para ajustar o espaçamento, desfoque e cor base da imagem.

## Código Principal

### CSS
As variáveis CSS são definidas no `:root` e aplicadas dinamicamente à imagem.

```css
:root {
    --spacing: 10px;
    --blur: 10px;
    --base: #ffc600;
}

img {
    padding: var(--spacing);
    background: var(--base);
    filter: blur(var(--blur));
    transition: all 0.2s ease;
}
