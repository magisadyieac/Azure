## Passo a Passo da Criação Que Fiz Para Testar

### 1. Acesso ao Portal Azure
- Acesse o portal: [https://portal.azure.com](https://portal.azure.com)
- Faça login com uma conta Microsoft válida.

### 2. Criação de um Recurso
- Clique em **"Criar um recurso"**
- Em seguida, selecione **"Máquina virtual"** na seção **Computação**

### 3. Configuração Básica da VM
- **Assinatura**: Free Trial
- **Grupo de recursos**: `vm-teste-rg` (novo grupo criado)
- **Nome da máquina virtual**: `vm-teste`
- **Região**: Brazil South
- **Imagem**: Ubuntu Server 24.04 LTS - x64 Gen2
- **Tamanho**: `Standard_B1s` (1 vCPU, 1 GiB RAM)
- **Usuário administrador**: `azureuser`
- **Método de autenticação**: Chave pública SSH (gerada via terminal local)

### 4. Configurações de Disco
- Tipo de disco do SO: SSD padrão
- Criação automática de disco de dados: desabilitada

### 5. Configurações de Rede
- Rede virtual: criada automaticamente
- Sub-rede: padrão
- Endereço IP público: dinâmico
- Porta SSH (22): aberta por padrão

### 6. Monitoramento e Avançado
- **Monitoramento**: Ativado (Log Analytics desativado)
- **Diagnóstico de inicialização**: habilitado
- **Extensões e scripts personalizados**: não utilizados

### 7. Revisar + Criar
- Após a validação dos dados, clique em **"Criar"**
- A implantação levou aproximadamente 2 minutos
