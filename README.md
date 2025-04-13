

# 💻 Sistema Bancário em Python - V2

Este projeto simula um sistema bancário simples com funcionalidades como depósito, saque, extrato, criação de usuários e contas bancárias.

---

## 📋 Funcionalidades

### `menu()`
Exibe o menu de opções para o usuário e retorna a escolha feita.

---

### `depositar(saldo, valor, extrato, /)`
- Realiza o depósito se o valor for positivo.
- Atualiza o saldo e registra a operação no extrato.

---

### `sacar(*, saldo, valor, extrato, limite, numero_saques, limite_saques)`
- Permite saques com as seguintes validações:
  - Se o valor é maior que o saldo.
  - Se o valor excede o limite por saque.
  - Se o número máximo de saques foi atingido.
- Atualiza saldo, extrato e contador de saques.

---

### `exibir_extrato(saldo, /, *, extrato)`
- Mostra todas as movimentações registradas no extrato.
- Exibe o saldo atual.

---

### `criar_usuario(usuarios)`
- Cria um novo usuário mediante CPF não cadastrado.
- Coleta nome completo, data de nascimento e endereço.

---

### `filtrar_usuario(cpf, usuarios)`
- Busca um usuário com base no CPF.
- Retorna o primeiro usuário encontrado ou `None`.

---

### `criar_conta(agencia, numero_conta, usuarios)`
- Cria uma conta para um usuário já existente.
- Associa a conta ao CPF informado.

---

### `listar_contas(contas)`
- Lista todas as contas existentes no sistema com:
  - Agência
  - Número da conta
  - Nome do titular

---

### `main()`
- Função principal que mantém o programa em execução.
- Controla o fluxo do menu e chama as funções conforme a opção selecionada.
- Define constantes e armazena os dados temporários como usuários, contas e extrato.

---

## 🏁 Execução
O programa começa pela função `main()` e segue em loop até que o usuário escolha sair `[q]`.

