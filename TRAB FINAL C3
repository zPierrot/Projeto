 ESPECIFICAÇÃO DO SISTEMA

 Projeto: Sistema de Locação de Carros

 Integrantes

* Riquelme Correa de Lima
* Jeferson Lucas da Silva Almeida
* João Victor Moreira de Carvalho Rangel
* Filipe Ferreira Stofel

 Disciplina

Laboratório de Programação II

 Professor

Rober Marcone Rosi

---

 1. Descrição do Sistema

O Sistema de Locação de Carros tem como objetivo auxiliar uma locadora no controle de clientes, funcionários, veículos e locações realizadas.

O sistema permitirá o cadastro de clientes, funcionários e veículos, além da realização de locações, devoluções e consultas de informações cadastradas. Todos os dados serão armazenados em arquivos para que possam ser recuperados quando o sistema for executado novamente.

O software será desenvolvido utilizando a linguagem Java e os conceitos de Programação Orientada a Objetos estudados durante a disciplina.

---

 2. Objetivos

* Cadastrar clientes.
* Cadastrar funcionários.
* Cadastrar veículos disponíveis para locação.
* Realizar locações de veículos.
* Registrar devoluções.
* Consultar clientes, funcionários, veículos e locações.
* Salvar e recuperar dados em arquivos.

---

 3. Funcionalidades do Sistema

 Módulo Cliente

* Cadastrar cliente.
* Listar clientes.
* Buscar cliente por CPF.
* Atualizar dados do cliente.
* Remover cliente.

 Módulo Funcionário

* Cadastrar funcionário.
* Listar funcionários.
* Buscar funcionário por CPF ou matrícula.
* Atualizar dados do funcionário.
* Remover funcionário.

 Módulo Veículo

* Cadastrar veículo.
* Listar veículos.
* Consultar disponibilidade.
* Atualizar dados do veículo.
* Remover veículo.

 Módulo Locação

* Registrar locação.
* Registrar devolução.
* Calcular valor total da locação.
* Listar locações realizadas.
* Consultar histórico de locações.

---

 4. Estrutura de Classes

 Classe Pessoa

 Atributos

* nome
* cpf
* telefone

 Métodos

* getters e setters
* toString()
* equals()

---

 Classe Cliente (Herança de Pessoa)

 Atributos

* codigoCliente

 Métodos

* getters e setters
* toString()
* equals()

---

 Classe Funcionario (Herança de Pessoa)

 Atributos

* matricula
* cargo

 Métodos

* getters e setters
* toString()
* equals()

---

 Classe Veiculo

 Atributos

* placa
* modelo
* marca
* ano
* valorDiaria
* disponivel

 Métodos

* getters e setters
* toString()
* equals()

---

 Classe Locacao

 Atributos

* cliente
* funcionario
* veiculo
* dataLocacao
* quantidadeDias
* valorTotal

 Métodos

* calcularValor()
* toString()
* equals()

---

 Classe SistemaLocadora

Responsável pelo menu principal e gerenciamento das operações do sistema.

---

 5. Conceitos de POO Utilizados

* Classes e Objetos
* Encapsulamento
* Herança (Pessoa → Cliente e Pessoa → Funcionario)
* Polimorfismo (possível implementação futura)
* Sobrescrita de métodos
* Coleções (ArrayList)
* Tratamento de Exceções
* Persistência de Dados em Arquivos

---

 6. Armazenamento de Dados

Os dados serão armazenados em arquivos utilizando serialização de objetos ou arquivos texto, permitindo que as informações permaneçam salvas mesmo após o encerramento do sistema.

 Arquivos Utilizados

* clientes.dat
* funcionarios.dat
* veiculos.dat
* locacoes.dat

---

 7. Regras de Negócio

1. Um cliente só poderá alugar veículos cadastrados.
2. Um veículo só poderá ser alugado se estiver disponível.
3. Após a locação, o veículo ficará indisponível.
4. Após a devolução, o veículo voltará a ficar disponível.
5. O valor total da locação será calculado pela fórmula:

