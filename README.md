# resumo-do-lab
Este repositório contém o meu entendimento sobre a aula de computação em nuvem

## Computação em Nuvem - Resumo
  É um modelo de computação que consiste em abstrair o gerenciamento e virtualizar o acesso a operações e recursos associados ao servidor, tudo conectado via internet. A partir deste conceito, e em função das demandas de um mundo cada vez mais exigente quanto a velocidade, confiabilidade e portabilidade da informação, surgiram modelos de computação em nuvem que são: pública, privada e híbrida. Na primeira, o servidor possui acesso aberto a qualquer usuário; o segundo é mais restrito, limitando-se apenas ao órgão que gere o servidor, o qual infere em mais responsabilidades de ordem física e operacional do Data Center; o último acessa o melhor dos dois mundos, permitindo maior flexibilidade no uso dele.

## Benefícios da Nuvem - Resumo
  O benefícios inerentes a Computação em Nuvem são desenvolvidos tendo em vista a experiência do cliente, no que se refere a capacidade de fornecer soluções que atendam critérios como: 

  Escalabilidade: Capacidade de aumentar a capacidade dos recursos conforme a demanda prevista.
  
  Elasticidade: Cresce e diminui de capacidade conforme a demanda dinâmica por recursos.
  
  Governaça: Visa alinhar a estratégia de TI com os objetivos de negócios, gerenciar riscos, garantir conformidade com regulamentações e otimizar custos. 
  
  Gerenciabilidade: Capacidade de controlar, monitorar e otimizar recursos e serviços de nuvem, incluindo infraestrutura, aplicativos e dados, para garantir eficiência, segurança e controle de custos. A escalabilidade e a elasticidade são dois exemplos de gerenciabilidade .
  
  Confiabilidade: Refere-se ao quão resiliente e confiável é a sua solução em nuvem mediante quedas do servidor e sistema fora do ar.
  
  Previsibilidade: Capacidade de antecipar e controlar o comportamento de recursos, como custo, desempenho e uso, com base em dados históricos e tendências.
  
  Segurança: É o conjunto de políticas, controles, tecnologias e práticas de segurança que são usadas para proteger dados, aplicativos e infraestrutura em ambientes de nuvem.

  ## Tipos de Serviços da Nuvem - Resumo
  Quando se pensa em desenvolver uma solução por meio da nuvem, é possível escolher qual é o nível de responsabilidade que cada parte (cliente e provedor) terá, a fim de obter clareza na distribuição de direitos e deveres, assim evitando problemas de comunicação. Neste sentido, é importante entender os tipos de serviços de nuvem, que variam conforme aumentam ou diminuem o dever de cada um. São eles:
  
  IaaS: O cliente tem maior controle sobre a infraestrutura da aplicação. Assuntos como criação de instâncias, hosts e por aí vai são configurados por ele. Exemplo de IaaS é a AWS.
  
  PaaS: É um serviço cuja plataforma utilizada na criação de aplicações cuida da infraestrutura e permite realizar operações como deploy em algum ambiente, testes e hospedagem de páginas web. A Vercel é um ótimo exemplo de PaaS.
  
  SaaS: O serviço com menos responsabilidade para o clinte, pois ele só precisa autenticar e ser autorizado para então fazer uso do software disponibilizado gratuitamente. O Postman API e o GitHub representam o serviço de SaaS.

  ## Componentes de Arquitetura do Azure - Resumo
Existem diversos componentes de arquitetura de Azure da Microsoft que trabalham em conjunto para prover a solução em nuvem para nós, clientes. Por conta disso, eu me atentarei aos pares de regiões, grupos de recursos e assinatura. Para isso, gosto de usar uma analogia que também me ajudou a entender os conceitos vistos em aula.

Se compararmos o Azure como se ele fosse um parque de diversos, poderíamos dizer que os pares de regiões são como dois brinquedos gigantes em lados diferentes do parque, mas conectados por um trilho expresso. Se um brinquedo quebrar (problema em uma região), o outro entra em ação rapidinho (alta disponibilidade e recuperação de desastres).

 Agora, dentro do parque, suponha que eu tenha uma mochila mágica onde guardo todos os meus brinquedos: ingressos, mapas, etc. Essa mochila é o grupo de recursos — ela guarda todos os itens (máquinas virtuais, bancos de dados, etc.) que fazem parte da mesma aventura (ou projeto). Então é com ele que eu possuo acesso aos componentes de que cada região possui.
  
Quanto à assinatura do Azure, ele é como o meu passe de entrada no parque. Eu pago por ele e, com esse passe, posso usar os brinquedos, comer no restaurante e participar dos eventos (ou seja, usar e pagar pelos recursos do Azure). Cada assinatura tem limites e regras, como “esse passe permite usar até 5 brinquedos por vez”. Até aí pode-se dizer que é uma assinatura como qualquer outra.

Por fim, o grupo de gerenciamento é como um chefe de excursão com várias turmas, precisa organizar tudo. O grupo de gerenciamento é a prancheta do chefe, onde ele agrupa vários passes de entrada (assinaturas) e aplica regras para todas elas ao mesmo tempo — como horários, limites de gastos, segurança etc.

## Computação e Rede - Resumo

Serviços de Computação e Máquinas Virtuais do Azure

O Azure oferece uma variedade de serviços de computação que permitem a execução de aplicações e cargas de trabalho na nuvem. Um dos principais serviços é a Máquina Virtual (VM), que simula um computador físico e permite que o usuário execute sistemas operacionais e aplicativos como se estivesse em um ambiente local. As VMs do Azure são altamente configuráveis, permitindo a escolha de sistema operacional, tamanho, desempenho e localização geográfica. Elas são ideais para cenários que exigem controle total do sistema, como testes, desenvolvimento e hospedagem de aplicações empresariais.

Conjuntos de Disponibilidade de Máquinas Virtuais do Azure

Os Conjuntos de Disponibilidade (Availability Sets) são um recurso que melhora a alta disponibilidade das VMs. Ao distribuir as máquinas virtuais entre domínios de falha e domínios de atualização, o Azure reduz a probabilidade de que uma interrupção de hardware ou uma manutenção planejada afete todas as VMs simultaneamente. Dessa forma, mesmo que parte da infraestrutura sofra problemas, outras instâncias continuarão funcionando, garantindo a continuidade do serviço.

Área de Trabalho Virtual e Contêineres do Azure

A Área de Trabalho Virtual do Azure (Azure Virtual Desktop) é uma solução de virtualização que permite aos usuários acessarem um ambiente de desktop remoto, hospedado na nuvem. Essa funcionalidade é muito útil para empresas que desejam fornecer acesso seguro e centralizado a aplicativos e dados. Já os contêineres, como os do Azure Kubernetes Service (AKS), oferecem uma forma leve e eficiente de empacotar, distribuir e gerenciar aplicações em ambientes isolados. Os contêineres são mais rápidos para iniciar e consomem menos recursos que VMs tradicionais, sendo ideais para aplicações em nuvem escaláveis.

Azure Functions e Serviços de Aplicativo do Azure

O Azure Functions é um serviço de computação sem servidor (serverless) que executa trechos de código em resposta a eventos, sem a necessidade de gerenciar infraestrutura. Ele é ideal para tarefas automatizadas e processos de integração. Já o Serviço de Aplicativo (App Service) do Azure permite a criação e o gerenciamento de aplicativos web e APIs em diversas linguagens, como .NET, Java, Node.js e Python. Ele fornece escalabilidade automática, integração com DevOps e alta disponibilidade, facilitando o desenvolvimento e a hospedagem de aplicações modernas na nuvem.


