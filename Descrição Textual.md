Trabalho Prático de Laboratório de Programação II — C3

Grupo de Desenvolvimento

* Riquelme Corrêa de Lima
* Jeferson Lucas da Silva Almeida
* João Victor Moreira de Carvalho Rangel
* Filipe Ferreira Stofel

 Sistema de Locação de Carros

O Sistema de Locação de Carros tem como objetivo auxiliar empresas de aluguel de veículos no gerenciamento de sua frota, clientes e contratos de locação, permitindo o controle eficiente das reservas, locações e devoluções dos automóveis.

O sistema será utilizado por funcionários e administradores da locadora, possibilitando o cadastro de veículos e clientes, consulta de informações, registro de locações e devoluções, além do acompanhamento da disponibilidade da frota.

Funcionalidades Principais

* Cadastro de veículos;
* Cadastro de clientes;
* Consulta de veículos cadastrados;
* Consulta de clientes cadastrados;
* Atualização de informações dos veículos;
* Atualização de informações dos clientes;
* Registro de locação de veículos;
* Registro de devolução de veículos;
* Consulta da disponibilidade dos veículos;
* Geração de relatórios simples de locações;
* Armazenamento dos dados em arquivo.

Benefícios

* Melhor organização da frota;
* Controle eficiente das locações;
* Facilidade na consulta de clientes e veículos;
* Redução de erros no processo de aluguel;
* Agilidade no atendimento aos clientes.

 Regras de Negócio

* Cada veículo deve possuir uma placa única.
* Não é permitido cadastrar veículos com valor de diária menor ou igual a zero.
* Não é permitido cadastrar veículos sem modelo ou marca.
* Cada cliente deve possuir um CPF único.
* Não é permitido cadastrar clientes menores de 18 anos.
* Um veículo só pode ser locado se estiver disponível.
* A locação deve registrar a data de retirada e a previsão de devolução.
* A devolução deve alterar o status do veículo para disponível.
* Não é permitido excluir veículos que possuam locações registradas.
* Toda locação e devolução deve ser registrada em arquivo.
* O sistema deve emitir um alerta para veículos com manutenção pendente.

Organização das Tarefas (Trello)

Etapa 1 – Planejamento

* Definição dos requisitos do sistema;
* Levantamento das funcionalidades;
* Criação da descrição do projeto.

Etapa 2 – Modelagem

* Desenvolvimento do diagrama de classes UML;
* Definição dos atributos e métodos das classes;
* Organização dos pacotes.

Etapa 3 – Desenvolvimento

* Implementação da classe Veiculo;
* Implementação da classe Cliente;
* Implementação da classe Locacao;
* Implementação da classe Frota;
* Implementação do menu principal;
* Implementação da persistência em arquivos.

Etapa 4 – Testes

* Testes de cadastro de veículos;
* Testes de cadastro de clientes;
* Testes de locação e devolução;
* Testes de gravação e leitura dos arquivos;
* Correção de erros.

Etapa 5 – Documentação

* Elaboração do relatório;
* Captura de telas;
* Revisão do código.

 Etapa 6 – Apresentação

* Preparação dos slides;
* Demonstração do sistema.

 Possíveis Classes

 1. Veiculo

* placa
* marca
* modelo
* ano
* valorDiaria
* disponivel

 2. Cliente

* cpf
* nome
* telefone
* idade
* endereco

 3. Frota

* lista de veículos

 Métodos

* cadastrarVeiculo()
* removerVeiculo()
* buscarVeiculo()
* listarVeiculosDisponiveis()

 4. Locaçao

* cliente
* veiculo
* dataRetirada
* dataDevolucaoPrevista
* dataDevolucaoReal

 Métodos

* registrarLocacao()
* registrarDevolucao()
* calcularValorLocacao()
