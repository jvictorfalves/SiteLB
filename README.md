# La Bella - Loja Virtual de Maquiagem

## Descrição

O **La Bella** é uma loja virtual de maquiagem que oferece uma experiência de compra online acessível e intuitiva. A página é responsiva e utiliza HTML, CSS e JavaScript para proporcionar uma navegação fluida, com foco em produtos de beleza e atendimento ao cliente.

## Funcionalidades

- **Carrinho de Compras**: Permite aos usuários adicionar produtos ao carrinho, visualizar o total e remover itens antes de finalizar a compra.
- **Visualização de Produtos**: Exibe produtos com imagens e preços. O layout é dinâmico e responsivo, adaptando-se a diferentes tamanhos de tela.
- **Seção de Loja Física**: Apresenta informações sobre a loja física, com fotos e detalhes sobre o local.
- **Seção de Dúvidas Frequentes**: Exibe uma lista de perguntas comuns com ícones representando cada item.
- **Barra de Navegação**: Links para as páginas 'Sobre Nós', 'Produtos' e 'Contato'.
- **Rodapé com Informações**: Contém informações sobre a loja, incluindo redes sociais e contatos.

## Estrutura do Código

### HTML

O código HTML define a estrutura básica do site, com seções como cabeçalho, produtos, carrinho, informações sobre a loja física, dúvidas frequentes e rodapé. A navegação é feita por meio de links e ícones de redes sociais.

### CSS

O estilo da página é moderno e clean, utilizando uma paleta de cores com tons de dourado e preto. O layout é responsivo, ajustando-se bem a diferentes tamanhos de tela, com foco em uma experiência de usuário otimizada para desktop e dispositivos móveis.

**Exemplo de Estilos Importantes**:
- O fundo da página é definido como uma imagem de fundo fixa, com o uso de `background-size: cover` e `background-attachment: fixed` para um efeito visual atrativo.
- A barra de navegação tem links que alteram de cor com o hover, destacando o tom dourado.
- Os produtos são exibidos em cards com imagens e preços, com transições suaves para efeitos de hover.

### JavaScript

O JavaScript gerencia as funcionalidades do carrinho de compras, permitindo adicionar e remover produtos, além de atualizar o total da compra. A função `toggleCarrinho()` é usada para mostrar ou esconder o carrinho de compras, enquanto `adicionarAoCarrinho()` e `removerDoCarrinho()` gerenciam os itens no carrinho.

**Funções Principais**:
- **toggleCarrinho()**: Exibe ou oculta o carrinho suspenso na tela.
- **adicionarAoCarrinho(produto, preco)**: Adiciona um produto ao carrinho e atualiza o total.
- **atualizarCarrinho()**: Atualiza o conteúdo visual do carrinho, incluindo os itens e o total.
- **removerDoCarrinho(index)**: Remove um item específico do carrinho.
- **finalizarCompra()**: Finaliza a compra e limpa o carrinho.

## Responsividade

O site foi projetado para ser responsivo, ajustando-se adequadamente a diferentes tamanhos de tela:
- Para telas menores que 768px (como dispositivos móveis), o layout da barra de navegação e dos ícones de redes sociais é reorganizado para uma coluna, melhorando a usabilidade.

### Exemplo de Responsividade:
```css
@media (max-width: 768px) {
    .header-content {
        flex-direction: column;
        align-items: center;
    }

    .navbar {
        flex-direction: column;
        align-items: center;
    }

    .social-icons {
        margin-top: 1rem;
    }
}
