# Analista de Segurança da Informação - MDR

## 1. Informações Gerais
* **Nível:** Não especificado, mas inferido como **Pleno** devido à exigência de "experiência comprovada" e à natureza das responsabilidades.
* **Modalidade:** Presencial (Fortaleza/CE)
* **Tipo de Contrato:** Não especificado, mas a lista robusta de benefícios (assistência médica, VA, seguro de vida, etc.) sugere fortemente um contrato **CLT**.
* **Nível de Inglês:** Técnico (para leitura de documentação).
* **Empresa (setor):** Empresa Confidencial de Serviços de Segurança Gerenciada (MSSP).
* **Vaga Inclusiva:** Aberta para Pessoas com Deficiência (PCDs).
* **Publicada em 19/09/2025**

## 2. "Traduzindo" as Responsabilidades

* **Responsabilidade:** Monitorar eventos e alertas no SIEM (IBM QRadar) e demais ferramentas correlacionadas.
    * **Tradução:** Você será o "vigia da torre de controle". Seu dia a dia será ficar de olho no painel principal de segurança (o SIEM), que agrega logs de toda a empresa, procurando por qualquer sinal de atividade suspeita ou maliciosa.

* **Responsabilidade:** Realizar análise de logs, correlação de eventos e investigação de incidentes de segurança.
    * **Tradução:** Quando um alarme soar, você será o detetive. Sua missão é mergulhar nos registros (logs), conectar os pontos entre diferentes eventos para entender a história completa de um possível ataque e determinar se é um alarme falso ou uma ameaça real.

* **Responsabilidade:** Atuar em resposta a incidentes (contenção, mitigação e recuperação).
    * **Tradução:** Se a ameaça for real, você entra em ação. Seu trabalho será seguir os procedimentos para isolar o problema (contenção), remover a ameaça (mitigação) e ajudar a restaurar os sistemas ao normal (recuperação).

* **Responsabilidade:** Elaborar reports semanais e mensais para clientes e gestão interna.
    * **Tradução:** Você precisará documentar suas descobertas e atividades. Isso significa criar relatórios claros que mostrem o que foi detectado, o que foi feito e qual o estado da segurança, tanto para a equipe técnica quanto para os gestores e clientes.

* **Responsabilidade:** Apoiar na criação de regras de correlação, casos de uso e ajustes finos no SIEM.
    * **Tradução:** Além de usar o SIEM, você vai ajudá-lo a ficar mais inteligente. Com base em novas ameaças ou no ambiente da empresa, você vai criar novas "regras de alarme" para que a ferramenta possa detectar ataques mais sofisticados automaticamente.

* **Responsabilidade:** Interagir com equipes internas (SOC, NOC, Endpoint, etc.) e clientes, garantindo comunicação clara e objetiva.
    * **Tradução:** Você não trabalha sozinho. Será preciso conversar constantemente com outras equipes de tecnologia para investigar e resolver incidentes, além de se comunicar com os clientes para explicar os riscos e as ações tomadas.

* **Responsabilidade:** Apoiar auditorias e conformidade com normas como ISO 27001, NIST e LGPD.
    * **Tradução:** Você ajudará a provar que a empresa está seguindo as regras e leis de segurança. Isso envolve coletar evidências (logs, relatórios de configuração) que demonstrem que os controles de segurança estão funcionando como deveriam.

## 3. Decifrando os Requisitos (Hard Skills)

#### Requisito: Experiência comprovada com SIEM (preferencialmente QRadar, mas conhecimento em outros será valorizado).
* **O que é?** SIEM (Security Information and Event Management) é o cérebro de um Centro de Operações de Segurança (SOC). É uma plataforma que coleta e analisa logs de segurança de toda a rede.
* **Por que pedem?** É a principal ferramenta de trabalho da vaga. Toda a função de detecção e análise gira em torno dela.
* **Como estudar?** Crie um laboratório em casa (home lab) com ferramentas open-source como **Wazuh** ou **Elastic SIEM**. Pratique a ingestão de logs de diferentes fontes (Windows, Linux) e a criação de regras de detecção. Existem plataformas como a **LetsDefend** que simulam um ambiente de SOC para você praticar.

#### Requisito: Conhecimentos em MDR, análise de logs, redes e protocolos de segurança.
* **O que é?** MDR (Managed Detection and Response) é o serviço que está sendo oferecido. Análise de logs é a habilidade de "ler" os registros de sistemas. Conhecer redes (TCP/IP, DNS, HTTP) é fundamental para entender como os ataques se movem.
* **Por que pedem?** É a base teórica para o trabalho. Sem entender como a comunicação funciona (redes) e como os sistemas registram eventos (logs), é impossível investigar um incidente.
* **Como estudar?** Para redes, o conteúdo da certificação **CompTIA Network+** é o padrão-ouro. Para análise de logs, pratique em seu home lab, tentando identificar atividades suspeitas nos logs do Windows (Event Viewer) e do Linux (`/var/log`).

#### Requisito: Experiência com resposta a incidentes de segurança e investigação forense básica.
* **O que é?** Saber o que fazer quando um ataque é confirmado, seguindo um plano para conter e erradicar a ameaça. Forense básica envolve saber coletar e preservar evidências digitais.
* **Por que pedem?** A função não é apenas detectar, mas também responder. A empresa precisa de alguém que saiba agir sob pressão para minimizar os danos de um ataque.
* **Como estudar?** Estude o ciclo de vida de resposta a incidentes (ex: **PICERL** - Preparation, Identification, Containment, Eradication, Recovery, Lessons Learned). Use plataformas de treino como **Blue Team Labs Online (BTLO)** para praticar em cenários realistas.

