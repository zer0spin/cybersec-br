# Análise de Vaga: Analista de NOC - Júnior (com Foco em Migração para Cibersegurança)

## 1. Informações Gerais
* **Nível:** Júnior
* **Modalidade:** Híbrido/Remoto com uma condição especial: os 3 primeiros meses são 100% presenciais na sede da empresa (Cláudio/MG), com ajuda de custo. Após esse período, a vaga se torna 100% remota.
* **Tipo de Contrato:** "Contrato". **Este é um ponto de atenção:** É crucial esclarecer com o recrutador se é um contrato **CLT** (com benefícios) ou **PJ** (Pessoa Jurídica).
* **Nível de Inglês:** Não especificado.
* **Empresa (setor):** Empresa Confidencial de Soluções em Telecomunicações.

## 2. "Traduzindo" as Responsabilidades (com um Olhar de Cibersegurança)

* **Responsabilidade:** Gerenciar as redes dos clientes e analisar o tráfego de dados (...) para evitar eventos que gerem lentidão, instabilidades e quedas.
    * **Tradução:** Você será o "controlador de tráfego" da internet dos clientes. Seu trabalho é monitorar constantemente o fluxo de dados para garantir que tudo esteja funcionando bem, com o objetivo principal de manter os serviços online e com bom desempenho (disponibilidade).
    * **Ponte para Cibersegurança:** Esta é a habilidade mais importante que você vai aprender. Para identificar um tráfego **malicioso**, você primeiro precisa ser um expert em identificar o tráfego **normal**. Analisar o tráfego de dados para fins de performance é o primeiro passo para aprender a analisá-lo em busca de anomalias de segurança.

* **Responsabilidade:** Realizar configurações, de baixa complexidade, de roteadores, switches, antenas e servidores.
    * **Tradução:** Você colocará a "mão na massa" para fazer ajustes básicos em equipamentos de rede e servidores, seguindo os procedimentos da empresa.
    * **Ponte para Cibersegurança:** Conhecer como os equipamentos de rede são configurados é fundamental para entender como eles podem ser atacados (devido a uma configuração incorreta) e como devem ser protegidos (processo de *hardening*).

* **Responsabilidade:** Prestar atendimento e suporte técnico ao cliente.
    * **Tradução:** Quando um cliente tiver um problema de conexão, você será a pessoa que ele irá contatar para investigar e resolver a questão.
    * **Ponte para Cibersegurança:** Muitas vezes, um "problema de lentidão" reportado por um cliente pode ser o primeiro sintoma de um ataque de segurança (como um DDoS). Você aprenderá a fazer as perguntas certas e a investigar a fundo, desenvolvendo o raciocínio analítico necessário para a triagem de incidentes de segurança.

* **Responsabilidade:** Manter documentação técnica precisa e atualizada.
    * **Tradução:** Você precisará registrar as configurações, alterações e soluções de problemas em uma base de conhecimento.
    * **Ponte para Cibersegurança:** A documentação meticulosa é uma exigência em cibersegurança, seja para registrar as etapas de uma investigação forense ou para manter as políticas de segurança da empresa atualizadas.

## 3. Decifrando os Requisitos (e Como Usá-los para Migrar)

#### Requisito: Familiaridade com ferramentas de teste e medição (MTR, Ping, tracert, SpeedTest, nslookup, entre outras).
* **O que é?** São as ferramentas básicas de qualquer profissional de redes para diagnosticar problemas de conectividade.
* **Por que pedem?** São o "kit de primeiros socorros" que você usará todos os dias para entender por que uma conexão está lenta ou não funciona.
* **Como usar para Cibersegurança?** Um analista de segurança usa exatamente as mesmas ferramentas na fase inicial de uma investigação. Um alerta de segurança em um servidor? O primeiro passo é usar `ping` e `tracert` para verificar se há um problema de rede ou se o servidor está realmente offline, talvez por um ataque de negação de serviço.

#### Requisito: Familiaridade, com ferramentas de monitoramento de redes (Zabbix, Grafana ou similares).
* **O que é?** São plataformas que coletam dados da rede e os exibem em painéis e gráficos, permitindo que o analista veja a "saúde" da rede em tempo real.
* **Por que pedem?** É a principal ferramenta que você usará para monitorar o tráfego e identificar problemas de performance.
* **Como usar para Cibersegurança?** A lógica de monitoramento de um NOC é 90% similar à de um SOC. Aprender a ler gráficos no Grafana, criar alertas no Zabbix e identificar anomalias de performance é o treinamento perfeito para depois trabalhar com um **SIEM** (como Splunk, QRadar ou Wazuh), que monitora eventos de segurança.

