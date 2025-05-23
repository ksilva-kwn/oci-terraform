# Infraestrutura da OCI como código
Terraform Configuration for OCI: VCN, Subnets, Security, and Windows VM <br>
Este repositório contém uma configuração completa do Terraform para provisionar infraestrutura na Oracle Cloud Infrastructure (OCI). 

A configuração inclui:

☁️ VCN (Virtual Cloud Network): CIDR: 10.5.0.0/16

Internet Gateway e NAT Gateway configurados. <br>
Service Gateway para acesso a serviços da OCI. <br>

<br>

Subnets:

Subnet Pública (10.5.1.0/24) com acesso à internet via Internet Gateway. <br>
Subnet Privada (10.5.2.0/24) com acesso à internet via NAT Gateway e Service Gateway.

#

🔐 Segurança:

Security Lists para tráfego público e privado. <br>
Network Security Group (NSG) configurado para a instância.

#

🖥️ Instância Windows:

Shape: VM.Standard.E5.Flex com 1 OCPU e 4 GB de RAM. <br>
Imagem personalizada do Windows Server 2019. <br>
Disco de boot de 50 GB (iSCSI). <br>
Disco Adicional de 50gb (Paravirtualized) <br>
VMssociada à subnet pública e ao NSG. <br>


`Este projeto é ideal para criar uma infraestrutura básica e segura na OCI, com suporte para instâncias públicas e privadas.`

## :memo: License

This project is under [MIT License](./LICENSE).

<p align='center'>
  Do you like my open source projects? <a href='https://stars.github.com/nominate/'>Nominate me to Github Stars ⭐</a>
</p>
