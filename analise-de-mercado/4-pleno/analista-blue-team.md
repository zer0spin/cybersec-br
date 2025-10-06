# Análise de Vaga: Analista de Segurança da Informação - Blue Team

## 1. Informações Gerais
* **Nível:** Não especificado, mas a profundidade dos requisitos ("experiência comprovada", "domínio", "conhecimento profundo") sugere um nível **Pleno**.
* **Modalidade:** Remoto
* **Tipo de Contrato:** Não especificado (provavelmente CLT).
* **Nível de Inglês:** Não especificado, mas altamente recomendável para estudo e leitura de documentação técnica.
* **Empresa (setor):** Empresa Confidencial do setor de Software/Tecnologia.
* **Publicada em:** 02/10/2025

## 2. "Traduzindo" as Responsabilidades

* **Responsabilidade:** Monitoramento e Detecção de Ameaças (...) correlacionando eventos para identificar atividades maliciosas em tempo real.
    * **Tradução:** Você será um detetive digital, olhando para os painéis de controle das ferramentas de segurança (Wazuh, Fortigate, Kaspersky). Seu trabalho é como montar um quebra-cabeça: um alerta de firewall aqui, um log estranho de um servidor ali. Você vai juntar as peças para enxergar um ataque em andamento.

* **Responsabilidade:** Resposta a Incidentes (...) executando ações de remediação, como isolamento de hosts e bloqueio de IPs.
    * **Tradução:** Quando um ataque é confirmado, você se torna a equipe de "pronto-socorro" cibernético. Seguindo um plano (playbook), sua missão é conter a ameaça o mais rápido possível. Isso significa, na prática, apertar o "botão vermelho" para isolar um computador infectado da rede ou bloquear o endereço de IP do atacante no firewall.

* **Responsabilidade:** Gerenciamento de Ferramentas de Segurança (...) realizando o tuning fino para maximizar a detecção e minimizar falsos positivos.
    * **Tradução:** Você será o "engenheiro" das ferramentas de defesa. Sua função é ajustar as configurações do Fortigate, Kaspersky e Wazuh para que eles se tornem mais inteligentes, pegando mais ameaças reais (maximizar detecção) e gerando menos alarmes falsos (minimizar falsos positivos) que desperdiçam o tempo da equipe.

* **Responsabilidade:** Garantia da Resiliência e Recuperação (...) validando a integridade e a segurança dos backups gerenciados pelo Veeam Backup.
    * **Tradução:** Você vai garantir que o "plano B" da empresa funcione. Em um cenário de desastre, como um ataque de ransomware que criptografa tudo, os backups são a única salvação. Você vai verificar se os backups estão sendo feitos corretamente e se estão seguros, para que a empresa possa se recuperar.

* **Responsabilidade:** Threat Hunting Proativo (...) caçar proativamente por Táticas, Técnicas e Procedimentos (TTPs) de adversários.
    * **Tradução:** Em vez de esperar o alarme soar, você vai ativamente "caçar" por sinais de invasores que podem estar escondidos na rede. Usando seu conhecimento sobre como os hackers operam (TTPs), você vai procurar por comportamentos sutis e anômalos que as ferramentas automáticas podem ter deixado passar.

* **Responsabilidade:** Análise de Vulnerabilidades (...) para priorizar a aplicação de patches.
    * **Tradução:** Você receberá uma lista de "portas abertas" (vulnerabilidades) nos sistemas da empresa. Sua tarefa é analisar essa lista e, usando os dados das outras ferramentas, determinar quais são as mais perigosas e que precisam ser corrigidas (patched) primeiro.

* **Responsabilidade:** Elaboração de Relatórios e Dashboards (...) para públicos técnicos e executivos.
    * **Tradução:** Você precisa traduzir a atividade de segurança, que é altamente técnica, em informações que todos possam entender. Isso significa criar relatórios detalhados sobre incidentes para sua equipe e, ao mesmo tempo, gráficos e métricas simples (MTTD/MTTR - Tempo Médio para Detectar/Responder) para que a diretoria saiba se os investimentos em segurança estão funcionando.

## 3. Decifrando os Requisitos (Hard Skills)

#### Requisito: Experiência comprovada em Segurança Defensiva, Blue Team, SOC ou Resposta a Incidentes.
* **O que é?** A empresa quer alguém que já tenha trabalhado na linha de frente da defesa cibernética, com experiência real em monitoramento e resposta a ataques.
* **Por que pedem?** O ritmo de um SOC é intenso e exige conhecimento prático. Não é uma posição para quem está começando do zero absoluto.
* **Como estudar?** Acelere sua experiência em laboratórios práticos (home labs) e plataformas como o TryHackMe e Hack The Box, que possuem salas e trilhas de estudo focadas em defesa (Blue Team).

