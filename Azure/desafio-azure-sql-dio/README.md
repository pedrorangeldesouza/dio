Desafio DIO - Configurando uma Instância de Banco de Dados na Azure
📝 Descrição
Este projeto foi desenvolvido como parte do desafio da Digital Innovation One (DIO) sobre configuração de uma instância de Banco de Dados na Microsoft Azure.

O objetivo é praticar a criação e configuração de uma instância gerenciada de banco de dados SQL, documentando todas as etapas e aprendizados de forma clara e estruturada.

🚀 Tecnologias Utilizadas
Microsoft Azure
Azure SQL Database / SQL Managed Instance
GitHub
Markdown (para documentação)
🧩 Passo a Passo
1️⃣ Criação do Grupo de Recursos
Antes de iniciar, criamos um Grupo de Recursos chamado RG_BancoDados para organizar todos os recursos relacionados ao projeto.

2️⃣ Criando o Servidor de Banco de Dados SQL
No Portal Azure, clique em “Criar um recurso”
Selecione Banco de Dados > Banco de Dados SQL
Escolha a assinatura, grupo de recursos e defina:
Nome do banco de dados: db-lab
Servidor: criar novo (definir nome, usuário administrador e senha forte)
Tipo de computação: Basic ou Standard (conforme o plano gratuito ou necessidade)
Localização: Sul do Brasil
3️⃣ Configurações de Rede e Segurança
Na aba Rede, configure:

Método de Conectividade: Endpoint público
Regras de firewall: habilitar acesso apenas ao IP atual
Autenticação: SQL (usuário e senha definidos na criação)
💡 Dica: Evite permitir acesso a "Todos os IPs". Isso reduz o risco de exposição do banco.

4️⃣ Revisar e Criar
Revise todas as informações e clique em “Criar”.
O Azure provisionará automaticamente o banco de dados e o servidor.

5️⃣ Testando a Conexão
Após a criação:

Acesse o Azure SQL Database no portal.
Copie a string de conexão.
Teste a conexão usando ferramentas como:
Azure Data Studio
SQL Server Management Studio (SSMS)
Visual Studio Code com extensão SQL
💡 Aprendizados
Durante este desafio, aprendi a:

Criar e configurar uma instância de banco de dados SQL no Azure;
Entender as opções de rede, segurança e desempenho;
Configurar regras de firewall e boas práticas de acesso;
Testar conexões utilizando ferramentas externas;
Documentar processos técnicos de forma organizada no GitHub.
