# 🚀 Criação de Máquina Virtual no Microsoft Azure

Este repositório documenta o processo de criação e configuração de uma máquina virtual (VM) na plataforma Microsoft Azure. O conteúdo faz parte do laboratório prático proposto pela **DIO (Digital Innovation One)**, com o objetivo de reforçar o aprendizado sobre serviços de computação na nuvem.

---

## 🎯 Objetivo

- Reforçar o uso do portal Azure
- Praticar a criação de recursos computacionais (VMs)
- Documentar o processo de forma clara e reutilizável

---

## 🛠️ Tecnologias e Ferramentas

- **Microsoft Azure**
- **Portal Web do Azure**
- (Opcional) Cliente SSH / RDP para acesso à VM
- (Opcional) Visual Studio Code com extensões remotas

---

## 📋 Etapas do Processo

### 1. Acesso ao Portal
- URL: [https://portal.azure.com](https://portal.azure.com)
- Login com conta Microsoft

### 2. Criação da Máquina Virtual
- **Menu:** Máquinas Virtuais > Criar
- **Configurações básicas:**
  - Sistema operacional: `Ubuntu Server 22.04 LTS` (ou outro)
  - Tamanho: `B1s (1 vCPU, 1 GiB de memória)` — gratuito
  - Autenticação: `Chave SSH` ou `Senha`
  - Nome da VM: `vm-azure-teste` (exemplo)
- **Rede:** Criar nova ou usar existente

### 3. Acesso à VM
- Acesso via SSH (Linux/macOS/WSL) ou via cliente RDP (Windows)
```bash
ssh azureuser@<IP_PUBLICO_DA_VM>
