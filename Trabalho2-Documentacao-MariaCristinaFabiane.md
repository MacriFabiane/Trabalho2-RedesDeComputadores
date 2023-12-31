# Trabalho 2: Integração de habilidades - 2023/2
**Disciplina: Redes de Computadores**

**Curso: Engenharia de Computação / Elétrica**

**Nome/RA: Maria Cristina Fabiane/2456591**


## Tarefa 1:  Sub-Redes
| Sub- Rede |             IPv6 - Sub-Rede            |  IPv4 - Sub-Rede  |  IPv4 - Máscara   | 
|:---------:|:--------------------------------------:|:-----------------:|:-----------------:|
| Matriz    | 2001:DB8:CAFE:**5B** *00* ::/64 | 200.136.**91**.*0*   | 255.255.255.*192* | 
| Filial 1  | 2001:DB8:CAFE:**5B** *01* ::/64 | 200.136.**91**.*64*  | 255.255.255.*224* | 
| Filial 2  | 2001:DB8:CAFE:**5B** *02* ::/64 | 200.136.**91**.*196*  | 255.255.255.*224* | 
| Filial 3  | 2001:DB8:CAFE:**5B** *03* ::/64 | 200.136.**91**.*128* | 255.255.255.*224* | 
| Filial 4  | 2001:DB8:CAFE:**5B** *04* ::/64 | 200.136.**91**.*160* | 255.255.255.*224* |
| Filial 5  | 2001:DB8:CAFE:**5B** *05* ::/64 | 200.136.**91**.*192* | 255.255.255.*224* |
| pb-vit    | 2001:DB8:CAFE:**5B**FF:: *0* :0/112 | 200.136.**91**.*224* | 255.255.255.*252* |
| vit-fb    | 2001:DB8:CAFE:**5B**FF:: *1* :0/112 | 200.136.**91**.*228* | 255.255.255.*252* |
| fb-ita    | 2001:DB8:CAFE:**5B**FF:: *2* :0/112 | 200.136.**91**.*232* | 255.255.255.*252* | 
| ita-pb    | 2001:DB8:CAFE:**5B**FF:: *3* :0/112 | 200.136.**91**.*236* | 255.255.255.*252* | 
| ita-cv    | 2001:DB8:CAFE:**5B**FF:: *4* :0/112  | 200.136.**91**.*240* | 255.255.255.*252* | 


