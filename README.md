<h1>Sistema de Processamento de Transações Financeiras</h1>
Este projeto é um sistema simples de processamento de transações financeiras entre contas bancárias. O sistema processa várias transações de forma simultânea, utilizando o ThreadPoolExecutor para acelerar o processamento.

Funcionalidades
Criação de Transações : O sistema cria transações entre contas de origem e destino, especificando o valor a ser transferido.
Execução de Transações : As transações são realizadas de forma paralela para otimizar o tempo de processamento.
Verificação de Saldos : O sistema garante que as transações sejam concluídas se houver saldo suficiente na conta de origem.
Atualização de Saldos : Após a execução das transações, os saldos das contas de origem e destino são atualizados.
Estrutura do Código
Transação : Representa uma transação financeira com conta de origem, conta de destino e valor.
ContaSaldo : Armazena o saldo de uma conta bancária.
AcessoDados : Simula o acesso e a atualização dos saldos das contas.
ExecutarTransacaoFinanceira : Gerencia a lógica de execução das transações, incluindo verificação de saldos e atualização de contas.
TransacaoFactory : Cria instâncias da classe Transacaode forma padronizada.
Como Executar
Certifique-se de que o Python esteja instalado em seu sistema.
Clone o repositório ou baixe o código.
