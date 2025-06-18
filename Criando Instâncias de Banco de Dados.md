Criação de Instância de Banco de Dados para teste



1. Entre em [https://portal.azure.com](https://portal.azure.com)
2. No menu esquerdo, clique em **"Criar um recurso"**
3. Em seguida, selecione **"Banco de dados" > "Azure Database for MySQL – Servidor flexível"**

---

### 2. Preencha as Informações Básicas

| Campo                     | Valor sugerido                          |
|---------------------------|------------------------------------------|
| **Assinatura**            | Free Trial ou ativa                      |
| **Grupo de recursos**     | `meu-grupo-banco` (crie um novo, se necessário) |
| **Nome do servidor**      | `meu-servidor-mysql`                    |
| **Região**                | Brazil South (ou a mais próxima)         |
| **Modo de disponibilidade** | Sem redundância                       |
| **Versão do MySQL**       | 8.0                                     |
| **Usuário admin**         | `adminuser`                              |
| **Senha**                 | (crie uma senha forte)                   |

---

### 3. Escolha o Plano de Computação

- Selecione o plano **"Burstável"** para menor custo
- Tamanho sugerido: **B1MS** (1 vCPU, 2 GB RAM) – elegível à camada gratuita
- Armazenamento: **32 GB** (limite da camada gratuita)

> ℹ️ Camada gratuita disponível em algumas regiões. Pode ser necessário selecionar "East US" se indisponível no Brasil.

---

### 4. Configure a Rede

- Tipo de acesso: **Acesso público**
- Clique em "Adicionar endereço IP atual" para permitir acesso externo
- Opcional: configure regras de firewall específicas por faixa de IP

---

### 5. Políticas de Backup

- Retenção padrão: 7 dias
- Criptografia: habilitada por padrão
- Local de backup: na mesma região

---

### 6. Revisar e Criar

- Revise todos os campos preenchidos
- Clique em **"Criar"**
- A criação leva entre 3 e 10 minutos
