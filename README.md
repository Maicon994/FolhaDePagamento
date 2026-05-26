# Folha de Pagamento System

Aplicativo mobile desenvolvido em Java no Android Studio com o objetivo de calcular a folha de pagamento de um funcionário, realizando automaticamente os descontos de INSS e IR, além do cálculo do salário-família e salário líquido.

---

## Objetivo da Aplicação

O sistema foi desenvolvido para automatizar o cálculo do salário líquido de um funcionário a partir das seguintes informações:

* Nome do funcionário
* Salário bruto
* Sexo
* Número de filhos

A aplicação realiza todos os cálculos exigidos pela atividade e apresenta os resultados formatados na tela.

---

# Funcionalidades

## Entrada de Dados

O aplicativo permite informar:

* Nome do funcionário
* Salário bruto
* Sexo (Masculino ou Feminino)
* Quantidade de filhos

---

# Cálculos Realizados

## Desconto do INSS

O cálculo do INSS é realizado conforme a faixa salarial:

| Faixa Salarial              | Desconto |
| --------------------------- | -------- |
| Até R$ 1.212,00             | 7,5%     |
| R$ 1.212,01 até R$ 2.427,35 | 9%       |
| R$ 2.427,36 até R$ 3.641,03 | 12%      |
| R$ 3.641,04 até R$ 7.087,22 | 14%      |

---

## Desconto do IR

O cálculo do Imposto de Renda segue as regras:

| Faixa Salarial              | Desconto |
| --------------------------- | -------- |
| Até R$ 1.903,98             | Isento   |
| R$ 1.903,99 até R$ 2.826,65 | 7,5%     |
| R$ 2.826,66 até R$ 3.751,05 | 15%      |
| R$ 3.751,06 até R$ 4.664,68 | 22,5%    |

---

## Salário Família

Funcionários com salário bruto de até R$ 1.212,00 recebem:

* R$ 56,47 por filho

---

# Fórmula Utilizada

O salário líquido é calculado da seguinte forma:

```text
Salário Líquido =
Salário Bruto − (INSS + IR) + Salário Família
```

---

# Tecnologias Utilizadas

* Java
* Android Studio
* ConstraintLayout
* XML
* RadioButton
* EditText
* TextView
* Button
* Toast
* Try/Catch

---

# Tratamento de Dados

A aplicação possui:

* Validação de campos vazios
* Verificação de valores negativos
* Tratamento de exceções utilizando Try/Catch
* Mensagens de erro para entradas inválidas

---

# Interface

A interface foi desenvolvida com foco em:

* Facilidade de uso
* Organização visual
* Responsividade
* Boa experiência do usuário

Foram utilizadas cores e componentes visuais para melhorar a usabilidade do sistema.

---

# Resultado Exibido

Após o cálculo, o sistema apresenta:

* Nome do funcionário com tratamento “Sr.” ou “Sra.”
* Valor do desconto do INSS
* Valor do desconto do IR
* Valor do salário-família
* Valor do salário líquido

---

# Exemplo de Funcionamento

```text
Funcionário: Sra. Maria
Salário Bruto: R$ 2000,00

INSS: R$ 180,00
IR: R$ 150,00
Salário Família: R$ 0,00

Salário Líquido: R$ 1670,00
```

---

# Conclusão

O aplicativo atende todos os requisitos propostos na atividade, realizando corretamente os cálculos da folha de pagamento e apresentando os resultados de forma clara e organizada ao usuário.

---

## Autor
Maicon Ferreira Machado
