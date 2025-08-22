A simple HTML/JS/CSS starter template
# Padaria da Villa - Site Institucional e Formulários

Este projeto consiste em um site estático simples de apresentação para a Padaria da Villa, destacando nossos produtos artesanais, história, serviços para eventos e formas de contato. O objetivo é oferecer uma presença online que reflita a qualidade e o carinho dos nossos produtos, além de permitir a interação dos clientes através de diversos formulários.


## Funcionalidades Principais

*   Apresentação da Padaria da Villa (História, Produtos, Serviços).
*   Informações sobre serviços para Eventos.
*   **Formulário de Contato Geral:** Para dúvidas, sugestões, reclamações e elogios.
*   **Formulário de Pedidos Especiais:** Para encomendas personalizadas.
*   **Formulário de Feedback:** Para coletar opiniões sobre produtos e serviços.
*   **Formulário de Cadastro/Newsletter:** Para que os clientes recebam promoções e novidades.

## Tecnologias Utilizadas
*   **JavaScript:** Para adicionar interatividade e lógica de negócios ao site.
*   **HTML5:** Para a estrutura das páginas e formulários.


## Funcionalidades JavaScript

Com base nas atividades de desenvolvimento, as seguintes funcionalidades foram implementadas com JavaScript:

*   **Gerenciamento de Variáveis e Tipos de Dados:** Utilização de variáveis para armazenar informações da padaria e dados dinâmicos.
*   **Calculadora de Pedidos:** Lógica para calcular subtotal, descontos, impostos, total geral, troco e pontos de fidelidade.
*   **Manipulação de Strings e Dados:** Funções para formatação de moeda e data/hora, validação de campos de formulário, saudação personalizada e busca de produtos.
*   **Gerenciamento de Arrays e Listas Dinâmicas:**
    *   Gerenciamento do carrinho de compras (adicionar, remover, exibir itens).
    *   Registro e exibição do histórico de pedidos.
    *   Funcionalidade de marcar/desmarcar produtos favoritos.
    *   Cálculo e exibição do ranking de produtos mais vendidos.
    *   Gerenciamento da lista de clientes frequentes (cadastro, exibição, busca).
*   **Objetos e Estruturas Complexas:** Criação e manipulação de objetos para representar produtos, clientes e pedidos completos (incluindo dados de pagamento, observações e endereço de entrega).
*   **CSS:** Utilização de uma paleta de cores em tons terrosos, dourados e avermelhados para um design acolhedor.
    *   **Estilização Detalhada:** O arquivo `css/style.css` foi organizado em seções comentadas (Reset, Layout, Componentes, Utilitários) para melhor manutenção. Foram utilizados seletores de elemento, classe, ID, seletores descendentes e pseudo-classes (`:hover`) para aplicar estilos específicos aos elementos da página. Variáveis CSS (`:root`) foram empregadas para gerenciar a paleta de cores de forma centralizada.
    *   **Classes Utilitárias:** Foram criadas classes utilitárias reutilizáveis (ex: `.text-center`, `.margin-top-10`, `.color-primary`) para facilitar a aplicação de estilos comuns.
 * **Atualizações Recentes:**
 * A paleta de cores no arquivo `css/style.css` foi atualizada e organizada utilizando variáveis CSS dentro do seletor `:root`.
 * Novas variáveis de cor foram adicionadas com nomes descritivos (ex: `--cor-fundo-claro`, `--cor-texto-geral`, `--cor-elementos-interativos`, etc.) para melhorar a legibilidade e facilitar futuras modificações.
 * O código CSS foi revisado para garantir uma estrutura mais limpa e organizada, com comentários claros para cada seção (Reset, Layout, etc.).



## Estrutura de Arquivos

O projeto segue a seguinte estrutura (simplificada):



## Como Visualizar o Projeto

Para visualizar o site localmente, siga estes passos:

1.  Clone este repositório para o seu computador.
2.  Abra o arquivo `index.html` em qualquer navegador web moderno (como Google Chrome, Firefox, Safari, Edge, etc.).
3.  Navegue pelas páginas utilizando o menu no cabeçalho.

## Como Utilizar os Formulários

