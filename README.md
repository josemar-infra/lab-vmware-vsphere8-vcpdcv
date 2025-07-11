# Laboratório VMware vSphere 8 para Certificação VCP-DCV 💻 

Este repositório documenta o laboratório completo que desenvolvi como parte da minha preparação para a certificação **VCP-DCV (VMware Certified Professional – Data Center Virtualization)**, já concluída com sucesso.  
O ambiente foi construído com base em **VMware vSphere 8** e serviu como plataforma prática para consolidar os conhecimentos exigidos no exame oficial da VMware.

---

## 🧰 Infraestrutura Utilizada

- Servidor físico: HP ProLiant DL380p Gen8
- Memória RAM: 64 GB
- Armazenamento: 5 discos SAS de 300 GB
- Sistema base: Windows Server 2016 (instalado diretamente no servidor)
- Virtualizador: VMware Workstation 16 Pro (executando todas as VMs do lab)

---

## 🎯 Objetivo do Projeto

Construir um ambiente de laboratório que simule uma infraestrutura de datacenter virtualizado, possibilitando o estudo e prática de recursos essenciais do vSphere 8, incluindo:

- Instalação e gerenciamento do vCenter Server
- Hosts ESXi
- Switches virtuais
- Armazenamento via iSCSI (com LUNs HP configuradas em VSA)
- Domínio Active Directory integrado ao ambiente vSphere
- Recursos de alta disponibilidade (HA)
- Balanceamento (DRS)
- Tolerância a falhas (FT)
- Criação e gerenciamento de VMs
- vSAN, vMotion e monitoramento de desempenho

---

## 🧱 Arquitetura do Ambiente

> Todo o ambiente foi implementado **dentro do VMware Workstation 16 Pro**, que por sua vez roda sobre o **Windows Server 2016** instalado diretamente no servidor físico.

### Componentes Virtuais Criados:

- **3 Hosts ESXi 8.0 U2**
- **1 vCenter Server 8.0**
- **1 VSA (HP Storage - Storage Virtual Appliance) com LUNs iSCSI**
- **1 Active Directory (Windows Server 2016), para gerenciamento de domínio**
- **Várias VMs de teste para laboratório**

---

## 🗺️ Topologia do Laboratório

![Topologia](imagens/topologia.png)

---

## 📄 Documentação

- [Roteiro do Laboratório em PDF](docs/documentacao.pdf)

---

## 🛠️ Etapas de Implementação

1. Instalação das VMs no VMware Workstation
2. Deploy do Windows Server 2016 como sistema base
3. Instalação dos ESXi 8.0 dentro do Workstation
4. Deploy e configuração do vCenter Server 8.0
5. Instalação do Storage HP VSA com LUNs iSCSI (VMFS e NFS)
6. Integração com Active Directory e junção ao domínio
7. Criação de VMs de teste
8. Configuração de recursos como HA, FT, DRS, vMotion e vSAN
9. Monitoramento e gestão de recursos via vCenter

---

## 📁 Organização do Repositório

| Pasta             | Conteúdo                                                         |
|------------------|------------------------------------------------------------------|
| `imagens/`       | Screenshots do laboratório, topologia e mapas mentais            |
| `docs/`          | Documentos de apoio, anotações técnicas, arquivos PDF, Visio     |
| `configuracoes/` | Scripts de configuração, arquivos `.ovf`, `.txt`, entre outros   |

---

## 🎓 Certificação Alvo

> ✅ Certificação Concluída: VCP-DCV – VMware Certified Professional - Data Center Virtualization

Este laboratório foi construído como parte da minha preparação para a certificação **VCP-DCV**, a qual conquistei com êxito. A experiência prática adquirida nesse ambiente foi essencial para consolidar os conhecimentos exigidos no exame, especialmente em temas como virtualização de data center, alta disponibilidade, vSAN, vMotion, DRS, e gestão centralizada via vCenter.


---

## 👨‍💻 Sobre o Autor

**Josemar Maximino**
Systems & Infrastructure Administrator | On-Premises & Clound

🔗 [LinkedIn](https://www.linkedin.com/in/josemar-maximino-8bb974251?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app)  
📧 Email: josemarmateus2003@gmail.com

---

## 📌 Observações

Este projeto é de uso educacional e tem como objetivo auxiliar estudantes e profissionais da área de infraestrutura na preparação para exames de certificação, bem como no desenvolvimento de habilidades práticas em ambientes virtualizados corporativos.

---

## 🙏 Agradecimentos

Este projeto foi inspirado no curso **"Virtualização de servidores com VMware vSphere 7.0"** ministrado por **John Costa**, criador do canal e marca **Expert em TI**.  
A topologia e os conceitos abordados seguem a estrutura do treinamento, adaptados e personalizados para minha infraestrutura local.  
🔗 [Canal do Expert em TI no YouTube](https://www.youtube.com/@ExpertemTI)
