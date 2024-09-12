<h1>Sistema de Processamento de Transações Financeiras</h1>

<p>
    Este projeto é um sistema simples de processamento de transações financeiras entre contas bancárias. Ele possui duas versões:
</p>

<ul>
    <li><strong>Versão com Múltiplos Arquivos</strong>: Cada classe e responsabilidade estão separadas em arquivos diferentes, seguindo as boas práticas de modularização.</li>
    <li><strong>Versão com um Único Arquivo</strong>: Todo o código centralizado em um único arquivo <code>.py</code>, o que pode facilitar a explicação em algumas situações.</li>
</ul>

<p>
    O sistema utiliza o <code>ThreadPoolExecutor</code> para processar múltiplas transações em paralelo, acelerando o processamento. Na versão com pandas, os resultados podem ser visualizados em um <strong>DataFrame</strong>.
</p>

<h2>Funcionalidades</h2>

<ul>
    <li><strong>Criação de Transações</strong>: O sistema cria transações entre contas de origem e destino, especificando o valor a ser transferido.</li>
    <li><strong>Execução de Transações</strong>: As transações são realizadas de forma paralela para otimizar o tempo de processamento.</li>
    <li><strong>Verificação de Saldos</strong>: O sistema garante que as transações sejam concluídas se houver saldo suficiente na conta de origem.</li>
    <li><strong>Atualização de Saldos</strong>: Após a execução das transações, os saldos das contas de origem e destino são atualizados.</li>
    <li><strong>Visualização dos Resultados (Versão com pandas)</strong>: Ao final da execução, os resultados podem ser exibidos em um <strong>DataFrame</strong>, que contém informações detalhadas de cada transação, como número da transação, conta de origem, conta de destino, valor, saldo e status da transação.</li>
</ul>

<h2>Estrutura do Código</h2>

<h3>Versão com Múltiplos Arquivos</h3>
<p>
    A versão modular segue boas práticas de separação de responsabilidades, onde cada parte do sistema tem seu próprio arquivo <code>.py</code>.
</p>
<ul>
    <li><code>models.py</code>: Define as classes de dados (<code>Transacao</code> e <code>ContaSaldo</code>).</li>
    <li><code>data_access.py</code>: Implementa o acesso aos saldos e a lógica de atualização das contas.</li>
    <li><code>transacoes.py</code>: Contém a <code>TransacaoFactory</code>, que cria transações.</li>
    <li><code>services.py</code>: Contém a lógica de negócios (<code>ExecutarTransacaoFinanceira</code>), que gerencia a execução e o processamento das transações.</li>
    <li><code>main.py</code>: Arquivo principal para a execução do sistema.</li>
</ul>

<h3>Versão com um Único Arquivo</h3>
<p>
    Para fins de simplificação e explicação centralizada, há também uma versão onde todo o código está centralizado em um único arquivo <code>.py</code>. Isso é útil quando você deseja visualizar ou compartilhar tudo em um único lugar sem a necessidade de lidar com vários arquivos.
</p>
