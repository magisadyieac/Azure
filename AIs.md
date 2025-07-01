## 🚀 Funcionalidades Exploradas

- **GitHub Copilot** para sugestões de código automatizadas;
- **ChatGPT** para explicações técnicas e refinamento de ideias;
- **Geração de conteúdo técnico via IA**;
- **Aplicação prática de prompts e filtros de conteúdo**.

---

## 📓 Anotações de Aprendizado

- Prompts bem elaborados resultam em respostas mais relevantes e completas;
- A IA é útil como parceira na criação e explicação de código;
- A documentação técnica pode ser significativamente agilizada com uso de ferramentas assistidas por IA;
- Importância de validar as respostas da IA antes de aplicá-las em produção.

---

## 🧪 Exemplos de Uso e Documentação Técnica

### 📌 Caso de Uso: Organização de Arquivos por Extensão

#### Objetivo
Criar um script que organize arquivos em uma pasta, separando-os por tipo de extensão (.txt, .jpg, .pdf, etc.).

#### Prompt Utilizado
> "Crie um script em Python que organize os arquivos de uma pasta em subpastas de acordo com a extensão dos arquivos."

#### Código Gerado
```python
import os
import shutil

def organizar_arquivos_por_extensao(pasta):
    for arquivo in os.listdir(pasta):
        caminho_completo = os.path.join(pasta, arquivo)

        if os.path.isfile(caminho_completo):
            extensao = arquivo.split('.')[-1]
            pasta_destino = os.path.join(pasta, extensao.upper())

            if not os.path.exists(pasta_destino):
                os.makedirs(pasta_destino)

            shutil.move(caminho_completo, os.path.join(pasta_destino, arquivo))

# Exemplo de uso:
organizar_arquivos_por_extensao('C:/Users/SeuUsuario/Downloads')