#### Requisito: Conhecimento em ferramentas de segurança como EDR, antivírus corporativo, DLP, firewall, etc.
* **O que é?** São as fontes de dados do SIEM. EDR (Endpoint Detection and Response) monitora notebooks e servidores; DLP (Data Loss Prevention) previne vazamento de dados; Firewall controla o tráfego de rede.
* **Por que pedem?** Para analisar um alerta do SIEM, você precisa entender o que a ferramenta que o gerou (como o EDR) está "dizendo".
* **Como estudar?** Em seu home lab, instale e configure um EDR open-source (como o próprio Wazuh ou o Elastic Agent) para entender que tipo de telemetria ele coleta.

#### Requisito: Entendimento de frameworks como MITRE ATT&CK.
* **O que é?** É um "mapa" de táticas e técnicas usadas por cibercriminosos. Ele padroniza a forma como falamos sobre ataques.
* **Por que pedem?** É a linguagem universal para detecção e resposta. Ajuda a criar regras de detecção mais eficazes ("estou criando uma regra para detectar a técnica T1059.001") e a entender o comportamento do invasor.
* **Como estudar?** Navegue pelo site oficial do MITRE ATT&CK. Escolha uma técnica (ex: "Credential Dumping") e pesquise como ela funciona e como pode ser detectada.

## 4. Analisando os Diferenciais

* **Diferencial:** Certificações como CompTIA Security+, CySA+, IBM QRadar, NSE, ou equivalentes.
    * **Por que é um diferencial?** Certificações validam seu conhecimento de forma rápida para o recrutador. A **CySA+** é especialmente relevante, pois é focada em análise de segurança. Uma certificação no próprio **QRadar** te colocaria muito à frente.

* **Diferencial:** Experiência com automação de processos de segurança (SOAR, Python, n8n).
    * **Por que é um diferencial?** Mostra que você é um profissional que busca eficiência. Automatizar tarefas repetitivas (como bloquear um IP malicioso no firewall) libera tempo para análises mais complexas. Isso é um sinal de maturidade profissional e proatividade.

* **Diferencial:** Vivência em ambientes com alta criticidade (financeiro, governo, indústria, etc.).
    * **Por que é um diferencial?** Estes ambientes não toleram erros e exigem processos rigorosos. Ter essa experiência indica que você é um profissional disciplinado, resiliente e que sabe trabalhar sob pressão.

## 5. Habilidades Comportamentais (Soft Skills)

* **Raciocínio analítico e detalhista:** Essencial para não deixar passar pistas importantes durante uma investigação.
* **Boa comunicação escrita e verbal:** Fundamental para escrever relatórios claros e para explicar situações técnicas complexas para clientes e outras equipes.
* **Proatividade e busca constante por melhorias:** O analista ideal não só resolve o problema, mas pensa em como evitar que ele aconteça novamente.

## 6. Dicas e "Bandeiras Vermelhas" (Red Flags)

* **Dica sobre o Escopo (Foco em Blue Team):** Esta é uma vaga "pura" de analista de SOC/MDR. O foco é 100% em defesa, detecção e resposta.
    * **Ponto Positivo (Green Flag 🟩):** É uma oportunidade fantástica para quem quer se especializar e se tornar um expert em Blue Team. Você vai viver e respirar a análise de incidentes, ganhando uma profundidade técnica imensa nessa área.

* **Dica sobre o Ambiente (MSSP):** A vaga menciona "clientes", o que indica que a empresa é um Provedor de Serviços de Segurança Gerenciada (MSSP).
    * **Ponto Positivo (Green Flag 🟩):** Você terá contato com diferentes tecnologias e realidades de múltiplos clientes. O aprendizado é extremamente acelerado.
    * **Ponto de Atenção (Yellow Flag 🟨):** O ritmo em um MSSP pode ser intenso e a pressão, alta. É um ambiente dinâmico que exige grande capacidade de organização. Pergunte na entrevista sobre a quantidade de clientes por analista e como é a escala de plantão.

* **Dica sobre a Maturidade (Green Flag 🟩):** A descrição da vaga é excelente. Ela cita frameworks padrão de mercado (MITRE, NIST, ISO 27001), ferramentas específicas (QRadar) e responsabilidades bem definidas. Isso mostra que a empresa tem um processo de segurança maduro e sabe exatamente o profissional que está procurando.

## 7. Sugestão de Roteiro de Estudos

Para se preparar para uma vaga como esta, seu foco deveria ser:

1.  **Certificação(ões):** A **CompTIA CySA+** é o alvo perfeito, pois cobre todo o escopo da vaga. A **Security+** é a base, caso ainda não a tenha. Se quiser ir além, busque materiais de estudo da certificação de Analista do **IBM QRadar**.
2.  **Conhecimento Prático:** Monte um **home lab** com **Wazuh** ou **Security Onion**. Use máquinas virtuais para simular ataques (ex: com a suite Metasploitable) e pratique a detecção e investigação dos alertas gerados no seu SIEM.
3.  **Projeto para Portfólio:** Documente uma de suas investigações no home lab em um post de blog ou em seu GitHub. Descreva o cenário, mostre os logs relevantes, explique como você conectou os pontos usando o framework **MITRE ATT&CK** e qual seria o plano de resposta.
4.  **Conceitos Teóricos:** Aprofunde-se no **MITRE ATT&CK**, escolhendo 5 técnicas comuns (ex: T1059.001 - PowerShell, T1078 - Valid Accounts) e estudando suas formas de detecção. Estude o ciclo de vida da Resposta a Incidentes do **NIST (SP 800-61)**.