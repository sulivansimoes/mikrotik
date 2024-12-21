# Topologia
A topologia apresentada abaixo possui a finalidade de ter 2 mikrotiks, sendo um mikrotik de borda responsável por gerenciar configurações
dhcp server e receber internet (via dhcp client), além de segmentar a infraestrutura em duas VLANs em uma porta de transporte.
O segundo mikrotik possuí as VLANs na porta que recepiciona o mikrotik 1, ou seja, na porta de transporte, é nele onde as estações de trabalho se conectarão.
Ao conectar uma estação de trabalho no mikrotik 2, ele segmentará a rede entre as VLANs de acordo com a porta que a estação de trabalho se conectou.
Ao colocar a VLAN na mesma bridge da ether fisica, o mikrotik deixa a porta fisica como ACCESS e deixa a VLAN como TRUNK.
A configuração presente nos backups e scripts não realizam isolamento entre as VLANs, ou seja, uma estação conectada em uma VLAN consegue acessar outra estação conectada em outra VLAN.

<img  alt="preview" src="https://raw.githubusercontent.com/sulivansimoes/mikrotik/refs/heads/main/VLAN%20-%20BRIDGE%20COM%20TRUNK%20E%20ACESS/topologia.png">

## Responsabilidade 
Esse repositório contém topologias e scripts usados para estudo em ambiente de laboratório. 
Cada topologia tem objetivo estreito e bem definido, ou seja, uma topologia VLAN não foca em regras
de firewall contra ataques externos. Caso tenha caído nesse reposítório de :parachute: e queira usar o conteúdo presente aqui
para estudo e afins, fique a vontade, mas ao colocar um script ou backup em ambiente de produção, você fica responsável :bomb:! 


