# Projeto Minimercado Web - Fase 2: Dinamismo e Interatividade no HTML

Este repositório apresenta as implementações e melhorias realizadas na Fase 2 do sistema web do Minimercado, que segue o desenvolvimento iniciado na Fase 1. O foco desta etapa foi tornar o sistema mais atrativo e dinâmico, além de incluir funcionalidades essenciais como cadastro de clientes e agendamento de serviços.

## Sumário

* [Sobre a Fase 2](#sobre-a-fase-2)
* [Novas Funcionalidades e Melhorias](#novas-funcionalidades-e-melhorias)
* [Estrutura do Projeto](#estrutura-do-projeto)
* [Como Executar](#como-executar)
* [Tecnologias Utilizadas](#tecnologias-utilizadas)
* [Acessibilidade](#acessibilidade)
* [Autor](#autor)

## Sobre a Fase 2

A Fase 2 do projeto Minimercado Web concentrou-se na modernização da interface e na adição de funcionalidades interativas e de gerenciamento de dados do cliente. As principais metas foram:
* Aprimorar a experiência visual e de uso com um design responsivo.
* Incluir elementos dinâmicos para tornar a navegação mais envolvente.
* Desenvolver um formulário completo para cadastro de clientes.
* Implementar um sistema de agendamento para entrega ou retirada de pedidos.
* Garantir maior acessibilidade ao site.

## Novas Funcionalidades e Melhorias

As seguintes funcionalidades e melhorias foram implementadas na Fase 2:

1.  **Design Responsivo com Bootstrap:**
    * Todas as páginas (`index.html`, `frutas.html`, `alimentos.html`, `higiene.html`, `servicos.html`, `cadastro.html`) foram reestruturadas e estilizadas utilizando o framework CSS Bootstrap 5.
    * Isso garante que o layout do site se adapte de forma otimizada a diferentes tamanhos de tela, desde desktops até dispositivos móveis.
    * Elementos como o cabeçalho (`navbar`) e o rodapé foram padronizados para consistência visual.
    * As listagens de produtos nas páginas de categorias foram convertidas de tabelas simples para `Cards` do Bootstrap, oferecendo uma apresentação mais moderna e flexível.

2.  **Carrossel de Imagens (Homepage):**
    * A página inicial (`index.html`) agora conta com um carrossel interativo do Bootstrap.
    * Este componente exibe imagens de produtos ou promoções em destaque, adicionando dinamismo e atratividade à primeira impressão do site.

3.  **Formulário de Cadastro do Cliente:**
    * Criada uma nova página dedicada ao cadastro de clientes: `cadastro.html`.
    * O formulário inclui diversos tipos de campos HTML (`input type="text"`, `email`, `tel`, `radio`, `select`, `checkbox`) com uso de `placeholder` e atributos `required` para validação.
    * **Validação em JavaScript:** Implementação de validação cliente-side para campos obrigatórios e formatos específicos (e.g., CPF, CEP, Telefone), utilizando a validação nativa do Bootstrap com JavaScript para feedback ao usuário.
    * **Formatação Automática:** Adição de funções JavaScript para formatar o CPF, CEP e Telefone em tempo real enquanto o usuário digita, melhorando a usabilidade.
    * Exemplo de inclusão de `Modal` para exibir "Termos de Serviço".

4.  **Agendamento de Serviços:**
    * Na página `servicos.html`, a seção de agendamento foi aprimorada.
    * Inclusão de campos para seleção de **data (`input type="date"`)** e **horário (`input type="time"`)** do agendamento, utilizando elementos HTML5 para uma interface de calendário e relógio.
    * **Lógica Dinâmica com JavaScript:** O formulário de endereço de entrega agora é exibido ou ocultado dinamicamente com base na escolha entre "Retirada Local" ou "Tele-entrega".
    * Validação em JavaScript para garantir que data e hora sejam selecionadas, e que os campos de endereço sejam preenchidos caso a "Tele-entrega" seja escolhida.

5.  **Acessibilidade:**
    * **Atributo `alt` em Imagens:** Todas as tags `<img>` em todas as páginas foram revisadas e o atributo `alt` foi preenchido com descrições concisas e relevantes. Isso é crucial para usuários de leitores de tela, que dependem dessas descrições para entender o conteúdo visual.
    * **Associação de `Label`s:** O uso correto do atributo `for` nas tags `<label>` e a sua associação aos `input`s correspondentes foram implementados em todos os formulários, melhorando a navegação por teclado e a compreensão do formulário por tecnologias assistivas.

## Estrutura do Projeto

A estrutura do projeto, com a adição da nova página `cadastro.html`, é a seguinte:

├── index.html
├── frutas.html
├── alimentos.html
├── higiene.html
├── servicos.html
├── cadastro.html             <- NOVA PÁGINA
├── logo.png                  (Recurso de imagem)
├── arroz.jpg                 (Recurso de imagem)
├── chuchu.jpg                (Recurso de imagem)
├── feijao.jpg                (Recurso de imagem)
├── maca.jpg                  (Recurso de imagem)
├── papel.jpg                 (Recurso de imagem)
└── sabonete.jpg              (Recurso de imagem)

## Como Executar

Para visualizar o site desenvolvido na Fase 2, basta abrir qualquer um dos arquivos `.html` (recomendado iniciar por `index.html`) em seu navegador web preferido (Google Chrome, Mozilla Firefox, Microsoft Edge, etc.). Por ser um projeto puramente front-end, não é necessário configurar um servidor web.

## Tecnologias Utilizadas

* **HTML5:** Para a estrutura semântica das páginas web.
* **CSS3:** Para a estilização e apresentação.
* **Bootstrap 5.3.3:** Framework CSS moderno para design responsivo e componentes de interface de usuário, incluindo carrossel e formulários estilizados.
* **JavaScript (ES6+):** Utilizado para adicionar interatividade, validações de formulário complexas, lógica de exibição dinâmica e formatação de campos.

## Acessibilidade

A acessibilidade foi um requisito fundamental na Fase 2. A implementação de atributos `alt` completos em todas as imagens e a correta associação de `labels` em formulários visam garantir que o conteúdo seja compreensível e navegável por um público mais amplo, incluindo usuários com deficiência visual que utilizam leitores de tela.

## Autor

Robson Valentim
