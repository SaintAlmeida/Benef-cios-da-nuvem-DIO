# Beneficios-da-nuvem-DIO


Criar uma máquina virtual (VM) no Microsoft Azure é um processo direto que pode ser realizado pelo portal web. Primeiramente, acesse o Portal do Azure com suas credenciais. No painel de navegação, digite "Máquinas virtuais" na barra de pesquisa e selecione a opção correspondente. Na página de Máquinas Virtuais, clique em "Criar" e escolha "Máquina virtual do Azure". Você será direcionado para a página de criação, onde deverá fornecer detalhes como o nome da VM, região, imagem do sistema operacional (por exemplo, Windows Server 2022 Datacenter) e tamanho da máquina. Em seguida, configure a conta de administrador, definindo um nome de usuário e uma senha segura. Na seção de regras de porta de entrada, selecione as portas que deseja permitir, como RDP (3389) para acesso remoto e HTTP (80) para tráfego web. Após preencher todas as informações necessárias, clique em "Examinar + criar" para revisar as configurações. Se tudo estiver correto, clique em "Criar" para iniciar a implantação da VM. O Azure começará a provisionar os recursos e, em alguns minutos, sua máquina virtual estará pronta para uso. Para acessar a VM, vá até a página de visão geral da máquina virtual e clique em "Conectar" > "RDP". Baixe o arquivo RDP fornecido, abra-o e insira as credenciais de administrador definidas anteriormente. Uma vez conectado, você terá acesso total à sua nova máquina virtual no Azure. Lembre-se de monitorar e gerenciar sua VM conforme necessário, utilizando as ferramentas e recursos disponíveis no portal. Esse processo permite que você aproveite a flexibilidade e escalabilidade da computação em nuvem oferecida pelo Azure.​

# Etapas para Criar uma Máquina Virtual no Azure
# Acessar o Portal do Azure
Navegue até o Portal do Azure e faça login com suas credenciais.

# Iniciar a Criação da Máquina Virtual
No painel de navegação, digite "Máquinas virtuais" na barra de pesquisa e selecione a opção correspondente. Na página de Máquinas Virtuais, clique em "Criar" e escolha "Máquina virtual do Azure".

# Configurar Detalhes da Instância
Na aba "Básico", forneça informações como:

Nome da máquina virtual (por exemplo, myVM)

Região (por exemplo, "Brasil Sul")

Imagem do sistema operacional (por exemplo, "Windows Server 2022 Datacenter")

# Tamanho da VM (escolha conforme a necessidade de recursos)​

# Definir Conta de Administrador
Configure as credenciais de administrador:

# Nome de usuário (por exemplo, azureuser)

Senha segura com pelo menos 12 caracteres, incluindo letras maiúsculas, minúsculas, números e símbolos​

# Configurar Regras de Porta de Entrada
Na seção de regras de porta de entrada, selecione as portas que deseja permitir, como:

RDP (3389) para acesso remoto

HTTP (80) para tráfego web​

# Revisar e Criar a Máquina Virtual
Após preencher todas as informações necessárias, clique em "Examinar + criar" para revisar as configurações. Se tudo estiver correto, clique em "Criar" para iniciar a implantação da VM.

# Acompanhar o Processo de Implantação
O Azure começará a provisionar os recursos. Você pode acompanhar o progresso na seção de notificações. Em alguns minutos, sua máquina virtual estará pronta para uso.

Acessar a Máquina Virtual
Para acessar a VM:

Vá até a página de visão geral da máquina virtual.

Clique em "Conectar" > "RDP".

Baixe o arquivo RDP fornecido.

Abra o arquivo e insira as credenciais de administrador definidas anteriormente.​

# Instalar o Servidor Web (Opcional)
Para ver sua VM em ação, você pode instalar o servidor web IIS:

Abra o PowerShell na VM.

Execute o comando:

Install-WindowsFeature -name Web-Server -IncludeManagementTools
Verificar a Página de Boas-Vindas do IIS
Após a instalação, abra um navegador e digite o endereço IP público da VM. Você deverá ver a página padrão de boas-vindas do IIS.

# Configurar o Desligamento Automático (Opcional)
Para economizar custos, você pode configurar o desligamento automático da VM:

Na seção "Operações" da VM, selecione "Desligamento automático".

Ative a opção e defina o horário desejado para o desligamento.

Clique em "Salvar" para aplicar as configurações.

# Excluir Recursos Quando Não Necessários
Quando não precisar mais da VM, é recomendável excluir os recursos para evitar cobranças:

Na página de visão geral da VM, clique no link do grupo de recursos.

Na página do grupo de recursos, clique em "Excluir grupo de recursos".

Digite o nome do grupo de recursos para confirmar e clique em "Excluir"