Os formulários são a parte interativa do site. Para que os dados enviados pelos usuários cheguem até você, é necessário implementar um **sistema de back-end**. Este projeto foca no front-end com HTML e CSS, e a funcionalidade de envio dos formulários precisaria ser desenvolvida em outra camada (por exemplo, com JavaScript para enviar dados para um servidor, ou configurando um serviço de formulário de terceiros).

## Otimizações de Responsividade e Performance (Trabalho Recente)

Foram realizadas diversas otimizações para tornar o site responsivo e melhorar sua performance, especialmente em dispositivos móveis.

### Imagens e Mídia Responsiva

**🎯 Objetivo:** Otimizar imagens e mídias para múltiplas resoluções e conexões.

*   **Implementação de imagens responsivas:** Regra CSS `max-width: 100%; height: auto;` adicionada a todas as imagens para garantir que se ajustem aos seus contêineres.
*   **Uso da tag `<picture>`:** A primeira imagem da fachada no `index.html` foi envolvida pela tag `<picture>` para permitir a exibição de diferentes versões da imagem dependendo do tamanho da tela (requer a criação manual das versões das imagens).
*   **Implementação de lazy loading:** O atributo `loading="lazy"` foi adicionado às tags `<img>` no `index.html` para atrasar o carregamento de imagens fora da viewport, melhorando o tempo de carregamento inicial da página.
*   **Otimização de vídeo:** O iframe do vídeo do YouTube no `index.html` foi envolvido em uma div com a classe `video-container` e regras CSS foram adicionadas para torná-lo responsivo, mantendo a proporção em diferentes tamanhos de tela.

### Componentes e Interações Responsivas

**🎯 Objetivo:** Criar componentes adaptáveis e funcionais em qualquer dispositivo.

*   **Cards responsivos:** Regras CSS com Flexbox e media queries foram adicionadas para que os cards de produto na seção "Nossos Produtos" se reorganizem em telas menores, empilhando-se e ajustando sua largura.
*   **Formulários adaptáveis:** Regras CSS foram adicionadas para que os elementos dos formulários se empilhem verticalmente e os campos de input ocupem a largura total em telas pequenas, melhorando a usabilidade mobile.
*   **Botões touch-friendly:** Regras CSS foram adicionadas para garantir uma área de toque mínima de 44x44 pixels para os botões de submit em telas menores, facilitando o clique em dispositivos touch.
*   **Tabelas adaptadas:** As tabelas no `index.html` foram envolvidas em divs com a classe `table-responsive` e regras CSS foram adicionadas para permitir scroll horizontal em telas pequenas, garantindo a visualização de todo o conteúdo.
*   **Modais responsivos:** A estrutura HTML básica para um modal foi adicionada ao `index.html` e regras CSS foram adicionadas para posicionar e dimensionar o modal de forma responsiva (a funcionalidade de abrir/fechar requer JavaScript).
*   **Carrossel/slider responsivo:** A estrutura HTML básica para um carrossel foi adicionada à seção "Nossos Produtos" no `index.html` e regras CSS foram adicionadas para estilizar os slides, contêiner e navegação de forma responsiva (a funcionalidade de troca de slides requer JavaScript).
*   **Otimização de estados de hover:** Regras CSS foram modificadas para que o conteúdo dos tooltips nos cards de produto seja visível por padrão em telas menores, eliminando a dependência do estado de hover em dispositivos touch.

### Testes e Otimização

**🎯 Objetivo:** Validar responsividade em diferentes dispositivos e cenários.

*   **Testes de Tamanho de Tela (DevTools):** Validação visual da adaptação do layout em diversas dimensões de tela usando o Device Mode. Resultado: OK.
*   **Validação de Performance Mobile (Lighthouse/PageSpeed Insights):** Auditoria para medir métricas de velocidade e interatividade em mobile. Resultado: OK.
*   **Verificação de Acessibilidade (Lighthouse):** Auditoria para identificar problemas de acessibilidade em mobile. Resultado: OK.
*   **Testes de Orientação (Portrait/Landscape):** Verificação da adaptação do layout ao alternar entre orientações vertical e horizontal. Resultado: OK.
*   **Validação de Carregamento em 3G:** Teste de carregamento simulando uma conexão 3G para avaliar o desempenho em redes mais lentas. Resultado: OK.


## Autor

[Luciana Souza Siqueira]
