# Infraestrutura da OCI como código
Terraform Configuration for OCI: VCN, Subnets, Security, and Windows VM <br>
Este repositório contém uma configuração completa do Terraform para provisionar infraestrutura na Oracle Cloud Infrastructure (OCI). 

A configuração inclui:

VCN (Virtual Cloud Network): CIDR: 10.5.0.0/16


Internet Gateway e NAT Gateway configurados.
Service Gateway para acesso a serviços da OCI.
Subnets:

Subnet Pública (10.5.1.0/24) com acesso à internet via Internet Gateway.
Subnet Privada (10.5.2.0/24) com acesso à internet via NAT Gateway e Service Gateway.

#

Segurança:

Security Lists para tráfego público e privado.
Network Security Group (NSG) configurado para a instância.

#

Instância Windows:

Shape: VM.Standard.E5.Flex com 1 OCPU e 4 GB de RAM.
Imagem personalizada do Windows Server 2019.
Disco de boot de 50 GB (iSCSI).
Associada à subnet pública e ao NSG.


`Este projeto é ideal para criar uma infraestrutura básica e segura na OCI, com suporte para instâncias públicas e privadas.`
