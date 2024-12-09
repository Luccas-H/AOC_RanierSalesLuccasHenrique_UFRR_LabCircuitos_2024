# Relatório Técnico de Circuitos Digitais

## Componente: Unidade Lógica e Aritmética (ULA)

---

### 1. Descrição do Componente

- **Descrição Geral:**  
  A Unidade Lógica e Aritmética (ULA) é um componente digital responsável por realizar operações lógicas e aritméticas em circuitos computacionais. Ela processa dois conjuntos de dados de entrada (A e B), seleciona a operação com base em um seletor (4 bits), e fornece um resultado na saída, além de sinais auxiliares, como *carryout*. Este relatório aborda as operações AND, OR, NOT, NOR, NAND, XOR, deslocamento de bits (SHIFT) e operações aritméticas (soma e subtração).

- **Pinos e Lógica do Componente:**  

  | Pino | Nome/Função           | Descrição                                                   |
  |------|-----------------------|-----------------------------------------------------------|
  | 1    | Entrada A             | Primeiro conjunto de dados (8 bits).                      |
  | 2    | Entrada B             | Segundo conjunto de dados (8 bits).                       |
  | 3    | Seletor    | Sinal de controle que seleciona a operação (4 bits).      |
  | 4    | Resultado             | Saída com o resultado da operação selecionada (8 bits).   |
  | 5    | Carry Out             | Indica *carry* em operações de soma/subtração.            |

- **Função Lógica:**  
  As operações realizadas são selecionadas com base no **código de controle (OpCode)**:

  | Código de Operação (4 bits) | Operação        | Descrição                                      |
  |-----------------------------|-----------------|------------------------------------------------|
  | 0000                        | AND             | Saída = A AND B                               |
  | 0001                        | OR              | Saída = A OR B                                |
  | 0010                        | NOT             | Saída = NOT A                                 |
  | 0011                        | NOT             | Saída = NOT B                                 |
  | 0100                        | NOR             | Saída = A NOR B                               |
  | 0101                        | NAND            | Saída = A NAND B                              |
  | 0110                        | XOR             | Saída = A XOR B                               |
  | 1000                        | SHIFT LEFT      | Saída = A deslocada 2 bits à esquerda         |
  | 1001                        | SHIFT LEFT      | Saída = B deslocada 2 bits à esquerda         |
  | 1010                        | SHIFT RIGHT     | Saída = A deslocada 2 bits à direita          |
  | 1011                        | SHIFT RIGHT     | Saída = B deslocada 2 bits à direita          |
  | 1100                        | Soma            | Saída = A + B                                 |
  | 1101                       | Subtração       | Saída = A - B                                 |

---

### 2. Esquema do Circuito

- **Captura de Tela do Circuito em Logisim:**  
  ![Esquema do Circuito](Imagens/ULA_cicuito_completo.png)  
  *Legenda:* Este esquema mostra a ULA implementada no Logisim com entradas (A e B), seletores de operação, e a saída.

- **Descrição do Esquema:**  
  O circuito foi montado no Logisim utilizando multiplexadores para selecionar a operação com base no código de controle. Os blocos individuais implementam operações específicas, como soma/subtração (usando somadores completos), e portas lógicas para AND, OR, NOR, etc. Os deslocadores de bits são implementados com registradores de deslocamento.

---

### 3. Testes Realizados

#### Configuração do Teste

- **Descrição do Teste:**  
  O objetivo dos testes foi validar cada operação da ULA, confirmando que as saídas correspondem aos resultados esperados para diferentes combinações de entradas e códigos de operação.

- **Entradas, Conexões e Saídas Esperadas:**  

  | Pino de Entrada | Sinal Aplicado        | Código de Operação | Pino de Saída | Resultado Esperado |
  |-----------------|-----------------------|--------------------|---------------|---------------------|
  | A = 00000101    | B = 00000100          | 0000 (AND)         | Saída         |            |
  | A = 00000101    | B = 00000100          | 0001 (OR)          | Saída         | 11101110           |
  | A = 00000101    | B = 00000100          | 0010 (NOT)         | Saída         | 00110011           |
  | A = 00000101    | B = 00000100          | 0100 (NOR)        | Saída         | 01110110           |
  | A = 00000101    | B = 00000100          | 0101 (NAND)        | Saída         | 01110110           |
  | A = 00000101    | B = 00000100          | 0110 (XOR)        | Saída         | 01110110           |
  | A = 00000101    | B = 00000100          | 1100 (Subtrator)        | Saída         | 01110110           |

#### Configuração do Logisim

- **Configurações Utilizadas:**  
  - Entradas A e B conectadas a *Switches*.  
  - Código de operação controlado por uma entrada de 4 bits.  
  - Saída conectada a *Probes* para visualização dos resultados.  

---

### 4. Resultados dos Testes

- **Resultados Obtidos no Logisim:**  

 | Pino de Entrada | Sinal Aplicado        | Código de Operação | Pino de Saída | Resultado Esperado |
  |-----------------|-----------------------|--------------------|---------------|---------------------|
  | A = 00000101    | B = 00000100          | 0000 (AND)         | Saída         |            |
  | A = 00000101    | B = 00000100          | 0001 (OR)          | Saída         | 11101110           |
  | A = 00000101    | B = 00000100          | 0010 (NOT)         | Saída         | 00110011           |
  | A = 00000101    | B = 00000100          | 0100 (NOR)        | Saída         | 01110110           |
  | A = 00000101    | B = 00000100          | 0101 (NAND)        | Saída         | 01110110           |
  | A = 00000101    | B = 00000100          | 0110 (XOR)        | Saída         | 01110110           |
  | A = 00000101    | B = 00000100          | 1100 (Subtrator)        | Saída         | 01110110           |

- **Captura de Tela dos Testes:**  
  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_and.jpg)  
  *Legenda:* Operação A AND B.
  
  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_or.jpg)  
  *Legenda:* Operação A OR B.

  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_not.jpg)  
  *Legenda:* Operação NOT A.

  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_nor.jpg)  
  *Legenda:* Operação A NOR B.

  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_nand.jpg)  
  *Legenda:* Operação A NAND B.

  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_xor.jpg)  
  *Legenda:* Operação NOT A XOR B.

  ![Resultados do Teste](Imagens/ULA-testes/ULA_teste_subtrator.jpg)  
  *Legenda:* Operação A - B.

- **Análise dos Resultados:**  
  Os resultados obtidos nos testes coincidiram com os valores esperados para todas as operações. Isso valida que a ULA foi implementada corretamente e opera conforme especificado.

---

*Relatório elaborado por:* *[Seu Nome/Equipe]*  
*Última atualização:* *[09/12/2024]*  
"""
