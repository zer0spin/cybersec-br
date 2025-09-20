# Trilha de Estudos: Red Team (Segurança Ofensiva)

Bem-vindo(a) à trilha de estudos do Red Team. O objetivo aqui é aprender a pensar e agir como um adversário para testar as defesas de uma organização de forma controlada e ética. Esta é a área dos Pentesters, Ethical Hackers e Operadores de Segurança Ofensiva.

Uma operação Red Team simula um ataque real e geralmente segue um ciclo de vida. Vamos estruturar nosso aprendizado em torno dessas fases.

---

## Fases de uma Operação Red Team

### Fase 1: Reconhecimento (Reconnaissance)

É a fase de coleta de informações. O objetivo é mapear a superfície de ataque do alvo, descobrindo tudo o que for publicamente acessível.

* **Objetivo:** Descobrir IPs, domínios, subdomínios, e-mails de funcionários, tecnologias usadas e possíveis pontos de entrada.
* **Conceitos Chave:** OSINT (Open Source Intelligence), Reconhecimento Ativo vs. Passivo, Footprinting, Google Dorking.
* **Ferramentas Essenciais:**
    * **Enumeração de Rede:** `Nmap`, `masscan`
    * **Enumeração de Subdomínios:** `subfinder`, `assetfinder`, `amass`
    * **Enumeração de Diretórios Web:** `dirsearch`, `gobuster`, `feroxbuster`
    * **Coleta de Informações (OSINT):** `theHarvester`, `Maltego`, Shodan
