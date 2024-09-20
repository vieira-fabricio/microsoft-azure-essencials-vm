# Resumo do Lab - Criando Máquinas Virtuais na Azure
#### Neste lab, exploramos o processo de criação e configuração de Máquinas Virtuais (VMs) no Microsoft Azure. O objetivo deste desafio é consolidar o 
conhecimento adquirido na prática de criar e gerenciar VMs, um dos principais serviços de computação na nuvem oferecidos pelo Azure.

### O que é uma Máquina Virtual?

Uma **Máquina Virtual (VM)** é uma representação virtual de um computador físico. Ela opera como se fosse um servidor independente, com sistema operacional, capacidade de processamento, memória, armazenamento e conectividade de rede. No Microsoft Azure, as VMs são usadas para executar cargas de trabalho variadas, como hospedagem de sites, aplicativos, bancos de dados ou ambientes de desenvolvimento. 

Ao usar uma VM no Azure, você pode escalar os recursos de computação conforme a demanda, além de controlar o sistema operacional e as aplicações que serão instaladas, como se fosse um servidor físico tradicional, mas com os benefícios da nuvem, como flexibilidade e pagamento conforme o uso.

---

### Passo a Passo para Criar uma Máquina Virtual no Azure

#### 1. **Acessar o Portal do Azure**
   - Vá até o site do [Portal do Azure](https://portal.azure.com/).
   - Faça login com suas credenciais de administrador ou conta Microsoft.

#### 2. **Abrir o Serviço de Criação de Máquina Virtual**
   - No painel de navegação à esquerda, clique em **Máquinas Virtuais** ou pesquise por "Máquina Virtual" na barra de pesquisa do topo.
   - Clique no botão **Criar** e selecione **Máquina Virtual**.

#### 3. **Configurar os Detalhes Básicos**
   - **Assinatura**: Escolha a assinatura do Azure que será utilizada.
   - **Grupo de Recursos**: Selecione um grupo de recursos existente ou crie um novo. O grupo de recursos organiza os recursos relacionados.
   - **Nome da Máquina Virtual**: Defina um nome para sua VM.
   - **Região**: Escolha a região do data center onde a VM será hospedada (ex: Leste dos EUA, Brasil Sul).
   - **Imagem**: Selecione o sistema operacional da VM (ex: Windows Server, Ubuntu, Red Hat).
   - **Tamanho**: Escolha o tamanho da VM (quantidade de CPU, memória), dependendo das necessidades de desempenho.

#### 4. **Configurar a Autenticação**
   - Escolha o método de autenticação:
     - **Chave SSH** (para Linux) ou **Usuário e Senha** (para Windows e Linux).
   - Defina as credenciais (nome de usuário e senha ou carregue uma chave pública SSH).

#### 5. **Configurar Disco e Armazenamento**
   - **Tipo de Disco OS**: Selecione o tipo de disco para o sistema operacional (SSD premium, SSD padrão, HDD padrão).
   - Configure discos adicionais, se necessário, para armazenamento de dados.

#### 6. **Configurar as Opções de Rede**
   - **Rede Virtual (VNet)**: Escolha uma rede virtual existente ou crie uma nova para a VM.
   - **Sub-rede**: Selecione a sub-rede onde a VM será conectada.
   - **IP Público**: Configure um endereço IP público se for necessário acessar a VM pela internet.
   - **Grupo de Segurança de Rede (NSG)**: Defina as regras de firewall para controlar o tráfego de entrada e saída.

#### 7. **Configurações de Gerenciamento**
   - Habilite o **Monitoramento** e outros recursos como backups automáticos, se necessário.
   - Escolha se deseja usar **Atualizações Automáticas** e **Backup**.

#### 8. **Revisar e Criar**
   - Clique em **Revisar e Criar**. O Azure fará uma validação das configurações.
   - Se tudo estiver correto, clique em **Criar**.

#### 9. **Aguarde a Implementação**
   - O processo de criação da máquina virtual será iniciado e pode levar alguns minutos.
   - Ao finalizar, você verá a VM criada no painel de **Máquinas Virtuais**.

#### 10. **Conectar à Máquina Virtual**
   - Após a implantação, selecione a máquina virtual criada.
   - Use o botão **Conectar** e escolha o método de conexão:
     - Para **Windows**, utilize **RDP**.
     - Para **Linux**, use o **SSH** com a chave configurada.

---

#### Conclusão
Durante este lab, aprendemos a criar e configurar máquinas virtuais no Microsoft Azure, o que inclui a escolha de uma imagem de sistema operacional, 
configuração de rede e gerenciamento de recursos. As VMs são essenciais para hospedar aplicativos e serviços, e o Azure oferece uma plataforma robusta 
para gerenciá-las de maneira eficiente.