#### Requisito: Experiência sólida na administração (...) utilizando Fortigate (NGFW) e Kaspersky EDRO.
* **O que é?** Conhecimento prático e aprofundado nas duas principais ferramentas de defesa da empresa: o firewall de próxima geração (NGFW) da Fortinet e a solução de detecção e resposta para endpoints (EDR) da Kaspersky.
* **Por que pedem?** São as ferramentas que você usará todos os dias. Você precisa saber não apenas interpretar seus alertas, mas também configurá-las e otimizá-las.
* **Como estudar?**
    * **Fortinet:** Estude para a certificação **NSE 4**. A Fortinet oferece muito material de estudo gratuito. Você pode usar firewalls open-source como pfSense ou OPNsense em seu lab para praticar os conceitos.
    * **Kaspersky EDRO:** Estude o conceito de EDR a fundo. Use soluções como o Wazuh ou a versão gratuita do Elastic Security em seu lab para entender como um EDR funciona na prática.

#### Requisito: Domínio de metodologias de defesa e frameworks, como o MITRE ATT&CK e a Cyber Kill Chain.
* **O que é?** São "enciclopédias" que mapeiam e categorizam as táticas e técnicas usadas por cibercriminosos. Não são ferramentas, mas sim modelos mentais para guiar a defesa.
* **Por que pedem?** Mostra que você entende *como* os adversários pensam e operam, permitindo que você crie defesas mais eficazes e realize threat hunting de forma estruturada.
* **Como estudar?** Navegue pelo site do MITRE ATT&CK. Escolha uma técnica (ex: T1059.001 - PowerShell) e pesquise como detectá-la. Use a ferramenta Atomic Red Team para simular essa técnica em seu lab e tente detectá-la com o Wazuh.

#### Requisito: Profundo conhecimento em sistemas operacionais Windows e Linux (análise de logs, hardening, forense).
* **O que é?** Você precisa ser um especialista nos sistemas que está protegendo. Isso significa saber onde os logs importantes ficam, como "blindar" um sistema (hardening) e como encontrar evidências de uma invasão (princípios de forense).
* **Por que pedem?** Um invasor age dentro do sistema operacional. Se você não conhecer o terreno melhor que ele, não conseguirá encontrá-lo.
* **Como estudar?** Crie máquinas virtuais Windows e Linux em seu lab. Aprenda a usar o Sysmon no Windows e o auditd no Linux para monitoramento detalhado. Pratique analisando os logs de eventos nativos.

#### Requisito: Experiência prática com ferramentas de segurança defensiva (SIEM: Wazuh, Análise de Rede: Wireshark, Backup: Veeam).
* **O que é?** Conhecimento em ferramentas que complementam o stack principal. Wazuh para centralizar e analisar logs (SIEM), Wireshark para "farejar" o tráfego da rede e Veeam para a estratégia de recuperação.
* **Por que pedem?** Mostra que você tem uma visão ampla da defesa, desde o endpoint até a recuperação de desastres.
* **Como estudar?** Todas essas ferramentas podem ser utilizadas gratuitamente em um laboratório. Instale o Wazuh, use o Wireshark para capturar o tráfego do seu próprio lab e baixe a edição comunitária do Veeam para simular rotinas de backup.

## 4. Analisando os Diferenciais
* **Diferencial:** Certificações (Fortinet NSE 4+, CySA+, GCIH).
    * **Por que é um diferencial?** Valida formalmente suas habilidades práticas. A NSE 4 mostra que você domina a ferramenta principal deles. A CySA+ valida sua capacidade analítica como um todo. A GCIH é uma das certificações de resposta a incidentes mais respeitadas do mundo.

* **Diferencial:** Habilidade em programação/scripting (Python ou PowerShell).
    * **Por que é um diferencial?** É um multiplicador de força. Permite que você automatize tarefas repetitivas, analise grandes volumes de logs de forma programática e crie suas próprias ferramentas de defesa. Mostra um nível de maturidade profissional muito alto.

* **Diferencial:** Experiência com segurança em ambientes de nuvem (AWS, Azure, GCP).
    * **Por que é um diferencial?** As empresas estão na nuvem. Saber como aplicar os mesmos princípios de defesa (monitoramento, resposta a incidentes, etc.) em ambientes AWS, Azure ou GCP é uma habilidade extremamente valiosa e mostra que você está preparado para o futuro.

