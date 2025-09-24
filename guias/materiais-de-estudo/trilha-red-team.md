# Trilha de Estudos: Red Team (Segurança Ofensiva)

Bem-vindo(a) à trilha de estudos do Red Team. O objetivo aqui é aprender a pensar e agir como um atacante para testar as defesas de uma organização de forma controlada e ética. Esta é a área dos Pentesters, Ethical Hackers e Operadores de Segurança Ofensiva.

Uma operação Red Team simula um ataque real e geralmente segue um ciclo de vida. Vamos estruturar nosso aprendizado em torno dessas fases.

### Fundamentos e Mentalidade (Mindset)

Antes de mergulhar nas ferramentas, é crucial entender a filosofia por trás do Red Team.

  * **(PT-BR) [O que é equipe vermelha?](https://www.ibm.com/br-pt/think/topics/red-teaming)**: Red Team na visão da IBM.
  * **(PT-BR) [Pensar como o Inimigo: A Arte do Red Team - IDSC](https://www.youtube.com/live/ks1gprSmcug)**: Live que aborda a mentalidade e a arte do Red Teaming.
   * **(EN) [Responsible Red Teaming - Taggart Institute](https://taggartinstitute.org/p/responsible-red-teaming)**: Seminário sobre as considerações éticas, legais e táticas de operações Red Team.
  * **(EN) [Transitioning From OffSec to Red Teaming](https://medium.com/@ty.anderson.3/transitioning-from-offsec-to-red-teaming-165fc2e968f8)**: Um pequeno texto com várias indicações de livros para refletir sobre a "mentalidade do Red Team".

## Fases de uma Operação Red Team

### Fase 1: Reconhecimento (Reconnaissance)

É a fase de coleta de informações. O objetivo é mapear a superfície de ataque do alvo, descobrindo tudo o que for publicamente acessível.

  * **Objetivo:** Descobrir IPs, domínios, subdomínios, e-mails de funcionários, tecnologias usadas e possíveis pontos de entrada.
  * **Conceitos Chave:** OSINT (Open Source Intelligence), Reconhecimento Ativo vs. Passivo, Footprinting, Google Dorking.
  * **Ferramentas Essenciais:**
      * **Enumeração de Rede:** `Nmap`, `masscan`
      * **Enumeração de Subdomínios:** `subfinder`, `assetfinder`, `amass`
      * **Enumeração de Diretórios Web:** `dirsearch`, `gobuster`, `feroxbuster`
      * **Coleta de Informações (OSINT):** `theHarvester`, `Maltego`, `Shodan`, `web-check`
  * **Recursos de Estudo:**
      * Não tem um curso exatamente, mas pesquise pelo "Fernando Mercês", um dos idealizadores da ONG "Mentebinária". Ele é uma das maiores referências no Brasil sobre o assunto.
      * **(PT-BR) [Guia de OSINT do Bob Reis](https://github.com/bob-reis/OSINT)**: Uma coleção curada de recursos de OSINT.
      * **(EN) [Oh Shint\! It's a Blog](https://ohshint.gitbook.io/oh-shint-its-a-blog/)**: Blog com técnicas e write-ups de OSINT.
      * **(EN) [Awesome OSINT](https://github.com/jivoi/awesome-osint)**: Uma lista gigantesca e bem categorizada de ferramentas de OSINT.
      * **(EN) [The OSINT Framework](https://osintframework.com/)**: Framework interativo para encontrar ferramentas de OSINT.

### Fase 2: Acesso Inicial (Initial Access)

Com base nas informações coletadas, o objetivo agora é conseguir o primeiro acesso à rede ou sistema.

  * **Objetivo:** Obter acesso a pelo menos uma máquina ou conta de usuário.
  * **Conceitos Chave:** Phishing, Password Spraying, Exploração de Vulnerabilidades Públicas (CVEs), Engenharia Social.
  * **Ferramentas Essenciais:**
      * **Framework de Exploração:** `Metasploit Framework`
      * **Busca de Exploits:** `searchsploit`
      * **Ataques de Senha:** `Hydra`, `Medusa`, `SafeSpray` (BR, criada pelo Bob Reis)
      * **Simulação de Phishing:** `GoPhish`, `Evilginx2`
  * **Recursos de Estudo:**
      * **(EN) [HackTricks - Phishing Methodology](https://book.hacktricks.wiki/en/generic-methodologies-and-resources/phishing-methodology/index.html)**: Guia prático sobre Phishing (e vários outros tópicos relacionados à Fase 2).
      * **(EN) [Metasploit Unleashed](https://www.offensive-security.com/metasploit-unleashed/)**: O curso gratuito oficial do Metasploit, essencial para dominar o framework.

### Fase 3: Execução e Persistência (Execution & Persistence)

Uma vez dentro, é preciso garantir que o acesso não seja perdido e executar comandos no sistema comprometido.

  * **Objetivo:** Manter o acesso ao sistema mesmo após um reboot e estabelecer um canal de comando e controle (C2).
  * **Conceitos Chave:** C2 Frameworks, Agendamento de Tarefas, Chaves de Registro (Windows), Serviços, Living Off The Land (LotL).
  * **Ferramentas Essenciais:**
      * **C2 Frameworks (Pós-Exploração):** `Metasploit (Meterpreter)`, `Sliver`, `Havoc`. (Cobalt Strike e Brute Ratel são os padrões da indústria, mas são pagos).
      * **Técnicas Nativas:** `cron` (Linux), `schtasks.exe` (Windows), `PowerShell`.
  * **Recursos de Estudo:**
      * **(EN) [The C2 Matrix](https://www.thec2matrix.com/)**: Uma matriz comparativa de dezenas de frameworks de C2.
      * **(EN) [MITRE ATT\&CK - Persistence Techniques](https://attack.mitre.org/tactics/TA0003/)**: A maior base de conhecimento sobre táticas de persistência.
      * **(EN) [IppSec no YouTube](https://www.youtube.com/c/ippsec)**: Assista a resoluções de máquinas do Hack The Box para ver técnicas de persistência na prática.

### Fase 4: Escalação de Privilégios (Privilege Escalation)

O acesso inicial geralmente é com um usuário de poucos privilégios. O objetivo é se tornar `root` (Linux) ou `NT AUTHORITY\SYSTEM` (Windows).

  * **Objetivo:** Obter o maior nível de privilégio no sistema.
  * **Conceitos Chave:** Exploração de Kernel, Senhas em Arquivos, Permissões Inseguras, Binários SUID (Linux), DLL Hijacking, SeImpersonatePrivilege (Windows).
  * **Ferramentas Essenciais:**
      * **Scripts de Enumeração:** `LinPEAS` (Linux), `WinPEAS` (Windows)
      * **Bases de Conhecimento:** `GTFOBins` (para Linux), `LOLBAS` (para Windows)
  * **Recursos de Estudo:**
      * **(EN) [HackTricks - Linux Privilege Escalation](https://book.hacktricks.wiki/en/linux-hardening/linux-privilege-escalation-checklist.html)**: Um checklist completo de técnicas.
      * **(EN) [HackTricks - Windows Privilege Escalation](https://book.hacktricks.wiki/en/windows-hardening/windows-local-privilege-escalation/index.html)**: Checklist para ambientes Windows.

### Fase 5: Movimentação Lateral e Domínio do Ambiente (Foco em Active Directory)

Com privilégios máximos em uma máquina, o objetivo é se mover para outras máquinas na rede, buscando o controle total do ambiente (geralmente, o Domain Controller em redes corporativas).

  * **Objetivo:** Comprometer outras máquinas, escalar privilégios no domínio e alcançar o objetivo final da operação.
  * **Conceitos Chave:** Pass the Hash/Ticket, Kerberoasting, Pivoting, Exfiltração de Dados, Golden/Silver Ticket.
  * **Ferramentas Essenciais:**
      * **Extração de Credenciais:** `Mimikatz`
      * **Kit de Ferramentas de Rede:** `Impacket Suite` (`psexec`, `smbclient`, `secretsdump`, etc.)
      * **Análise de AD:** `BloodHound`
      * **Pivoting:** `Chisel`, `SSH`
  * **Recursos de Estudo:**
      * **(EN) [The Hacker Recipes - Active Directory](https://www.thehacker.recipes/ad/escalation/)**: Um "cookbook" online e direto ao ponto com comandos e técnicas para AD.    

### Fase 6: Red Teaming em Ambientes de Nuvem (Cloud)

As táticas se adaptam quando o alvo está em infraestrutura de nuvem (AWS, Azure, GCP).

  * **Objetivo:** Explorar configurações incorretas na nuvem, roubar chaves de acesso e mover-se lateralmente entre serviços.
  * **Conceitos Chave:** IAM Roles, Metadados de Instância, Serverless Exploitation, Storage Buckets Públicos.
  * **Ferramentas Essenciais:**
      * **AWS:** `Pacu`, `Cloudsplaining`
      * **Azure:** `MicroBurst`, `PowerZure`
      * **GCP:** `GCPBucketBrute`
  * **Recursos de Estudo:**
      * Existem pouquíssimos conteúdos gratuitos nessa área, então iremos atualizar aqui conforme surgirem e eventualmente com os cursos pagos mais relevantes.
      * **(EN) [Pacu - The AWS Exploitation Framework](https://github.com/RhinoSecurityLabs/pacu)**: Documentação da principal ferramenta para pentest em AWS.

### Cursos Gratuitos Abrangentes

  * **(PT-BR) [Desec Security](https://desecsecurity.com/)**: Oferece cursos gratuitos de base e uma plataforma de laboratórios (a parte paga inclui mais conteúdo e labs).
  * **(EN) [Learn Penetration Testing - TCM Security](https://academy.tcm-sec.com/p/learn-penetration-testing-free)**: Mais de 27 horas de material gratuito de alta qualidade no YouTube.
  * **(EN) [Hacker101](https://www.hackerone.com/hackers/hacker101)**: Conteúdo gratuito da HackerOne, focado em Bug Bounty mas com conceitos fundamentais para segurança ofensiva.

### Certificações Recomendadas

  * **Iniciante:** eJPTv2 (eLearnSecurity Junior Penetration Tester), PNPT (Practical Network Penetration Tester)
  * **Intermediário:** OSCP (Offensive Security Certified Professional), CRTO (Certified Red Team Operator)
  * **Avançado:** OSEP (Offensive Security Experienced Penetration Tester), OSEE (Offensive Security Exploitation Expert), CRTE (Certified Red Team Expert)

### Como Praticar

  * **Plataformas:** Hack The Box, TryHackMe, Proving Grounds, VulnHub.
  * **Home Lab:** Crie seu próprio laboratório com Active Directory para simular um ambiente corporativo real. Isso é essencial para treinar ataques a AD. E crie laboratórios para todos os tipos de ataques possíveis, será seu momento de maior aprendizado.