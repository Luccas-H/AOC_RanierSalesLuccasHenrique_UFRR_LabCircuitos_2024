# Laboratório de Circuitos Digitais - AOC

Este repositório contém os projetos desenvolvidos para a disciplina de **Arquitetura e Organização de Computadores (AOC)** na **Universidade Federal de Roraima (UFRR)**. Os trabalhos consistem em implementações práticas de circuitos digitais utilizando o simulador **Logisim**, incluindo banco de registradores, multiplexadores, máquinas de estados e outros componentes fundamentais para sistemas digitais.

---

## Estrutura do Repositório

O repositório está organizado por tópicos abordados ao longo da disciplina, com cada diretório contendo os circuitos implementados e relatórios detalhados:

### Diretórios Principais

- **[1 - FlipFlopD e JK](https://github.com/RanierSales/AOC_RanierSalesLuccasHenrique_UFRR_LabCircuitos_2024/tree/main/Flip-Flop%20D_JK)**  
  Implementação de multiplexadores 2x1, 4x1, 8x1 e 16x1.  
  - [Relatório FlipFlop D e JK](https://github.com/RanierSales/AOC_RanierSalesLuccasHenrique_UFRR_LabCircuitos_2024/blob/main/Flip-Flop%20D_JK/Relatorio.md)
  - [Circuito FlipFlop D e JK](https://github.com/RanierSales/AOC_RanierSalesLuccasHenrique_UFRR_LabCircuitos_2024/blob/main/Flip-Flop%20D_JK/FLIPFLOP.circ)

- **[2 -Multiplexadores de 4 entradas](./Multiplexador)**  
  Implementação de multiplexadores 2x1, 4x1, 8x1 e 16x1.  
  - [Relatório Multiplexadores](./Multiplexador/Relatorio.md)
  - [Circuito Multiplexadores](./Multiplexador/Multiplexador.circ)

- **[3 - Porta Lógica XOR](./Porta_XOR)**  
  Implementação da porta lógica XOR utilizando apenas de portas AND, OR e NOT. 
  - [Relatório Porta XOR](./Porta_XOR/Relatorio.md)
  - [Circuito de XOR](./Porta_XOR/XOR.circ)
 
- **[4 - Somador 8bits com 4](./Somador_8bits_4)**  
  Implementação do somador de 8 bits com o binpário 00000100(decimal 4).
  - [Relatório Somador8bits com 4](./Somador_8bits_4/Relatorio.md)
  - [Circuito Somador](./Somador_8bits_4/Somador8bitsCom4.circ)
    
- **[5 - Memória ROM](./Memoria_ROM)**  
  Implementação do circuito de simulação de uma memória ROM de 8 bits e sua tabela de endereços. 
  - [Relatório Memória ROM](./Memoria_ROM/Relatorio.md)
  - [Circuito Memória ROM](./Memoria_ROM/MemoriaROM.circ)
 
- **[6 - Memória RAM](./Memoria_RAM)**  
  Implementação do circuito de simulação de uma memória RAM de 8 bits utilizando registradores de  8 bits e multiplexador 8x1 de 8 bits.
  - [Relatório Memória RAM](./Memoria_RAM/Relatorio.md)
  - [Circuito Memória RAM](./Memoria_RAM/MemoriaRAM.circ)
    
- **[7 - Banco de Registradores](./BancoDeRegistradores)**  
  Implementação de um banco de registradores completo utilizando multiplexadores e registradores de 8 bits.  
  - [Relatório Banco de Registradores](./BancoDeRegistradores/Relatorio.md)
  - [Circuito Banco de Registradores](./BancoDeRegistradores/BancoDeRegistradores.circ)

- **[8 - Somador de 8bits](./Somador_8bits)**  
  Implementação do somador de dois numeros de 8 bits. 
  - [Relatório Somador de 8bits](./Somador_8bits/Relatorio.md)
  - [Circuito Somador de 8bits](./Somador_8bits/Somador8Bits.circ)
  
- **[9 - Detector da sequência 101](./Detector_101)**  
  Implementação de um circuito que detecta a sequência binária "101" em uma entrada de 8 bits. 
  - [Relatório Detector de sequência](./Detector_101/Relatorio.md)
  - [Circuito Detector de sequência](./Detector_101/Detector_101.circ)
  
- **[10 - ULA 8 Bits](./ULA_8bits)**  
  Unidade Lógica e Aritmética (ULA) capaz de realizar operações básicas de soma, subtração, e lógica.  
  - [Relatório ULA 8 Bits](./ULA_8bits/Relatorio.md)
  - [Circuito ULA 8 Bits](./ULA_8bits/ULA.circ)
  
- **[11 - Extensor de sinal](./Extensor_4bits_8bits)**  
  Circuito que possibilita a extensão de um entrada de 4 bits para uma saída de 8 bits sem perder o valor da entrada. 
  - [Relatório Extensor de sinal](./Extensor_4bits_8bits/Relatorio.md)
  - [Circuito Extensor de sinal](./Extensor_4bits_8bits/Extensor4bits_8bits.circ)
- **[12 - Máquinas de Estados](./MaquinaDeEstados)**  
  Projetos de máquinas de estados finitos (FSMs) com diferentes aplicações, incluindo LEDs indicadores e controle de direção.  
  - [Relatório Máquina de Estados](./MaquinaDeEstados/Relatorio.md)
  - [Circuito Máquina de Estados](./MaquinaDeEstados/MaquinaDeEstados.circ)

- **[13 - Contador Síncrono](./Contador_Sincrono)**  
  Implementação de um cirucito simulado de um contador síncrono utilizando flipflops e portas lógicas. 
  - [Relatório do contador síncrono](./Contador_Sincrono/Relatorio.md)
  - [Circuito do contador síncrono](./Contador_Sincrono/ContadorSincrono.circ)
 
- **[14 - Detector de paridade ímpar](./Detector_paridade_Impar)**  
  Projeto simulado que detecta a paridade ímpar de 1s em uma sequência de 4 bits como entrada. 
  - [Relatório Detector de paridade ímpar](./Detector_paridade_Impar/Relatorio.md)
  - [Cicrcuito Detector de paridade ímpar](./Detector_paridade_Impar/DetectorImparDe1s.circ)
 
- **[15 - Otimização com Karnaugh](./Otimizacao_Karnaugh)**  
  Demonstração simulada de cirucito que foi otimizado utilizando mapa de Karnaugh. 
  - [Relatório Otimização com Karnaugh](./Otimizacao_Karnaugh/Relatorio.md)
  - [Circuito Otimização com Karnaugh](./Otimizacao_Karnaugh/OtimizacaoDeKarnaugh.circ)
 
- **[16 - Decodificador de 7 segmentos](./Decodificador_7Segmentos)**  
  Implementação de circuito cuja função é transformar um entrada de 4 bits em uma saída no display de 7 segmentos de forma hexadecimal. 
  - [Relatório Decodificador de 7 segmentos](./Decodificador_7Segmentos/Relatorio.md)
  - [Circuito Decodificador de 7 segmentos](./Decodificador_7Segmentos/Decodificador7Segmentos.circ)

- **[17 - Detector de Numero Primo de 4 bits](./Detector_Numero_Primo)**  
  Projeto simulado que identifica se o número de até 4 bits é um número primo ou não.  
  - [Relatório Detector numero primo](./Detector_Numero_Primo/Relatorio.md)
  - [Circuito Detector numero primo](./Detector_Numero_Primo/IdentificadorDePrimo.circ)
---

## Objetivo

O objetivo deste repositório é documentar e centralizar os projetos desenvolvidos ao longo da disciplina, fornecendo uma base de estudos para futuros alunos e interessados em circuitos digitais. Cada diretório contém os arquivos do circuito no Logisim, capturas de tela do funcionamento e relatórios técnicos detalhados.

---

## Tecnologias Utilizadas

- **Logisim:** Simulador de circuitos digitais.
- **Markdown:** Para documentação e relatórios.
- **GitHub:** Para versionamento e compartilhamento de arquivos.

---

## Como Navegar

1. Clique no nome do diretório para acessar os arquivos correspondentes.
2. Dentro de cada diretório, consulte o arquivo `Relatorio.md` para obter informações detalhadas sobre os circuitos e testes realizados.

---

## Links Úteis

- [Documentação do Logisim](http://www.cburch.com/logisim/).

---

## Contribuidores

- **Ranier Sales**  
- **Luccas Henrique**

---

**UFRR - Universidade Federal de Roraima**  
**Curso de Engenharia de Computação**
