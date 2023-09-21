# Introdução a Redes de Computadores 🌐

<p align="center" width="300px">
  <img width="300px" src="https://cdn-icons-png.flaticon.com/512/3518/3518210.png">
</p>

Nesse repositório irei compartilhar alguns conhecimentos adquiridos aos meus anos de vida sobre Redes de Computadores. Irão desde o básico, o famoso "feijão com arroz" até alguns possíveis tópicos mais avançados.


### O que é uma Rede de Computadores? ###
“Conjunto de computadores computadores autônomos autônomos interconectados por uma única tecnologia” - Andrew S. Tanenbaum.
Podemos entender uma rede de computadores como um meio de dispositivos conectados a fim de transmitir informações. Essas informações podem ser trocadas por meios físicos como cabos e fibra ópticas e não físicos como ondas e satélite. 

<p align="center">
  <img width="350px" src="https://cecead.com/wp-content/uploads/2020/07/Comunica%C3%A7%C3%A3o-de-Dados.png">
</p>

#### Utilização das redes
Vamos pensar atualmente em um cenário empresarial, um escritório. Dentro desse escritório temos diversas máquinas que precisam compartilhar arquivos entre si, não se restringindo somente a computadores; incluindo impressoras, scanners e banco de dados que precisam ser acessados remotamente. Em ambos casos precisamos de uma máquina central que armazenará essas informações, o servidor.

<p align="center">
  <img width="370px" src="https://cdn.papercut.com/web/img/help/manuals/print-deploy/print-server-local-domain.png">
</p>

#### Cliente-Servidor
A situação descrita acima é um tipo de conexão chamado Cliente-Servidor em que um cliente faz uma solicitação e o servidor devolve a resposta. Esse modelo é aplicável em ambientes que a máquina do cliente e o servidor se encontram próximos um do outro (Como na mesma sala) ou longínquo como prédios diferentes.
Esses servidores podem ser de impressão, arquivos, e-mail, etc.

<p align="center">
  <img width="350px" src="https://camo.githubusercontent.com/a61ec8cf009a87cc79280f3a7d881364556ef690f98ea771a57ff0c575aed70a/687474703a2f2f692e696d6775722e636f6d2f4e63564d477a352e706e67">
</p>

#### Ponto a ponto
A arquitetura ponto a ponto (P2P) é aquela em que os computadores conectados tem privilégios e capacidades iguais. De tal forma, não existe um servidor central, cada dispositivo pode atuar como cliente ou como servidor. 

<p align="center">
  <img width="350px" src="https://www.gta.ufrj.br/ensino/eel878/redes1-2018-1/trabalhos-v1/p2p/images/p2p_model.png">
</p>

_________________________________________________________________________________________________

### Topologia de Rede
A topologia de rede é a forma como você organiza os elementos de uma rede de comunicação. A topologia de rede pode ser lógica ou física; a topologia lógica descreve o fluxo de dados na rede enquanto a física estabelece o layout da rede.

- **Topologia estrela**: É o tipo de topologia mais comum, nela os hosts são conectados a um dispositivo central que gerencia a transmissão de dados na rede.
- **Topologia barramento**: Conhecida como topologia backbone, distribui os dispositivos ao longo de um único cabo que vão de uma ponta a outra da rede.
- **Topologia anel**: Os nós (comunicação entre dispositivos) são configurados de forma circular, ou seja, os dados viajam todos os dispositivos até achar o destinatário.

Além dessas, existem diversas outras topologias de rede:
<p align="center">
  <img width="370px" src="https://anlix.io/wp-content/uploads/2022/02/topologia-exempllo-1024x685.png">
</p>

### Quais os tipos de redes de computadores?
Dependendo do tamanho e das funcionalidades da rede, elas recebem nomenclaturas e organizações diferentes.
*Tópicos embasados no site aws.amazon.com*

#### Rede de área local (LAN):
Uma LAN (Rede local) é um sistema interconectado limitado a um tamanho local. Normalmente as LAN's estão alocadas em algum edifício ou escritório. Uma rede local geralmente é configurada em ambientes do tipo "cliente-servidor", onde vários computadores compartilham programas, recursos e dados com outros dispositivos da rede (nós).

#### Redes de longa distância (WAN):
Uma rede, normalmente empresarial, que abrange edifícios ou cidades. Diferentemente das LAN's que são configuradas para transmitir dados em velocidades altas e pequena distância, as WAN's são configuradas para propagar os dados por distâncias maiores de maneira segura.

#### Redes de provedores de Serviço: 
As redes de provedores de serviço oferta aos clientes um aluguel da capacidade e funcionalidades de rede do provedor. Podem ser empresas de telecomunicações, provedoras de serviço de Internet, etc.

#### Redes em nuvem
As redes em nuvem podem ser entendidas como uma WAN em que a infraestrutura está alocada na nuvem. Atualmente as redes em nuvem são utilizadas a fim de diminuir os gastos com Hardware e alocação de ativos de rede, aproveitando seus benefícios.

<p align="center">
  <img width="350px" src="https://media.licdn.com/dms/image/C4D12AQF1VNs5oJD8uQ/article-cover_image-shrink_600_2000/0/1614211759270?e=2147483647&v=beta&t=QVDhMaHAdHgI5dZgZGriPkPWRMn-ZFnFyegYJ9Rs_Ro">
</p>

_________________________________________________________________________________________________ 

### Dispositivos de rede
Os dispositivos de rede são separados de duas formas: ativos e passivos; Os ativos de rede são aqueles equipamentos que permitem a conexão entre dispositivos, são eles que geram o tráfego dos dados que estão na rede. 
Os passivos da rede são aqueles que somente transportam os dados, sem interferir nas informações trafegadas. Eles são responsáveis por conectar os equipamentos (Ex: RJ45, fonte de alimentação, patch panel, calhas)

Iremos dar ênfase nos ativos de rede, nas suas particularidades e comportamentos.

#### Hubs
Hubs são ativos de rede que interligam computadores, enviando um mesmo pacote para todos os receptores igualmente. Devido seu funcionamento, o Hub cria um grande domínio de colisão com os dispositivos conectados, sendo pouco utilizado atualmente, principalmente no meio empresarial.
<p align="center">
  <img width="350px" src="https://www.controle.net/novo/assets/img/faq/Hubs-faq-hubs-switches-e-roteadores-qual-e-a-diferenca-controlenet.webp">
</p>

#### Switch
São ativos de rede muito utilizados; são os responsáveis pela ligação dos computadores, suportando uma alta quantidade de dispositivos conectados. Switchs são equipamentos que possuem diversas portas e conseguem manter a altar performance da rede.
<p align="center">
  <img width="350px" src="https://www.arubanetworks.com/wp-content/uploads/glossary-network-switch-diagram_1200x650.jpeg">
</p>
