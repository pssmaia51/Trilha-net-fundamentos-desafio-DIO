# 🅿️ Sistema de Estacionamento em C#

## 📌 Descrição
Este projeto é um sistema de gerenciamento de estacionamento desenvolvido em **C#** utilizando o .NET.  
O programa permite **adicionar**, **remover** e **listar veículos** estacionados, calculando o valor a ser pago com base no tempo de permanência.

O sistema é **interativo via console** e utiliza **POO (Programação Orientada a Objetos)** para organizar o código.

---

## 📂 Estrutura de Pastas
```
Instacionamento/
│
├── Models/
│   └── Estacionamento.cs      # Classe responsável pela lógica do sistema
│
├── Program.cs                 # Ponto de entrada do programa (menu interativo)
├── Instacionamento.sln        # Arquivo da solução .NET
└── DesafioDIOCShap.csproj     # Configuração do projeto
```

---

## 🛠️ Funcionalidades

- **Adicionar veículo**
  - Solicita ao usuário a placa do veículo e armazena na lista.
- **Remover veículo**
  - Solicita a placa e o tempo de permanência.
  - Calcula o valor a pagar:  
    ```
    valorTotal = precoInicial + (precoPorHora * horas)
    ```
- **Listar veículos**
  - Exibe todos os veículos estacionados.
  - Caso não haja veículos, mostra a mensagem:
    ```
    "Não há veículos estacionados."
    ```
- **Encerrar**
  - Finaliza o programa.

---

## 📜 Classe `Estacionamento`

### Atributos
- `decimal precoInicial` → Valor fixo cobrado ao estacionar.
- `decimal precoPorHora` → Valor por hora de permanência.
- `List<string> veiculos` → Lista com as placas dos veículos.

### Métodos
- `AdicionarVeiculo()` → Cadastra uma nova placa.
- `RemoverVeiculo()` → Remove a placa informada e calcula o valor devido.
- `ListarVeiculos()` → Mostra todos os veículos estacionados.

---

## 📋 Menu do Sistema

Ao iniciar o programa, o usuário informa:
- **Preço inicial**
- **Preço por hora**

Depois, é exibido um menu interativo:

```
=== Sistema de Estacionamento ===
1 - Cadastrar veículo
2 - Remover veículo
3 - Listar veículos
4 - Encerrar
Escolha uma opção:
```

---

## 🚀 Como Executar

1. **Clonar o repositório**
   ```powershell
   git clone <URL_DO_REPOSITORIO>
   cd Instacionamento
   ```

2. **Rodar o projeto**
   ```powershell
   dotnet run
   ```

---

## 💡 Conceitos Utilizados
- Programação Orientada a Objetos (POO)
- Listas (`List<string>`)
- Estrutura de repetição (`while`)
- Estrutura condicional (`if/else` e `switch`)
- Interação com o usuário via `Console.ReadLine` e `Console.WriteLine`

---

## 📷 Exemplo de Execução

```
Digite o preço inicial: 5
Digite o preço por hora: 2

=== Sistema de Estacionamento ===
1 - Cadastrar veículo
2 - Remover veículo
3 - Listar veículos
4 - Encerrar
Escolha uma opção: 1
Digite a placa do veículo para estacionar: ABC1234
Veículo adicionado com sucesso!

Pressione qualquer tecla para continuar...
```

---

## 🏷️ Licença
Este projeto é de uso livre para estudos e aperfeiçoamentos.