## Tarefa 2: Endereçamento de Dispositivos
| Dispositivo           |Interface|      IPv4     |  IPv4 - Máscara |IPv4 - Gateway|      IPv6/Prefixo (GUA)     | IPv6 (LLA) |IPv6-Gateway|
|:-----------------------:|:---------:|---------------|-----------------|--------------|-----------------------------|------------|---------|
| PC1                   | NIC     | 200.136.**91**.*3*   | 255.255.255.*192* | 200.136.**91**.*1*   | 2001:DB8:CAFE:**5B** *00*::*3*/64    |   EUI-64   | FE80::1 |
| PC2                   | NIC     | 200.136.**91**.*4*   | 255.255.255.*192* | 200.136.**91**.*1*   | 2001:DB8:CAFE:**5B***00*::*4*/64    |   EUI-64   | FE80::1 |
| PC3                   | NIC     | 200.136.**91**.*67*  | 255.255.255.*224* | 200.136.**91**.*65* | 2001:DB8:CAFE:**5B***01*::*3*/64    |   EUI-64   | FE80::1 |
| PC4                   | NIC     | 200.136.**91**.*68*  | 255.255.255.*224* | 200.136.**91**.*65* | 2001:DB8:CAFE:**5B***01*::*4*/64    |   EUI-64   | FE80::1 |
| PC5                   | NIC     | 200.136.**91**.*99*  | 255.255.255.*224* | 200.136.**91**.*197* | 2001:DB8:CAFE:**5B***02*::*3*/64    |   EUI-64   | FE80::1 |
| PC6                   | NIC     | 200.136.**91**.*100* | 255.255.255.*224* | 200.136.**91**.*197* | 2001:DB8:CAFE:**5B***02*::*4*/64    |   EUI-64   | FE80::1 |
| Switch-Matriz         | SVI     | 200.136.**91**.*2*   | 255.255.255.*192* | 200.136.**91**.*1*  |             -               |     -      |    -    |
| Switch-Filial1        | SVI     | 200.136.**91**.*66*  | 255.255.255.*224* | 200.136.**91**.*65* |             -               |     -      |    -    |
| Switch-Filial2        | SVI     | 200.136.**91**.*98*  | 255.255.255.*224* | 200.136.**91**.*197* |             -               |     -      |    -    |
| Roteador-Pato Branco  | Fa0/0   | 200.136.**91**.*1*   | 255.255.255.*192* |      -       | 2001:DB8:CAFE:**5B** *00*::*1*/64    |   FE80::1  |    -    |
| Roteador-Pato Branco  | Se0/0/0 | 200.136.**91**.*225* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*0*:*1*/112 |   EUI-64   |    -    |
| Roteador-Pato Branco  | Se0/0/1 | 200.136.**91**.*238* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*3*:*2*/112 |   EUI-64   |    -    |
| Roteador-Fco. Beltrão | Fa0/0   | 200.136.**91**.*65*  | 255.255.255.*224* |      -       | 2001:DB8:CAFE:**5B** *01*::*1*/64    |   FE80::1  |    -    |
| Roteador-Fco. Beltrão | Se0/0/0 | 200.136.**91**.*233* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*2*:*1*/112 |   EUI-64   |    -    |
| Roteador-Fco. Beltrão | Se0/0/1 | 200.136.**91**.*230* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*1*:*2*/112 |   EUI-64   |    -    | 
| Roteador-Vitorino     | Se0/0/0 | 200.136.**91**.*229* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*1*:*1*/112 |   EUI-64   |    -    | 
| Roteador-Vitorino     | Se0/0/1 | 200.136.**91**.*226* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*0*:*2*/112 |   EUI-64   |    -    | 
| Roteador-Itapejara    | Se0/0/0 | 200.136.**91**.*237* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*3*:*1*/112 |   EUI-64   |    -    | 
| Roteador-Itapejara    | Se0/0/1 | 200.136.**91**.*234* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*2*:*2*/112 |   EUI-64   |    -    | 
| Roteador-Itapejara    | Fa0/1   | 200.136.**91**.*241* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*4*:*1*/112 |   EUI-64   |    -    | 
| Roteador-Coronel      | Fa0/0   | 200.136.**91**.*197*  | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B** *02*::*1*/64    |   FE80::1  |    -    |
| Roteador-Coronel      | Fa0/1   | 200.136.**91**.*242* | 255.255.255.*252* |      -       | 2001:DB8:CAFE:**5B**FF::*4*:*2*/112 |   EUI-64   |    -    | 



## Tarefa 3: Tabela de Roteamento
### IPv4

#### Roteador Pato Branco
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|      (WAN V-FB) 200.136.91.228            |      255.255.255.252           |    200.136.91.226               |       Se0/0/0             | 
|           (WAN FB-ITA) 200.136.91.232       |     255.255.255.252            |    200.136.91.226                |Se0/0/0      | 
|   (WAN ITA-CV)    200.136.91.240            |    255.255.255.252             |         200.136.91.226          |        Se0/0/0            | 
|       (LANF1)   200.136.91.64         |        255.255.255.224         |      200.136.91.226             |          Se0/0/0          | 
|       (LANF2)    200.136.91.96        |      255.255.255.224           |   200.136.91.226                |     Se0/0/0               | 


#### Roteador Francisco Beltrão
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|      (WAN PB-VIT)  200.136.91.224           |   255.255.255.252              |      	200.136.91.234           |       Se0/0/0             | 
|        (WAN ITA-CV) 200.136.91.240          |      255.255.255.252           |      200.136.91.234               |    Se0/0/0                | 
|         (WAN ITA-PB)  200.136.91.236        |      255.255.255.252           |               200.136.91.234      |      Se0/0/0              | 
|       (LANM)  200.136.91.0          |     255.255.255.192            |                200.136.91.234     |     Se0/0/0               | 
|   (LANF2)    200.136.91.96            |      255.255.255.224           |              200.136.91.234       |        Se0/0/0            | 

