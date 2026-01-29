# Desafio DIO - Máquinas Virtuais na Azure

## 📝 Descrição
Este projeto foi desenvolvido como parte do desafio da Digital Innovation One (DIO) sobre criação e gerenciamento de máquinas virtuais no Microsoft Azure.

O objetivo é aplicar os conhecimentos adquiridos nas aulas, criar uma máquina virtual no Azure e documentar todo o processo de forma clara e organizada.

## 🚀 Tecnologias Utilizadas
- Microsoft Azure
- Portal Azure (interface gráfica)
- Windows Server 2019 (imagem da VM)
- GitHub (para documentação)
- Markdown (README.md)

---

## 🧩 Passo a Passo: Criando a VM

### 1️⃣ Criar Grupo de Recursos
Antes de criar a VM, é importante organizar todos os recursos. Criamos um **Grupo de Recursos** chamado `RG_Lab` (RG = Resource Group), que facilitará o gerenciamento e organização das máquinas e serviços.

---

### 2️⃣ Adicionar Máquina Virtual
- Selecione o grupo de recursos criado;
- Clique em **“+ Adicionar”**;
- Escolha **Computação > Máquina Virtual**.

---

### 3️⃣ Configurações Básicas da VM
Na aba **Básico**, configure:

- **Assinatura:** 
- **Grupo de Recursos:** RG_Lab  
- **Nome da Máquina Virtual:** SrvLab  
- **Região:** Sul do Brasil (ou conforme necessidade)  
- **Opções de Disponibilidade:** Nenhuma (pode configurar redundância se necessário)  
- **Sistema Operacional:** Windows Server 2019  
- **Instância Azure Spot:** Opcional  
- **Tamanho da Máquina:** B2ms (2 vCPUs, 8GB RAM)  
- **Nome de usuário e senha:** Administração padrão (senha forte)  
- **Portas de Entrada Pública:** Nenhuma, por segurança  
- **Licenciamento:** Habilitado caso possua licença

💡 Observação: a escolha da região influencia a latência. O tamanho da VM impacta custo e desempenho.

---

### 4️⃣ Configuração de Disco
Na aba **Discos**:

- **Tipo de Disco:** SSD Standard  
- **Criptografia:** Padrão do Azure  
- **Disco de dados:** Opcional  
- **Compatibilidade com Disco Ultra:** Apenas se necessário para alto desempenho  

💡 Dica: Discos SSD Premium têm melhor desempenho, mas maior custo. Escolha conforme uso da VM.

---

### 5️⃣ Configuração de Rede
Na aba **Rede**:

- **Rede Virtual e Sub-rede:** Criadas automaticamente pelo Azure (default)  
- **IP Público:** Default (ou configure conforme necessidade)  
- **Grupo de Segurança da Rede (NSG):** Default  
- **Portas de Entrada Públicas:** Nenhuma (por segurança)

💡 É possível customizar todas as configurações, mas para este laboratório mantivemos o padrão.

---

### 6️⃣ Gerenciamento da VM
Na aba **Gerenciamento**, você pode configurar:

- **Monitoramento:** habilitado com Storage Account gerenciada  
- **Diagnóstico do SO:** opcional para monitoramento de aplicativos  
- **Identidade gerenciada:** opcional, usada para autenticação em serviços Azure sem armazenar credenciais  
- **Desligamento automático:** configurado às 19h (Horário de Brasília)  
- **Backup:** configurado em Storage Account, com política de backup  

💡 Essas ações garantem segurança, controle e monitoramento da VM.

---

### 7️⃣ Marcas (Tags)
Na aba **Marcas**:

- **Nome:** Ambiente  
- **Valor:** SrvLab  

💡 Tags ajudam a organizar recursos e gerar relatórios de custo e uso.

---

### 8️⃣ Revisão e Criação
Na aba **Revisão**, confira todas as configurações. Caso tudo esteja correto, clique em **Criar**.  

Parabéns! Sua VM está pronta e funcional.

---

## 💡 Aprendizados
Durante este desafio, aprendi a:

- Criar e configurar uma máquina virtual no Azure de forma segura;  
- Entender as opções de discos, rede e gerenciamento;  
- Aplicar boas práticas de segurança, como não abrir portas públicas desnecessárias;  
- Habilitar monitoramento, diagnóstico e backup;  
- Documentar processos técnicos usando Markdown e GitHub.
