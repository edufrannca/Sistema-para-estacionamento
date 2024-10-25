# 🚗 Sistema de Gerenciamento de Estacionamento

Bem-vindo ao **Sistema de Gerenciamento de Estacionamento**! Este projeto em C# oferece uma solução simples e eficaz para o gerenciamento de veículos em um estacionamento, destacando-se pela sua lógica de validação robusta e interface amigável.

## ✨ Funcionalidades

### 1. **Cadastro de Veículo**
   - Permite a adição de veículos ao estacionamento.
   - **Validação de Placas**: O sistema aceita dois formatos de placas:
     - Padrão antigo: `ABC1D23`
     - Padrão Mercosul: `ABC1D23` e `ABC4D56`
   - Garante que placas duplicadas não sejam cadastradas.

### 2. **Remoção de Veículo**
   - Remove veículos do estacionamento.
   - **Cálculo de Preço**: O valor total é calculado com base em:
     - **Preço Inicial**: Valor fixo cobrado no início do estacionamento.
     - **Preço por Hora**: Taxa cobrada por cada hora adicional.
   - O sistema informa o usuário sobre o valor total a ser pago.

### 3. **Listagem de Veículos**
   - Exibe uma lista dos veículos atualmente estacionados.
   - Facilita a visualização do espaço ocupado no estacionamento.

## 🔍 Lógica Implementada

O sistema é estruturado com base em uma classe chamada `Estacionamento`, que encapsula as seguintes responsabilidades:

- **Propriedades**:
  - `precoInicial`: Define o custo inicial para estacionar.
  - `precoPorHora`: Define a taxa cobrada por cada hora adicional.
  - `veiculos`: Uma lista que armazena as placas dos veículos cadastrados.

- **Métodos**:
  - `AdicionarVeiculo()`: Recebe a placa do veículo, valida seu formato e a adiciona à lista, se não estiver duplicada.
  - `RemoverVeiculo()`: Permite a remoção de um veículo, solicita o número de horas que o veículo permaneceu e calcula o valor total a ser pago.
  - `ListarVeiculos()`: Exibe todas as placas dos veículos atualmente estacionados.

## 🚀 Como Executar o Projeto

### Pré-requisitos
- .NET SDK instalado na sua máquina.

### Passos para Execução
1. **Clone o Repositório**:
   ```bash
   git clone https://github.com/edufrannca/Sistema-para-estacionamento.git
   cd Sistema-para-estacionamento
   ```

2. **Compile e Execute o Programa**:
   ```bash
   dotnet build
   dotnet run
   ```

3. **Interaja com o Sistema**:
   - Siga as instruções apresentadas no menu interativo.

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para:
- Criar uma **Issue** para reportar bugs ou sugerir melhorias.
- Fazer um **Pull Request** com suas melhorias.

## 📄 Licença

Este projeto está licenciado sob a [MIT License](LICENSE).

## 📬 Contato

Para mais informações ou perguntas, entre em contato:
- **E-mail**: luizeduardodefranca@gmail.com

---

Agradeço pela sua atenção e espero que este projeto desperte seu interesse!
