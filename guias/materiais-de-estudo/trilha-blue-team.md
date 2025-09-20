# Trilha de Estudos: Blue Team (Segurança Defensiva)

Bem-vindo(a) à trilha de estudos do Blue Team. O objetivo aqui é aprender a proteger os ativos digitais de uma organização, detectar atividades maliciosas e responder a incidentes de segurança. Esta é a área dos Analistas de SOC, Respondedores de Incidentes, Threat Hunters e Engenheiros de Segurança.

A defesa cibernética é um processo contínuo. Vamos estruturar nosso aprendizado em torno dos pilares do **NIST Cybersecurity Framework**, um dos modelos mais respeitados do mundo.

---

## Pilares da Defesa Cibernética

### Pilar 1: Identificar (Identify)

Você não pode proteger o que não sabe que existe. Esta fase é sobre entender o ambiente, os ativos e os riscos.

* **Objetivo:** Ter um inventário completo de todos os ativos (hardware, software, dados) e avaliar os riscos associados a eles.
* **Conceitos Chave:** Gestão de Ativos, Análise de Riscos, Governança, Políticas de Segurança.
* **Ferramentas Essenciais:** Ferramentas de inventário de rede, Scanners de Vulnerabilidades (`Nessus`, `OpenVAS`), Planilhas e frameworks de gestão de risco.
* **Recursos de Estudo:**
    * (PT-BR) **[O que é a ISO 27001? - TI Sem Segredos](https://www.youtube.com/watch?v=FcsYpWpQ-o0)**: Entender frameworks de gestão é um bom começo.
    * (EN) **[NIST Cybersecurity Framework - Site Oficial](https://www.nist.gov/cyberframework)**: Leia a documentação do framework que estrutura este guia.

### Pilar 2: Proteger (Protect)

Esta é a fase de implementação de controles para reduzir a superfície de ataque e impedir que incidentes ocorram.

* **Objetivo:** Implementar defesas para garantir a segurança da infraestrutura e dos dados.
* **Conceitos Chave:** Hardening de Sistemas, Gestão de Identidade e Acesso (IAM), Firewalls, IPS/IDS, Antivírus/EDR, Criptografia, Backups.
* **Ferramentas Essenciais:**
    * **Diretório:** `Active Directory` (para gestão de identidade)
    * **Firewall:** `pfSense` (open-source), firewalls de cloud (AWS Security Groups, Azure NSG)
    * **Configuração Segura:** `CIS Benchmarks`
* **Recursos de Estudo:**
    * (PT-BR) **[Segurança em Active Directory - Bóson Treinamentos](https://www.youtube.com/watch?v=T_APo4bu2i8)**: Entender como proteger o coração da rede corporativa.
    * (EN) **[CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks/)**: Guias detalhados e gratuitos para "blindar" praticamente qualquer sistema ou software.

### Pilar 3: Detectar (Detect)

Mesmo com as melhores proteções, incidentes podem ocorrer. Esta fase é sobre encontrar atividades suspeitas o mais rápido possível.

* **Objetivo:** Monitorar o ambiente para identificar anomalias e potenciais incidentes de segurança.
* **Conceitos Chave:** Análise de Logs, SIEM (Security Information and Event Management), Threat Intelligence, Threat Hunting, MITRE ATT&CK Framework.
* **Ferramentas Essenciais:**
    * **SIEM/EDR:** `Wazuh`, `Elastic Security` (open-source), `Splunk` (padrão de mercado).
    * **Análise de Rede (NIDS):** `Suricata`, `Zeek (Bro)`
    * **Análise de Pacotes:** `Wireshark`
* **Recursos de Estudo:**
    * (PT-BR) **[O que é SIEM? - Cássio Batistin](https://www.youtube.com/watch?v=3W1_NlkpC70)**: Uma ótima explicação do conceito.
    * (EN) **[LetsDefend.io](https://letsdefend.io/)**: Plataforma prática para treinar como analista de SOC, analisando alertas reais.
    * (EN) **[MITRE ATT&CK Framework](https://attack.mitre.org/)**: A "bíblia" das táticas e técnicas de ataque. Um Blue Teamer deve conhecê-la tão bem quanto um Red Teamer.

### Pilar 4: Responder (Respond)

Quando um incidente é detectado, é hora de agir para contê-lo e erradicá-lo.

* **Objetivo:** Conter o impacto de um incidente, erradicar a ameaça e notificar as partes interessadas.
* **Conceitos Chave:** Ciclo de Vida de Resposta a Incidentes (PICERL), Forense Digital, Análise de Malware, Análise de Memória.
* **Ferramentas Essenciais:**
    * **Kit de Ferramentas Forenses:** `The Sleuth Kit`, `Autopsy`
    * **Análise de Memória:** `Volatility Framework`
    * **Análise de Malware:** Ambientes de sandbox (`Cuckoo`), depuradores (`x64dbg`).
* **Recursos de Estudo:**
    * (EN) **[The DFIR Report](https://thedfirreport.com/)**: Análises detalhadas de incidentes reais, do acesso inicial à exfiltração. Leitura obrigatória.
    * (EN) **[SANS Digital Forensics and Incident Response Poster](https://www.sans.org/posters/dfir-find-evil/)**: Um "pôster" que resume os principais processos e locais para encontrar evidências.

---

### Certificações Recomendadas
* **Iniciante:** CompTIA Security+, CompTIA CySA+
* **Intermediário:** Blue Team Level 1 (BTL1), Certified Incident Handler (GCIH da SANS)
* **Avançado:** Certified Information Systems Security Professional (CISSP) - focado em gestão.

### Como Praticar
* **Plataformas:** Blue Team Labs Online (BTLO), LetsDefend.io, CyberDefenders.
* **Home Lab:** Crie seu próprio SIEM com Wazuh e Elastic, integre com Suricata e envie logs de máquinas Windows e Linux para simular um ambiente de monitoramento.