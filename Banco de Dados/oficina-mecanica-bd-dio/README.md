🧰 Oficina Mecânica - Banco de Dados


Este projeto foi desenvolvido como parte de um desafio de modelagem de banco de dados, com o objetivo de criar um esquema lógico para um sistema de controle e gerenciamento de ordens de serviço em uma oficina mecânica.

🎯 Objetivo


O sistema permite registrar e gerenciar:

Clientes e seus veículos
Equipes e mecânicos responsáveis pelos serviços
Ordens de serviço (OS) com datas, status e valores
Serviços executados e peças utilizadas
🧩 Entidades Principais


Cliente
Veiculo
OrdemServico
Equipe
Mecanico
Servico
Peca
🔗 Relacionamentos


O modelo inclui dois relacionamentos N:N representados por tabelas associativas:

Servico_OrdemServico → liga serviços às ordens de serviço
Peca_OrdemServico → liga peças às ordens de serviço
Essas tabelas também armazenam quantidades e subtotais, contribuindo para o valor total da OS.

🛠️ Ferramentas Utilizadas


MySQL Workbench (modelagem lógica)
MySQL (para possível implementação futura)
📚 Contexto do Desafio


Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica.
Clientes levam veículos à oficina para conserto ou revisão.
Cada veículo é designado a uma equipe de mecânicos, que identifica os serviços a executar e registra uma OS com data de entrega.
O valor final é calculado com base na tabela de mão de obra e nas peças utilizadas.
🧠 Aprendizados


Identificação de entidades e relacionamentos
Modelagem de relacionamentos N:N
Aplicação de normalização
Transformação de esquema conceitual em lógico
💼 Autor


Pedro Rangel

Estudante de Análise de Dados | Foco em SQL, Power BI e Modelagem de Dados
