# Acesso remoto com SSH

Esta atividade teve como objetivo compreender o funcionamento básico do **SSH (Secure Shell)** e preparar o ambiente Linux para um futuro teste de acesso remoto.

## Comando de ligação

A sintaxe básica é:

```bash
ssh utilizador@endereco_ip
```

Exemplo ilustrativo:

```bash
ssh ubuntu@192.168.1.100
```

> O endereço acima é apenas um exemplo. Num teste real deve ser utilizado o endereço IP efetivamente atribuído à máquina de destino.

## O que foi trabalhado

- identificação do endereço IP da máquina Linux;
- compreensão da sintaxe do comando `ssh`;
- verificação da necessidade de um serviço SSH ativo no servidor;
- análise das condições necessárias para estabelecer a ligação entre duas máquinas.

## Estado do laboratório

O ambiente utilizado é uma **VM Ubuntu Server local no VMware**. Nesta fase, o acesso remoto real a partir de outra máquina não foi concluído, por isso este documento regista a preparação e os requisitos técnicos para o teste.

## Requisitos para um teste real

Para validar uma ligação SSH entre máquinas seria necessário:

1. ter uma segunda máquina ou dispositivo capaz de alcançar a VM pela rede;
2. confirmar que o serviço OpenSSH Server está instalado e ativo;
3. identificar corretamente o endereço IP da VM;
4. configurar a rede do VMware de forma adequada, por exemplo em modo NAT ou Bridged conforme o cenário;
5. permitir o tráfego SSH no firewall apenas quando necessário;
6. utilizar credenciais válidas ou, preferencialmente, autenticação por chave num cenário mais avançado.

## Verificações úteis

Exemplos de comandos que podem ser usados para diagnosticar o ambiente:

```bash
ip addr
hostname -I
systemctl status ssh
ss -tulpn
```

Se o `ufw` estiver ativo, a configuração do firewall deve ser analisada antes de abrir qualquer porta.

## Boas práticas de segurança

- não expor o SSH à Internet sem necessidade;
- evitar passwords fracas;
- preferir autenticação por chaves em ambientes reais;
- limitar utilizadores autorizados;
- manter o sistema atualizado;
- aplicar o princípio do menor privilégio;
- registar e rever acessos quando o ambiente exigir.

## Próximo passo

Executar um teste controlado de SSH entre duas máquinas na mesma rede e documentar o resultado, incluindo configuração de rede, verificação do serviço e evidências do acesso bem-sucedido.
