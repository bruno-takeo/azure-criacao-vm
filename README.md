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
```

### 4. Testes e Configurações Iniciais

#### 🔄 Atualização do sistema:
```bash
sudo apt update && sudo apt upgrade -y
```

#### 🧰 Instalação de pacotes úteis (exemplo):
```bash
sudo apt install curl git htop -y
```

---

## 🖼️ Capturas de Tela

As imagens abaixo ilustram as principais etapas do processo.  
As capturas estão armazenadas na pasta `/images`.

- 📌 **Criação da VM:**  
  ![Criação da VM](images/passo1-criacao.png)

- 📌 **Configuração de rede:**  
  ![Configuração de rede](images/vm-configuracao.png)

- 📌 **Acesso via SSH:**  
  ![Acesso via SSH](images/acesso-vm.png)

---

## 💡 Dicas Úteis

- Utilize grupos de recursos para organizar os recursos criados
- Sempre revise as políticas de preços e limites do plano gratuito
- Lembre-se de **parar ou excluir a VM** quando não estiver em uso, para evitar cobranças

---

## ✍️ Autor

**Bruno Takeo**  
[GitHub - @bruno-takeo](https://github.com/bruno-takeo)

> _Projeto desenvolvido como parte do curso de Introdução ao Microsoft Azure, oferecido pela DIO._
