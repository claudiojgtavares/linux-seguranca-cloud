# Linux, Segurança e Cloud

Laboratório prático desenvolvido no contexto da formação **Skodji Digital**, com foco em administração básica de Linux, permissões, segurança e preparação para ambientes de cloud.

> **Estado do projeto:** em evolução. Este repositório será atualizado à medida que avanço no módulo e realizo novas atividades práticas.

## 🎯 Objetivos

- Preparar um ambiente Linux com Ubuntu Server.
- Praticar comandos essenciais de administração no terminal.
- Compreender permissões de ficheiros e o princípio do menor privilégio.
- Explorar conceitos de acesso remoto com SSH.
- Relacionar máquinas virtuais, VPS e infraestrutura em cloud.
- Documentar atividades e evidências de forma organizada no GitHub.

## 🖥️ Ambiente utilizado

- **Sistema anfitrião:** Windows 11
- **Virtualização:** VMware
- **Sistema convidado:** Ubuntu Server
- **Tipo de ambiente:** máquina virtual local para laboratório

## 🧰 Comandos e conceitos praticados

Alguns dos comandos utilizados durante as atividades:

```bash
pwd
ls
mkdir
nano
uname -a
hostname
```

Também foram trabalhados conceitos como:

- estrutura de diretórios;
- utilizadores e grupos;
- permissões de leitura, escrita e execução;
- princípio do menor privilégio;
- preparação para SSH;
- diferenças entre VM, VPS e infraestrutura em cloud.

## 🔐 Permissões e segurança

Foi realizada uma atividade específica sobre permissões de ficheiros, com exemplos como `644`, `640` e permissão de execução apenas para o proprietário.

➡️ [Ver documentação sobre permissões](./permissoes.md)

## 🌐 Acesso remoto com SSH

O laboratório também inclui preparação para acesso remoto via SSH. Como o ambiente utilizado é uma VM local isolada, o acesso remoto real entre máquinas não foi concluído nesta fase.

➡️ [Ver documentação sobre acesso remoto](./acesso-remoto.md)

## 📸 Evidências

As capturas de ecrã das atividades estão organizadas nas seguintes pastas:

- [Evidências iniciais](./Evidencias)
- [Evidências das atividades de permissões e utilizadores](./Evidencias%202)

Também está disponível o relatório produzido no contexto do trabalho:

- [Relatório do trabalho de grupo](./Relat%C3%B3rio%20do%20trabalho%20de%20grupo.pdf)

## ☁️ VM, VPS e Cloud

**VM local:** máquina virtual executada no próprio computador, útil para aprendizagem, testes e ambientes isolados.

**VPS:** servidor virtual alojado num datacenter e normalmente acedido através da Internet, com recursos dedicados ou partilhados conforme o serviço contratado.

**Infraestrutura em cloud:** conjunto de serviços computacionais disponibilizados por fornecedores de cloud, permitindo criar, gerir e escalar recursos conforme a necessidade.

## 📚 Aprendizagens

Este laboratório ajudou-me a consolidar:

- utilização prática do terminal Linux;
- organização de ficheiros e diretórios;
- importância das permissões corretas;
- relação entre controlo de acessos e segurança de sistemas;
- documentação técnica de atividades;
- utilização do GitHub como registo de evolução prática.

## 🚧 Próximos passos

- aprofundar comandos e administração de Ubuntu Server;
- praticar utilizadores, grupos e permissões avançadas;
- testar SSH entre máquinas num ambiente controlado;
- explorar firewall e serviços de rede;
- relacionar o laboratório local com ambientes VPS/cloud;
- continuar a melhorar a documentação do repositório.

---

**Autor:** Cláudio Tavares  
**Área:** Engenharia de Sistemas e Informática / Tecnologias de Informação  
**Contexto:** Skodji Digital — formação em andamento
