# ✨ Portfólio Profissional - Desenvolvimento de Sistemas

Nome do aluno: Pietro França Gomes

# 🚀 Descrição do portfólio

Este é um portfólio profissional desenvolvido como parte das atividades da Agenda 15 do curso Técnico em Desenvolvimento de Sistemas. O projeto consiste em uma página web responsiva criada para apresentar meu perfil, habilidades técnicas, trajetória acadêmica e os principais projetos práticos desenvolvidos ao longo do curso.

### Link do site publicado 

🌐 Acesse o portfólio online: https://pietrofran12.github.io/portfolio/

# 🛠️ Tecnologias utilizadas

HTML5: Estruturação semântica do conteúdo da página.

CSS3: Estilização personalizada, transições e efeitos visuais.

Bootstrap 5: Framework CSS utilizado para o sistema de grid, layout responsivo e componentes prontos (Navbar, Carousel, Cards, Botões).

Devicon: Biblioteca externa de ícones utilizada na seção de habilidades para ilustrar as linguagens e ferramentas.

![Bootstrap](https://img.shields.io/badge/Bootstrap-black?style=for-the-badge&logo=bootstrap
)
![CSS3](https://img.shields.io/badge/CSS3-%23663399?style=for-the-badge&logo=CSS
)
![HTML5](https://img.shields.io/badge/HTML-white?style=for-the-badge&logo=html5
)

# 📌 Explicação do funcionamento do projeto

O projeto funciona como uma Single Page Application (SPA) estática. Toda a navegação ocorre em uma única página através do menu superior fixo (Navbar). Quando o usuário clica em um link do menu, a página rola suavemente até a respectiva seção, identificada por um id específico (ex: #perfil, #projetos). O design é totalmente responsivo, ou seja, os elementos (como os cards e o carrossel) se reorganizam automaticamente para se adaptar a diferentes tamanhos de tela, como celulares, tablets ou monitores desktop, graças ao sistema de colunas (col-md, col-lg) do Bootstrap.

### Descrição do recurso novo adicionado

Para ir além do modelo base proposto em aula, foram adicionados três recursos novos:

Animação de Hover nos Cards: Um efeito visual interativo onde os cards da seção "Projetos" aumentam levemente de tamanho e ganham uma sombra ao passar o mouse por cima.

Nova Seção de Formação com Iframe: Uma área extra adicionada entre o "Perfil" e os "Projetos" contendo detalhes da trajetória acadêmica e a inclusão de um vídeo do YouTube embutido.

Rolagem Suave (Smooth Scroll): Um comportamento que torna a navegação pelos links internos do menu muito mais fluida, eliminando o "salto" abrupto direto para a seção.

### Explicação de como esse recurso foi implementado

Animação de Hover: Implementada através de CSS personalizado no `<head>`. Foi criada uma classe .hover-scale que utiliza as propriedades transition: transform 0.3s ease, box-shadow 0.3s ease;. No pseudo-estilo :hover, foi aplicado transform: scale(1.05) para aumentar o tamanho em 5% e adicionada uma sombra mais forte. Essa classe foi então inserida nas divs dos cards de projetos.

Seção com Iframe: Foi criada uma nova `<section id="formacao">`. Para o vídeo, utilizou-se a tag HTML `<iframe>` apontando para o link de incorporação do YouTube. Para garantir que o vídeo não perdesse a proporção no celular, ele foi envolvido em uma div com a classe utilitária do Bootstrap ratio ratio-16x9.

Rolagem Suave: Implementada de forma muito simples e eficiente utilizando CSS puro. Adicionei a regra scroll-behavior: smooth; diretamente no seletor html dentro da tag `<style>`, alterando o comportamento padrão de navegação das âncoras da página inteira.