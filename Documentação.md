# Trabalho 2: Integração de habilidades - 2023/1
**Disciplina: Redes de Computadores**

**Curso: Engenharia de Computação / Elétrica**

**Nome/RA: Maria Cristina Fabiane/2456591**


## Tarefa 1:  Sub-Redes
| Sub- Rede |             IPv6 - Sub-Rede            |  IPv4 - Sub-Rede  |  IPv4 - Máscara   | 
|:---------:|:--------------------------------------:|:-----------------:|:-----------------:|
| Matriz    | 2001:DB8:CAFE:**5B** *00* ::/64 | 200.136.**91**.*00*   | 255.255.255.*192* | 
| Filial 1  | 2001:DB8:CAFE:**5B** *01* ::/64 | 200.136.**91**.*64*  | 255.255.255.*224* | 
| Filial 2  | 2001:DB8:CAFE:**5B** *02* ::/64 | 200.136.**91**.*196*  | 255.255.255.*224* | 
| Filial 3  | 2001:DB8:CAFE:**5B** *03* ::/64 | 200.136.**91**.*128* | 255.255.255.*224* | 
| Filial 4  | 2001:DB8:CAFE:**5B** *04* ::/64 | 200.136.**91**.*160* | 255.255.255.*224* |
| Filial 5  | 2001:DB8:CAFE:**5B** *05* ::/64 | 200.136.**91**.*192* | 255.255.255.*224* |
| pb-vit    | 2001:DB8:CAFE:**5B**FF:: *??* :0/112 | 200.136.**91**.*??* | 255.255.255.*??* |
| vit-fb    | 2001:DB8:CAFE:**5B**FF:: *??* :0/112 | 200.136.**91**.*??* | 255.255.255.*??* |
| fb-ita    | 2001:DB8:CAFE:**5B**FF:: *??* :0/112 | 200.136.**91**.*??* | 255.255.255.*??* | 
| ita-pb    | 2001:DB8:CAFE:**5B**FF:: *??* :0/112 | 200.136.**91**.*??* | 255.255.255.*??* | 
| cv-ita    | 2001:DB8:CAFE:**5B**FF:: *??* :0/112  | 200.136.**91**.*??* | 255.255.255.*??* | 


## Tarefa 2: Endereçamento de Dispositivos
| Dispositivo           |Interface|      IPv4     |  IPv4 - Máscara |IPv4 - Gateway|      IPv6/Prefixo (GUA)     | IPv6 (LLA) |IPv6-Gateway|
|:-----------------------:|:---------:|---------------|-----------------|--------------|-----------------------------|------------|---------|
| PC1                   | NIC     | 200.134.**N**.*??*   | 255.255.255.*??* | 200.134.**N**.*??*  | 2001:DB8:CAFE:**NN***??*::*??*/64    |   EUI-64   | FE80::1 |
| PC2                   | NIC     | 200.134.**N**.*??*   | 255.255.255.*??* | 200.134.**N**.*??*  | 2001:DB8:CAFE:**NN***??*::*??*/64    |   EUI-64   | FE80::1 |
| PC3                   | NIC     | 200.134.**N**.*??*  | 255.255.255.*??* | 200.134.**N**.*??* | 2001:DB8:CAFE:**NN***??*::*??*/64    |   EUI-64   | FE80::1 |
| PC4                   | NIC     | 200.134.**N**.*??*  | 255.255.255.*??* | 200.134.**N**.*??* | 2001:DB8:CAFE:**NN***??*::*??*/64    |   EUI-64   | FE80::1 |
| PC5                   | NIC     | 200.134.**N**.*??*  | 255.255.255.*??* | 200.134.**N**.*??* | 2001:DB8:CAFE:**NN***??*::*??*/64    |   EUI-64   | FE80::1 |
| PC6                   | NIC     | 200.134.**N**.*??* | 255.255.255.*??* | 200.134.**N**.*??* | 2001:DB8:CAFE:**NN***??*::*??*/64    |   EUI-64   | FE80::1 |
| Switch-Matriz         | SVI     | 200.134.**N**.*??*   | 255.255.255.*??* | 200.134.**N**.*??*  |             -               |     -      |    -    |
| Switch-Filial1        | SVI     | 200.134.**N**.*??*  | 255.255.255.*??* | 200.134.**N**.*??* |             -               |     -      |    -    |
| Switch-Filial2        | SVI     | 200.134.**N**.*??*  | 255.255.255.*??* | 200.134.**N**.*??* |             -               |     -      |    -    |
| Roteador-Pato Branco  | Fa0/0   | 200.134.**N**.*??*   | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN** *??*::*??*/64    |   FE80::1  |    -    |
| Roteador-Pato Branco  | Se0/0/0 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    |
| Roteador-Pato Branco  | Se0/0/1 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    |
| Roteador-Fco. Beltrão | Fa0/0   | 200.134.**N**.*??*  | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN** *??*::*??*/64    |   FE80::1  |    -    |
| Roteador-Fco. Beltrão | Se0/0/0 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    |
| Roteador-Fco. Beltrão | Se0/0/1 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 
| Roteador-Vitorino     | Se0/0/0 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 
| Roteador-Vitorino     | Se0/0/1 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 
| Roteador-Itapejara    | Se0/0/0 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 
| Roteador-Itapejara    | Se0/0/1 | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 
| Roteador-Itapejara    | Fa0/1   | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 
| Roteador-Coronel      | Fa0/0   | 200.134.**N**.*??*  | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN** *??*::*??*/64    |   FE80::1  |    -    |
| Roteador-Coronel      | Fa0/1   | 200.134.**N**.*??* | 255.255.255.*??* |      -       | 2001:DB8:CAFE:**NN**FF::*??*:*??*/112 |   EUI-64   |    -    | 



## Tarefa 3: Tabela de Roteamento
#### IPv4

### Roteador Pato Branco
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 


#### Roteador Francisco Beltrão
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 

#### Roteador Vitorino
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 

#### Roteador Itapejara D'Oeste
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 

#### Roteador Coronel Vivida
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 
|                   |                 |                   |                    | 


### IPv6
#### Roteador Pato Branco
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
      
      
#### Roteador Francisco Beltrão
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
      
#### Roteador Vitorino
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
      
#### Roteador Itapejara D'Oeste
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
      
#### Roteador Coronel Vivida
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |
|                              |                              |                    |

## Topologia - Packet Tracer
- [ ] ![Trabalho2-Topologia-NomeAluno](trabalho2-20222-topologia-NomeAluno.pkt)