## 4. Analisando os Diferenciais
* A vaga não lista diferenciais, mas para uma posição de NOC Jr. com aspirações em segurança, certificações como **CompTIA Network+** ou **Cisco CCNA** e conhecimentos básicos em **Linux** e **scripting (Python)** seriam enormes vantagens.

## 5. Habilidades Comportamentais (Soft Skills)
* **Resolução de Problemas:** A essência do trabalho de NOC.
* **Atenção aos Detalhes:** Essencial para identificar pequenas anomalias nos gráficos de monitoramento que podem indicar um problema maior.
* **Comunicação Clara:** Fundamental para explicar problemas técnicos complexos para clientes que não são da área de TI.
* **Trabalho sob Pressão:** Quando a rede de um cliente importante cai, a pressão para resolver o problema rapidamente é alta.

## 6. Dicas e "Bandeiras Vermelhas" (Red Flags)

* **Oportunidade (Green Flag 🟩) - A Melhor Escola para o Blue Team:** Não há como enfatizar isso o suficiente: a experiência em um NOC é a melhor preparação possível para quem sonha em trabalhar em um SOC (Security Operations Center). Os conceitos de monitoramento, tráfego, protocolos e topologia de rede são diretamente transferíveis.

* **Ponto de Atenção Crítico (Red Flag 🟥) - A Condição de Realocação:** A exigência de trabalhar presencialmente em Cláudio/MG nos primeiros 3 meses é um obstáculo significativo para a maioria dos candidatos do Brasil. Você precisa avaliar com muito cuidado se a "ajuda de custo" oferecida cobre os seus gastos com aluguel temporário, alimentação e transporte. Para muitos, este pode ser um fator eliminatório.

* **Ponto de Atenção (Yellow Flag 🟨) - Ambiguidade do "Contrato":** É fundamental que você pergunte na primeira conversa com o RH se a vaga é CLT ou PJ. Se for PJ, você não terá benefícios como 13º salário, férias remuneradas e FGTS. Nesse caso, seu salário bruto precisa ser de 30% a 50% maior para compensar os custos e impostos que você terá como empresa.

* **Dica sobre o Foco: Disponibilidade vs. Segurança:** Lembre-se que seu objetivo principal no NOC será garantir a **disponibilidade** e a **performance** da rede. A segurança é uma preocupação secundária. A transição para uma mentalidade de segurança dependerá do seu esforço em estudar e aplicar esse conhecimento extra no seu dia a dia.

## 7. Sugestão de Roteiro de Estudos (Para Migração de NOC para SOC)

1.  **Fase 1: Domine o Terreno de Redes (Primeiros 6 meses)**
    * **Objetivo:** Se tornar um excelente Analista de NOC. Domine as ferramentas (Zabbix, Grafana) e os comandos de diagnóstico.
    * **Estudo Paralelo:** Estude para a certificação **CompTIA Network+**. Ela vai organizar e aprofundar todo o conhecimento prático que você ganhará no trabalho. Entenda a fundo a suíte de protocolos TCP/IP.

2.  **Fase 2: Construa a Ponte para a Segurança (6 a 12 meses)**
    * **Objetivo:** Começar a pensar e agir com uma mentalidade de segurança.
    * **Ações no Trabalho:** Ao analisar um pico de tráfego, pergunte-se: "Isso é um uso legítimo ou pode ser um ataque de negação de serviço (DDoS)?". Ao configurar um switch, pesquise sobre as melhores práticas de *hardening* para aquele equipamento.
    * **Estudo Paralelo:** Mergulhe na **CompTIA Security+**. Essa é a certificação que conecta o mundo das redes com o da segurança. Comece a estudar sobre firewalls, IDS/IPS e VPNs.

3.  **Fase 3: A Travessia para o SOC (12 a 24 meses)**
    * **Objetivo:** Se preparar para uma vaga de Analista de SOC Júnior.
    * **Estudo Paralelo:** Foque na certificação **CompTIA CySA+ (Cybersecurity Analyst)**. Construa um **home lab** com um SIEM open-source, como o **Wazuh** ou a versão gratuita do **Elastic Security**. Aprenda a coletar logs de diferentes fontes e a criar regras de detecção.
    * **Projeto para Portfólio:** Baixe arquivos de captura de pacotes (.pcap) de ataques simulados (disponíveis em sites como o Malware-Traffic-Analysis.net). Use o **Wireshark** para analisar o tráfego e escreva um relatório detalhado da sua investigação, explicando passo a passo como você identificou a atividade maliciosa. Este projeto demonstra, de forma prática, a habilidade mais importante de um analista de SOC, utilizando o conhecimento de redes que você solidificou no NOC.