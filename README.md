# OO Comidinhas Veganas

Este projeto é parte do Trabalho Prático da disciplina de Programação Orientada por Objetos do curso de Bacharelado em Sistemas de Informação da PUC Minas, orientado pelo professor João Caram.

## Descrição do Projeto

O projeto "OO Comidinhas Veganas" visa desenvolver um sistema de gerenciamento para um restaurante vegano e uma cafeteria, com funcionalidades para alocação de mesas, atendimento de clientes, gerenciamento de pedidos e geração de contas. O projeto foi desenvolvido em três sprints, cada uma adicionando novas funcionalidades ao sistema.

## Funcionalidades

### Sprint 1
- **Alocação de Mesas:** O sistema aloca mesas para os clientes com base no número de pessoas.
- **Fila de Espera:** Caso todas as mesas estejam ocupadas, os clientes são colocados em uma fila de espera.

### Sprint 2
- **Cardápio do Restaurante:** Adição de um cardápio com seis pratos e cinco bebidas.
- **Gestão de Pedidos:** Os clientes podem realizar pedidos ilimitados de pratos e bebidas durante o atendimento.
- **Fechamento de Conta:** O sistema calcula a conta com uma taxa de serviço de 10% e permite a divisão do valor entre os ocupantes da mesa.

### Sprint 3
- **Expansão para Cafeteria:** O sistema foi expandido para incluir uma cafeteria que oferece um cardápio de lanches rápidos e bebidas. Não há fila de espera, e os clientes podem se sentar em mesas livres por conta própria.

## Tecnologias e Conceitos de POO Utilizados

Durante o desenvolvimento do projeto, foram aplicados diversos conceitos e tecnologias de Programação Orientada a Objetos, como:

- **Herança:** A classe `Estabelecimento` serve como uma classe base para as classes `Restaurante` e `Cafeteria`, permitindo que compartilhem atributos e métodos comuns, enquanto implementam funcionalidades específicas de cada tipo de estabelecimento.

- **Polimorfismo:** Implementado através da interface `ICardapio`, que define métodos que devem ser implementados por qualquer classe que represente um cardápio, como `CardapioRestaurante` e `CardapioCafeteria`. Isso permite que o sistema trate diferentes tipos de cardápios de forma unificada.

- **Encapsulamento:** Cada classe no projeto encapsula seus dados e expõe apenas o que é necessário através de métodos públicos, protegendo a integridade dos dados e facilitando a manutenção do código.

- **Modularidade:** O projeto foi estruturado em diferentes classes que representam entidades do domínio, como `Cliente`, `Mesa`, `Pedido`, entre outras. Essa modularidade facilita a compreensão, manutenção e evolução do sistema.

- **Composição:** O conceito de composição é utilizado, por exemplo, na relação entre `Pedido` e `Produto`, onde um pedido é composto por múltiplos produtos, representando assim a relação "tem-um" entre essas classes.

## Estrutura do Projeto

- **Cafeteria.cs:** Implementa as funcionalidades específicas da cafeteria.
- **CardapioCafeteria.cs:** Contém os itens do cardápio da cafeteria.
- **CardapioRestaurante.cs:** Contém os itens do cardápio do restaurante.
- **Cliente.cs:** Representa os clientes do restaurante e da cafeteria.
- **Estabelecimento.cs:** Classe base para Restaurante e Cafeteria.
- **ICardapio.cs:** Interface para implementação de cardápios.
- **Mesa.cs:** Representa uma mesa no estabelecimento.
- **Pedido.cs:** Gerencia os pedidos feitos pelos clientes.
- **Produto.cs:** Representa os produtos disponíveis no cardápio.
- **Reserva.cs:** Gerencia as reservas de mesas.
- **Restaurante.cs:** Implementa as funcionalidades específicas do restaurante.
- **Program.cs:** Ponto de entrada do sistema.

## Requisitos

- .NET Core 6.0 ou superior
- IDE: Visual Studio 2022 ou Visual Studio Code

## Diagrama de Classes

O diagrama de classes do projeto pode ser encontrado na pasta `docs` do repositório.

## Contribuições

Este projeto foi desenvolvido em equipe, e cada membro contribuiu com diferentes partes do código e documentação. Qualquer sugestão ou melhoria é bem-vinda!

## Licença

Este projeto é de uso acadêmico e segue as diretrizes da PUC Minas para trabalhos práticos.