#### Roteador Vitorino
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|     (WAN FB-ITA)     200.136.91.232         |    255.255.255.252    	           |         200.136.91.230        |       Se0/0/0             | 
|      (WAN ITA-CV)   200.136.91.240          |        255.255.255.252         |        200.136.91.230          |          Se0/0/0          | 
|     (WAN ITA-PB)    200.136.91.236          |         255.255.255.252        |                 200.136.91.230     |          Se0/0/0          | 
|       (LANM) 200.136.91.0           |    255.255.255.192             |               200.136.91.230       |        Se0/0/0            | 
|         (LANF1)   200.136.91.64       |        	255.255.255.224         |               200.136.91.230       |      Se0/0/0              |                 
|      (LANF2)   200.136.91.96      |  	255.255.255.224       |      200.136.91.230           |   Se0/0/0      |

#### Roteador Itapejara D'Oeste
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|     (WAN VIT-FB)    200.136.91.228          |         255.255.255.252        |         200.136.91.238          |       Se0/0/0             | 
|     (WAN PB-VIT)   200.136.91.224           |        255.255.255.252         |      200.136.91.238             |      Se0/0/0              | 
|          (LANM)  200.136.91.0       |     255.255.255.192            |                  200.136.91.238 |      Se0/0/0              | 
|       (LANF1) 200.136.91.64            |     255.255.255.224            |                 200.136.91.238  |         Se0/0/0           | 
|   (LANF2)   200.136.91.96             |    255.255.255.224             |        200.136.91.242          |           Fa0/1         | 

#### Roteador Coronel Vivida
|  Rede de Destino  |     Máscara     |     Next Hop      | Interface de Saída |
|-------------------|-----------------|-------------------|--------------------|
|     (WAN FB-ITA)     200.136.91.232         |    255.255.255.252    	           |        200.136.91.241        |       Fa0/1            | 
|      (WAN PB-VIT)  200.136.91.224      |        255.255.255.252         |       200.136.91.241          |          Fa0/1         | 
|     (WAN ITA-PB)    200.136.91.236          |         255.255.255.252        |                200.136.91.241     |          Fa0/1         | 
|(WAN VIT-FB) 200.136.91.228      |   255.255.255.252      |          200.136.91.241        | Fa0/1  |
|       (LANM) 200.136.91.0           |    255.255.255.192             |              200.136.91.241       |        Fa0/1           | 
|         (LANF1)   200.136.91.64       |        	255.255.255.224         |              200.136.91.241       |      Fa0/1             |                 
|      (LANF2)   200.136.91.96      |  	255.255.255.224       |     200.136.91.241           |   Fa0/1     |

### IPv6
#### Roteador Pato Branco
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|      (WAN V-FB) 2001:DB8:CAFE:5BFF::1:0/112           |   2001:DB8:CAFE:5BFF::0:2/112              |       Se0/0/0             | 
|           (WAN FB-ITA) 2001:DB8:CAFE:5BFF::2:0/112          |   2001:DB8:CAFE:5BFF::0:2/112               |Se0/0/0      | 
|   (WAN ITA-CV) 2001:DB8:CAFE:5BFF::4:0/112          |        2001:DB8:CAFE:5BFF::0:2/112         |        Se0/0/0            | 
|       (LANF1)   2001:DB8:CAFE:5B01::/64        |     2001:DB8:CAFE:5BFF::0:2/112            |          Se0/0/0          | 
|       (LANF2)    2001:DB8:CAFE:5B02::/64                  |  2001:DB8:CAFE:5BFF::0:2/112               |     Se0/0/0               | 
      
      
#### Roteador Francisco Beltrão
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|      (WAN PB-VIT) 2001:DB8:CAFE:5BFF::0:0/112       |      	2001:DB8:CAFE:5BFF::2:2/112           |       Se0/0/0             | 
|        (WAN ITA-CV) 2001:DB8:CAFE:5BFF::4:0/112            |      2001:DB8:CAFE:5BFF::2:2/112               |    Se0/0/0                | 
|         (WAN ITA-PB)  2001:DB8:CAFE:5BFF::3:0/112           |               2001:DB8:CAFE:5BFF::2:2/112      |      Se0/0/0              | 
|       (LANM)  2001:DB8:CAFE:5B00::/64      |                2001:DB8:CAFE:5BFF::2:2/112     |     Se0/0/0               | 
|   (LANF2)    2001:DB8:CAFE:5B02::/64    |              2001:DB8:CAFE:5BFF::2:2/112       |        Se0/0/0            | 
      
