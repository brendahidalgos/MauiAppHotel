# 🏨 Calculadora de Diária de Hotel (Cálculo Avançado)

## 📝 Descrição

Este projeto é uma aplicação de exercício desenvolvida em **.NET MAUI** focada em simular uma lógica mais complexa de precificação de hospedagens.

O aplicativo realiza o cálculo do custo total da diária de hotel, considerando: o **tipo de suíte**, valores diferenciais para **adultos e crianças** e a **duração da estadia** calculada a partir das datas explícitas de check-in e check-out.

---

## ✨ Requisitos Técnicos e Funcionalidades

O desenvolvimento desta aplicação aborda os seguintes conceitos e requisitos de lógica em .NET MAUI:

### 1. Gestão e Validação de Datas
* **Datas de Estadia**: Utilização dos campos **Data de Entrada (Check-in)** e **Data de Saída (Check-out)** em vez de apenas o número de noites.
* **Validação de Calendário**: Implementação de lógica para garantir que a **Data de Saída seja sempre posterior** à Data de Entrada, emitindo alertas de erro caso contrário.
* **Cálculo de Duração**: O número de noites da hospedagem é calculado automaticamente com base na diferença entre as datas de Check-in e Check-out, utilizando as classes `DateTime` e `TimeSpan`.

### 2. Modelagem e Lógica de Negócio
* **Modelagem de Dados**: A classe `Hospedagem` (ou similar) inclui propriedades para `TipoSuite`, `DataEntrada`, `DataSaida` e os perfis de hóspedes.
* **BindingContext**: Uso do padrão MVVM para associar os campos da interface à *Model* de dados.
* **Lógica de Precificação**: Lógica na *Model* que aplica regras de custo diferenciado por perfil de hóspede (ex: crianças com 50% de desconto) e multiplica pelo número de noites calculado.

## ⚙️ Dados Solicitados no Cadastro

A interface de Cadastro solicita os seguintes dados para o cálculo:

* **Tipo de Suíte/Quarto** (Ex: Standard, Luxo)
* **Diária Base** (Valor monetário inicial)
* **Data de Entrada** (Check-in)
* **Data de Saída** (Check-out)
* **Número de Adultos**
* **Número de Crianças**

## 🚀 Como Executar o Projeto

Para testar o simulador de cálculo de diárias, siga as instruções de configuração:

### Pré-requisitos

* **Visual Studio 2022** (com a carga de trabalho de **.NET MAUI** instalada).
* **.NET 8**: Versão da *framework* utilizada no projeto.

### Instalação e Execução

1.  **Clone o Repositório:**
    ```bash
    git clone [https://github.com/brendahidalgos/NomeDoRepositorioHotel.git](https://github.com/brendahidalgos/NomeDoRepositorioHotel.git)
    ```
2.  **Abra no Visual Studio:**
    * Abra o arquivo de solução (`.sln`) no Visual Studio.
3.  **Execute o Aplicativo:**
    * Selecione o destino de sua preferência (Android Emulator, Windows Machine, etc.).
    * Pressione **F5** (Executar) para compilar e implantar o aplicativo.

---
## 👩‍💻 Desenvolvido em

* **Curso Técnico em Desenvolvimento de Sistemas**

## 📧 Contato

Se tiver alguma dúvida ou sugestão, pode me chamar!

* **GitHub**: [@brendahidalgos](https://github.com/brendahidalgos)

## ✍️ Autor

* **@brendahidalgos** - Aluna do curso de Análise e Desenvolvimento de Sistemas.
