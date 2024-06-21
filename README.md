# DIO_Desafio_Projeto_Paradigma_Orientado_a_Aspectos
Desafio DIO - C/C++ Paradigma de Programação Orientado à Aspectos

Projeto: Sistema Bancário com Verificação de Saldo usando Programação Orientada a Aspectos
Objetivo
Desenvolver um sistema bancário onde os saques em diferentes contas (corrente, salário, poupança, investimento) são acompanhados de uma verificação de saldo usando programação orientada a aspectos (AOP). A verificação de saldo e geração de log de erro serão implementadas usando AspectJ, enquanto as funcionalidades principais das contas serão implementadas usando programação orientada a objetos (OO) em Java.

Explicação
Classes de Conta: As classes Conta, ContaCorrente, ContaPoupanca e ContaInvestimento representam diferentes tipos de contas bancárias. Cada classe tem um método calculaValorTarifaManutencao que retorna a tarifa específica da conta.

Aspecto de Verificação de Saldo: O aspecto SaldoAspect usa pointcuts para interceptar chamadas ao método sacar em qualquer instância de Conta. Antes de realizar o saque, ele verifica se o saldo é suficiente. Se não for, lança uma exceção e gera uma mensagem de log.

Classe Principal: A classe Main cria instâncias de diferentes tipos de contas e realiza operações de saque e depósito, demonstrando a funcionalidade do aspecto de verificação de saldo.

Conclusão
Esta implementação demonstra como o paradigma de programação orientada a aspectos pode ser usado para separar a lógica transversal de verificação de saldo da lógica principal de negócios das contas bancárias. AspectJ facilita a inserção de comportamento adicional (como logs e validações) de forma modular e não invasiva.