Valor Total = Valor da Diária × Quantidade de Dias

6. Não será permitido cadastrar clientes ou funcionários com CPF duplicado.
7. Não será permitido cadastrar veículos com placa duplicada.
8. Toda locação deverá estar associada a um funcionário responsável.

---

 8. Menu Principal

1. Cadastrar Cliente
2. Listar Clientes
3. Buscar Cliente
4. Atualizar Cliente
5. Remover Cliente
6. Cadastrar Funcionário
7. Listar Funcionários
8. Buscar Funcionário
9. Atualizar Funcionário
10. Remover Funcionário
11. Cadastrar Veículo
12. Listar Veículos
13. Consultar Disponibilidade
14. Atualizar Veículo
15. Remover Veículo
16. Realizar Locação
17. Registrar Devolução
18. Listar Locações
19. Salvar Dados
20. Sair

---

 9. Requisitos Não Funcionais

* Interface em modo texto (console).
* Fácil utilização.
* Código organizado em pacotes.
* Comentários nas classes e métodos.
* Tratamento de entradas inválidas.
* Baixo consumo de recursos.
* Persistência de dados local.

---

 10. Organização dos Pacotes

 locadora.model

* Pessoa
* Cliente
* Funcionario
* Veiculo
* Locacao

 locadora.service

* GerenciadorClientes
* GerenciadorFuncionarios
* GerenciadorVeiculos
* GerenciadorLocacoes

 locadora.persistence

* ArquivoUtil

 locadora.main

* SistemaLocadora

 11. REGRAS DE NEGÓCIOS 

 7.1 Etapa de Cadastro
Durante o processo de cadastro, o sistema deverá garantir a integridade e a consistência das informações armazenadas. Não será permitido cadastrar clientes com CPF duplicado, funcionários com CPF ou matrícula já existentes e veículos com placa repetida. Além disso, todos os dados obrigatórios deverão ser informados para que o cadastro seja concluído com sucesso.

 7.2 Etapa de Locação
Para realizar uma locação, o cliente deverá estar previamente cadastrado no sistema e o veículo escolhido deverá estar disponível para aluguel. Toda locação deverá estar associada a um funcionário responsável pelo atendimento e registro da operação. O sistema não permitirá locações com quantidade de dias igual ou inferior a zero, nem permitirá que um mesmo veículo participe de duas locações simultaneamente. Após a confirmação da locação, o veículo terá seu status alterado automaticamente para indisponível.

 7.3 Etapa de Cálculo da Locação
O valor total da locação será calculado com base no valor da diária do veículo multiplicado pela quantidade de dias contratada. Caso existam cobranças adicionais decorrentes de atraso na devolução ou danos ao veículo, esses valores serão acrescentados ao valor final da locação.

 7.4 Etapa de Devolução
Ao registrar a devolução do veículo, o sistema deverá atualizar automaticamente sua disponibilidade para que possa ser alugado novamente. Caso a devolução ocorra após a data prevista, será aplicada uma multa correspondente ao valor de uma diária adicional para cada dia de atraso. Se forem identificados danos no veículo durante a vistoria, o funcionário responsável poderá registrar cobranças adicionais referentes aos custos de reparo ou manutenção.

 7.5 Etapa de Controle Financeiro
Clientes que possuírem débitos pendentes, multas por atraso ou cobranças não quitadas não poderão realizar novas locações até que sua situação seja regularizada. Todas as cobranças realizadas deverão permanecer registradas para fins de consulta e controle financeiro da locadora.

 7.6 Etapa de Controle Operacional e Persistência
Veículos que estiverem em manutenção ou apresentarem problemas mecânicos não poderão ser disponibilizados para locação até que sua situação seja regularizada. Todas as informações cadastradas e alterações realizadas deverão ser armazenadas em arquivos para garantir a persistência dos dados entre as execuções do sistema. Além disso, os registros de clientes, funcionários, veículos e locações poderão ser consultados, atualizados e removidos por meio das operações de CRUD (Create, Read, Update e Delete), mantendo o histórico e a consistência das informações do sistema.