* **Diferencial:** Conhecimento em técnicas de evasão de defesas.
    * **Por que é um diferencial?** Para se defender bem, você precisa entender como os atacantes tentam ser invisíveis. Saber como eles podem ofuscar um malware ou bypassar um firewall permite que você crie regras de detecção mais inteligentes e resilientes.

## 5. Habilidades Comportamentais (Soft Skills)
* **Mentalidade Defensiva e Proativa:** O desejo constante de proteger e a iniciativa de caçar ameaças em vez de apenas esperar por alertas.
* **Raciocínio Analítico e Resolução de Problemas:** Essencial para conectar eventos aparentemente não relacionados durante uma investigação.
* **Atenção aos Detalhes:** Fundamental para encontrar o "fio da meada" em meio a milhões de logs.
* **Comunicação Clara (Escrita e Verbal):** Crucial para documentar incidentes e apresentar relatórios para diferentes públicos.
* **Resiliência e Controle Emocional:** Responder a um incidente de segurança é uma atividade de alta pressão. Manter a calma e seguir o plano é fundamental.

## 6. Dicas e "Bandeiras Vermelhas" (Red Flags)

* **Dica sobre a Transparência (Green Flag 🟩):** A vaga é um excelente exemplo de transparência. Ela detalha exatamente o stack de tecnologia (Fortinet, Kaspersky, Wazuh, Veeam) e as metodologias (MITRE ATT&CK) utilizadas. Isso é ouro para um candidato, pois permite um estudo totalmente direcionado.
* **Dica sobre a Maturidade (Green Flag 🟩):** A descrição da vaga é extremamente bem escrita e utiliza terminologia padrão da indústria (TTPs, MTTD/MTTR, Blue Team). Isso indica uma equipe de segurança com alta maturidade, onde você provavelmente aprenderá muito com processos bem definidos.
* **Dica sobre o Nível de Exigência (Yellow Flag 🟨):** A lista de requisitos e diferenciais é longa e profunda, cobrindo múltiplas especialidades (redes, endpoint, SIEM, backup, nuvem, scripting). É uma vaga exigente, definitivamente não é para iniciantes. É importante ser honesto sobre seu nível de experiência para não gerar frustração.
* **Dica sobre o "Especialista Generalista":** O escopo da vaga abrange muitas áreas. Pode ser uma oportunidade incrível de aprendizado, mas também pode indicar uma equipe enxuta onde cada analista acumula muitas responsabilidades. É um bom ponto para perguntar na entrevista sobre o tamanho da equipe e a divisão de tarefas.

## 7. Sugestão de Roteiro de Estudos
1.  **Certificação(ões):** A **CompTIA CySA+** é a certificação que melhor reflete as responsabilidades desta vaga. Dado o foco da empresa, a **Fortinet NSE 4** se torna quase obrigatória para se destacar. Como um objetivo de longo prazo, a **GCIH** da SANS/GIAC é o padrão-ouro.
2.  **Conhecimento Prático (Home Lab):** Para esta vaga, ter um laboratório não é opcional, é essencial.
    * **Core:** Instale o **Wazuh** como seu SIEM.
    * **Endpoints:** Crie VMs Windows (com Sysmon) e Linux, e instale os agentes do Wazuh nelas.
    * **Rede:** Use o **pfSense** ou **OPNsense** para atuar como seu firewall, praticando a criação de regras e análise de logs de rede.
    * **Simulação de Ataques:** Use o framework **Atomic Red Team** para executar TTPs do MITRE ATT&CK em suas VMs e pratique a detecção e investigação dos alertas gerados no Wazuh.
3.  **Projeto para Portfólio:** Documente todo o seu home lab no GitHub. Escolha 3 TTPs do MITRE ATT&CK, simule-os em seu lab, e crie um relatório de "Resposta a Incidentes" para cada um, detalhando: (1) O Alerta Inicial, (2) Os Passos da Investigação, (3) As Ações de Contenção/Remediação, e (4) as Lições Aprendidas/Melhorias nas Regras de Detecção.
4.  **Conceitos Teóricos:** Faça um mergulho profundo no framework **MITRE ATT&CK Enterprise**. Não apenas leia, mas entenda as relações entre Táticas e Técnicas. Revise os fundamentos de redes TCP/IP e estude a fundo o funcionamento de protocolos como DNS, HTTP/S e SMB.