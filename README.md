# NumBase Converter C

![Language](https://img.shields.io/badge/language-C-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green)
![Contributions](https://img.shields.io/badge/contributions-welcome-brightgreen)

## 📌 Sobre o Projeto

**NumBase Converter C** é uma calculadora profissional de conversão de bases numéricas, desenvolvida em C, capaz de converter números entre diferentes sistemas de numeração, como **binário, octal, decimal e hexadecimal**. Projetado para precisão e desempenho, o projeto utiliza estruturas de dados eficientes e boas práticas de programação para lidar com conversões de forma rápida e confiável.

## ✨ Funcionalidades

✅ Conversão entre bases **binária (2), octal (8), decimal (10) e hexadecimal (16)**  
✅ Suporte para **grandes números** sem perda de precisão  
✅ Interface **interativa** baseada em terminal (CLI)  
✅ Implementação eficiente usando **pilhas e algoritmos otimizados**  
✅ Código modular e bem documentado para **facilidade de manutenção**  
✅ Testes unitários para garantir **confiabilidade**  

## 📁 Estrutura do Projeto

base-converter/
├── README.md              # General project documentation
├── LICENSE                # License file
├── Makefile               # Build file (or CMakeLists.txt if using CMake)
├── docs/                  # Detailed system documentation
│   ├── architecture.md    # Architecture overview and design decisions
│   ├── design.md          # Specification of modules and data flow
│   └── requirements.md    # Functional and non-functional requirements
├── src/                   # Main source code
│   ├── main.c             # Application entry point
│   ├── conversion/        # Module responsible for number base conversions
│   │   ├── conversion.c
│   │   └── conversion.h
│   ├── io/                # Input/output module and user interface
│   │   ├── io.c
│   │   └── io.h
│   └── utils/             # Utility functions like stack and array handling
│       ├── utils.c
│       └── utils.h
├── tests/                 # Unit and integration tests
│   ├── test_conversion.c
│   ├── test_io.c
│   └── test_utils.c
└── examples/              # Usage examples or test data
    └── usage_example.txt

## 🚀 Como Instalar e Compilar

### 🔧 Pré-requisitos

- **Compilador C** (GCC, Clang ou equivalente)
- **Make** (se for usar o Makefile)

### 🛠️ Compilação

```
git clone https://github.com/seu-usuario/numbase-converter-C.git
cd numbase-converter-C
make
```

Ou, manualmente:

```
gcc -o converter src/main.c src/conversion/conversion.c src/io/io.c src/utils/utils.c
```

## 📌 Como Usar
Após a compilação, execute o programa:

```
./converter
```

# Exemplo de uso:

```
Digite o número: 1011
Digite a base de entrada (2, 8, 10, 16): 2
Digite a base de saída (2, 8, 10, 16): 10

Resultado: 11
```

# 🧪 Como Executar os Testes
Para executar os testes unitários, use:

```
make test
```

Ou, manualmente:

```
gcc -o test_conversion tests/test_conversion.c src/conversion/conversion.c src/utils/utils.c
./test_conversion
```