#### Roteador Vitorino
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|     (WAN FB-ITA)    2001:DB8:CAFE:5BFF::2:0/112       |       2001:DB8:CAFE:5BFF::1:2/112        |       Se0/0/0             | 
|      (WAN ITA-CV)   2001:DB8:CAFE:5BFF::4:0/112       |      2001:DB8:CAFE:5BFF::1:2/112          |          Se0/0/0          | 
|     (WAN ITA-PB)   2001:DB8:CAFE:5BFF::3:0/112      |               2001:DB8:CAFE:5BFF::1:2/112     |          Se0/0/0          | 
|       (LANM) 2001:DB8:CAFE:5B00::/64      |             2001:DB8:CAFE:5BFF::1:2/112       |        Se0/0/0            | 
|         (LANF1)   2001:DB8:CAFE:5B01::/64        |             2001:DB8:CAFE:5BFF::1:2/112       |      Se0/0/0              |                 
|      (LANF2)  2001:DB8:CAFE:5B02::/64   |    2001:DB8:CAFE:5BFF::1:2/112           |   Se0/0/0      |
      
#### Roteador Itapejara D'Oeste
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|     (WAN VIT-FB)   2001:DB8:CAFE:5BFF::1:0/112   |         2001:DB8:CAFE:5BFF::3:2/112 |       Se0/0/0             | 
|     (WAN PB-VIT)   2001:DB8:CAFE:5BFF::0:0/112   |   2001:DB8:CAFE:5BFF::3:2/112 | Se0/0/0              | 
|          (LANM) 2001:DB8:CAFE:5B00::/64    | 2001:DB8:CAFE:5BFF::3:2/112  |   Se0/0/0              | 
|       (LANF1) 2001:DB8:CAFE:5B01::/64      |  2001:DB8:CAFE:5BFF::3:2/112  | Se0/0/0           | 
|   (LANF2)   2001:DB8:CAFE:5B02::/64  |   2001:DB8:CAFE:5BFF::4:2/112    |   Fa0/1        | 
      
#### Roteador Coronel Vivida
| Rede de Destino/Prefixo      | Next Hop                     | Interface de Saída |
|------------------------------|------------------------------|--------------------|
|     (WAN FB-ITA)    2001:DB8:CAFE:5BFF::2:0/112     |        2001:DB8:CAFE:5BFF::4:1/112        |       Fa0/1            | 
|      (WAN PB-VIT) 2001:DB8:CAFE:5BFF::0:0/112   |       2001:DB8:CAFE:5BFF::4:1/112          |          Fa0/1         | 
|     (WAN ITA-PB)    2001:DB8:CAFE:5BFF::3:0/112   |                2001:DB8:CAFE:5BFF::4:1/112     |          Fa0/1         | 
|(WAN VIT-FB)  2001:DB8:CAFE:5BFF::1:/112      |          2001:DB8:CAFE:5BFF::4:1/112        | Fa0/1  |
|       (LANM) 2001:DB8:CAFE:5B00::/64   |            2001:DB8:CAFE:5BFF::4:1/112       |        Fa0/1           | 
|         (LANF1)   2001:DB8:CAFE:5B01::/64      |              2001:DB8:CAFE:5BFF::4:1/112       |      Fa0/1             |                 
|      (LANF2)  2001:DB8:CAFE:5B02::/64  |     2001:DB8:CAFE:5BFF::4:1/112           |   Fa0/1     |

## Topologia - Packet Tracer
- [ ] ![Trabalho2-Topologia-NomeAluno](trabalho2-20222-topologia-NomeAluno.pkt)