* **Recursos de Estudo:**
    * (PT-BR) **[Curso de Nmap - Bóson Treinamentos](https://www.youtube.com/playlist?list=PLucm8g_ezqNp0-Y-n_5l12Q_3gJ5_3kS4)**: Um guia completo da ferramenta mais essencial.
    * (EN) **[The Cyber Mentor - The Art of Recon](https://www.youtube.com/watch?v=p4JgI_4W-w0)**: Vídeo prático sobre o processo de reconhecimento.
    * (EN) **[OWASP Amass Project](https://github.com/owasp-amass/amass)**: Documentação de uma das ferramentas mais poderosas de recon.

### Fase 2: Acesso Inicial (Initial Access)

Com base nas informações coletadas, o objetivo agora é conseguir o primeiro "pé dentro" da rede ou sistema.

* **Objetivo:** Obter acesso a pelo menos uma máquina ou conta de usuário.
* **Conceitos Chave:** Phishing, Password Spraying, Exploração de Vulnerabilidades Públicas (CVEs), Engenharia Social.
* **Ferramentas Essenciais:**
    * **Framework de Exploração:** `Metasploit Framework`
    * **Busca de Exploits:** `searchsploit`
    * **Ataques de Senha:** `Hydra`, `Medusa`
    * **Simulação de Phishing:** `GoPhish`
* **Recursos de Estudo:**
    * (PT-BR) **[O que é o OWASP Top 10? - Diogo Guanabara](https://www.youtube.com/watch?v=Gk5y4zSgy2o)**: Entender as principais falhas de aplicações web é crucial.
    * (EN) **[HackTricks - Password Spraying](https://book.hacktricks.xyz/pentesting-web/password-spraying)**: Guia prático sobre a técnica.
    * (EN) **[Metasploit Unleashed](https://www.offensive-security.com/metasploit-unleashed/)**: O curso gratuito oficial do Metasploit.

### Fase 3: Execução e Persistência (Execution & Persistence)

Uma vez dentro, é preciso garantir que o acesso não seja perdido e executar comandos no sistema comprometido.

* **Objetivo:** Manter o acesso ao sistema mesmo após um reboot e estabelecer um canal de comando e controle (C2).
* **Conceitos Chave:** C2 Frameworks, Agendamento de Tarefas, Chaves de Registro (Windows), Serviços, Living Off The Land (LotL).
* **Ferramentas Essenciais:**
    * **C2 Frameworks (Pós-Exploração):** `Metasploit (Meterpreter)`, `Sliver`, `Havoc`. (Cobalt Strike é o padrão da indústria, mas é pago).
    * **Técnicas Nativas:** `cron` (Linux), `schtasks.exe` (Windows), `PowerShell`.
* **Recursos de Estudo:**
    * (EN) **[MITRE ATT&CK - Persistence Techniques](https://attack.mitre.org/tactics/TA0003/)**: A maior base de conhecimento sobre táticas de persistência.
    * (EN) **[IppSec no YouTube](https://www.youtube.com/c/ippsec)**: Assista a resoluções de máquinas do Hack The Box para ver técnicas de persistência na prática.

### Fase 4: Escalação de Privilégios (Privilege Escalation)

O acesso inicial geralmente é com um usuário de poucos privilégios. O objetivo é se tornar `root` (Linux) ou `NT AUTHORITY\SYSTEM` (Windows).

* **Objetivo:** Obter o maior nível de privilégio no sistema.
* **Conceitos Chave:** Exploração de Kernel, Senhas em Arquivos, Permissões Inseguras, Binários SUID (Linux), DLL Hijacking, SeImpersonatePrivilege (Windows).
* **Ferramentas Essenciais:**
    * **Scripts de Enumeração:** `LinPEAS` (Linux), `WinPEAS` (Windows)
    * **Bases de Conhecimento:** `GTFOBins` (para Linux), `LOLBAS` (para Windows)
    * **Frameworks de Pós-Exploração:** `PowerSploit`, `BloodHound` (para Active Directory).
* **Recursos de Estudo:**
    * (EN) **[HackTricks - Linux Privilege Escalation](https://book.hacktricks.xyz/linux-hardening/linux-privilege-escalation-checklist)**: Um checklist completo de técnicas.
    * (EN) **[HackTricks - Windows Privilege Escalation](https://book.hacktricks.xyz/windows-hardening/windows-local-privilege-escalation)**: Checklist para ambientes Windows.

### Fase 5: Movimentação Lateral e Domínio do Ambiente

Com privilégios máximos em uma máquina, o objetivo é se mover para outras máquinas na rede, buscando o controle total do ambiente (geralmente, o Domain Controller em redes corporativas).

* **Objetivo:** Comprometer outras máquinas, escalar privilégios no domínio e alcançar o objetivo final da operação.
* **Conceitos Chave:** Pass the Hash/Ticket, Kerberoasting, Pivoting, Exfiltração de Dados, Active Directory.
* **Ferramentas Essenciais:**
    * **Extração de Credenciais:** `Mimikatz`
    * **Kit de Ferramentas de Rede:** `Impacket Suite` (`psexec`, `smbclient`, etc.)
    * **Pivoting:** `Chisel`, `SSH`
* **Recursos de Estudo:**
    * (PT-BR) **[Ataques em Active Directory - Ricardo Longatto](https://www.youtube.com/playlist?list=PLy024vWc_w42bI9d-S-4C-0s-g2IA-M2a)**: Playlist com os principais ataques a AD.
    * (EN) **[The Cyber Mentor - Practical Ethical Hacking Course](https://www.youtube.com/watch?v=f_pEnnprt7w)**: Curso completo que aborda todas as fases.

---

### Certificações Recomendadas
* **Iniciante:** eLearnSecurity Junior Penetration Tester (eJPTv2)
* **Intermediário:** Offensive Security Certified Professional (OSCP), PNPT (Practical Network Penetration Tester)
* **Avançado:** OSEP, OSEE (Offensive Security), CRTE (Certified Red Team Expert)

### Como Praticar
* **Plataformas:** Hack The Box, TryHackMe, Proving Grounds, VulnHub.
* **Home Lab:** Crie seu próprio laboratório com Active Directory para simular um ambiente corporativo real.