# Guia de Programação para Cibersegurança

Saber programar é o que transforma um profissional de segurança de um mero "usuário de ferramentas" em um criador de soluções. A habilidade de criar seus próprios scripts para automatizar tarefas, analisar dados ou até mesmo desenvolver exploits customizados é um divisor de águas na sua carreira, seja no ataque ou na defesa.

Este guia apresenta as linguagens de programação mais relevantes para a área, explicando por que são importantes e fornecendo recursos para o seu aprendizado.

## 1. Python

Python é a linguagem mais popular e versátil em cibersegurança, sendo considerada o "canivete suíço" do profissional da área. Sua sintaxe simples e a vasta coleção de bibliotecas a tornam ideal para automação rápida e desenvolvimento de ferramentas.

#### Aplicações para Red Team (Ataque)
* **Desenvolvimento de Ferramentas:** Criar scanners, scripts de enumeração e automatizar a exploração de vulnerabilidades.
* **Criação de Exploits:** Desenvolver provas de conceito (PoCs) para vulnerabilidades.
* **Web Scraping:** Coletar informações de alvos de forma automatizada (OSINT).

#### Aplicações para Blue Team (Defesa)
* **Automação de Análise de Logs:** Criar scripts para ler, filtrar e identificar padrões suspeitos em logs.
* **Análise de Malware:** Desempacotar e analisar o comportamento de artefatos maliciosos.
* **Integração de Ferramentas (API):** Conectar diferentes soluções de segurança (SIEM, EDR, etc.).

#### Recursos Recomendados
* **Livros:**
    * (EN) *Black Hat Python* (Justin Seitz): Um clássico para aplicações ofensivas.
    * (EN) *Violent Python* (TJ O'Connor): Focado em scripts de ataque e forense.
    * (PT-BR) *Introdução à Programação com Python* (Nilo Ney Coutinho Menezes): Excelente livro para quem está começando do zero em português.
* **Cursos:**
    * (PT-BR) **[Curso de Python - Gustavo Guanabara](https://www.youtube.com/playlist?list=PLHz_AreHm4dlKP6QQCekuIPky1CiwmdI6)**: Uma das melhores introduções à lógica e à linguagem.
    * (PT-BR) **[Python para Segurança da Informação na Solyd Offensive Security](https://solyd.com.br/treinamentos)**: Curso pago e muito focado na prática.
    * (EN) **[Python for Everybody (FreeCodeCamp)](https://www.freecodecamp.org/learn/scientific-computing-with-python/)**: Curso universitário completo e gratuito.

## 2. Bash/Shell Scripting

Bash é a linguagem do terminal Linux. Dominá-la é fundamental, pois a maioria das ferramentas de segurança e servidores do mundo rodam em ambientes baseados em Unix/Linux.

#### Aplicações para Red Team
* **Automação de Reconhecimento:** Encadeamento de ferramentas como `nmap`, `gobuster`, e `jq`.
* **Criação de Payloads:** Escrever one-liners para obter acesso a um sistema (shells reversas).

#### Aplicações para Blue Team
* **Análise de Logs na Linha de Comando:** Uso de `grep`, `awk`, `sed`, `cut` para investigar logs.
* **Automação de Tarefas de Administração:** Scripts para backups, verificações de segurança, etc.

#### Recursos Recomendados
* **Livros:**
    * (EN) *The Linux Command Line* (William Shotts): A "bíblia" para aprender a linha de comando.
* **Cursos e Canais:**
    * (PT-BR) **[Curso de Shell Script - Bóson Treinamentos](https://www.youtube.com/playlist?list=PLucm8g_ezqNrYgj4gS_I2Wc0t_wStw_dG)**: Um curso muito completo e didático.
    * (PT-BR) **[Canal Diolinux](https://www.youtube.com/c/Diolinux)**: Conteúdo geral sobre Linux que ajuda a aprimorar as habilidades no terminal.
    * (EN) **[Linux Journey](https://linuxjourney.com/)**: Plataforma interativa e gratuita.

## 3. PowerShell

PowerShell é para o Windows o que o Bash é para o Linux: um framework de automação e linha de comando extremamente poderoso. É essencial para administrar, atacar e defender ambientes corporativos.

#### Aplicações para Red Team
* **Living Off The Land (LotL):** Uso do PowerShell nativo para executar atividades maliciosas sem malwares externos.
* **Ataques em Active Directory:** Automatizar a enumeração de usuários e políticas com frameworks como PowerSploit.

#### Aplicações para Blue Team
* **Administração e Hardening:** Automatizar a aplicação de políticas de segurança em máquinas Windows.
* **Threat Hunting:** Criar scripts para procurar por sinais de comprometimento (IoCs).

#### Recursos Recomendados
* **Livros:**
    * (EN) *Learn PowerShell in a Month of Lunches* (Don Jones): Um dos livros mais recomendados para iniciantes.
* **Cursos e Canais:**
    * (PT-BR) **[Curso de PowerShell - Wellyngton Galvão](https://www.youtube.com/playlist?list=PL-f7S1d_hANdSWs9xIacq-2S1f-IE22A_)**: Um bom ponto de partida em português.
    * (EN) Documentação oficial da Microsoft e canais no YouTube de especialistas como John Savill.

## 4. C/C++

C e C++ são linguagens de baixo nível, o que significa que oferecem um controle muito granular sobre a memória e os recursos do sistema. São a base sobre a qual muitos sistemas operacionais e ferramentas de segurança foram construídos.

* **Por que são importantes?** Entender C/C++ é fundamental para a análise de malware, engenharia reversa e desenvolvimento de exploits, pois permite compreender como os programas interagem diretamente com a memória.

#### Aplicações para Red Team
* **Desenvolvimento de Exploits:** Essencial para criar exploits de buffer overflow e outras vulnerabilidades de corrupção de memória.
* **Desenvolvimento de Shellcode:** Escrever o código de baixo nível que é executado após uma vulnerabilidade ser explorada.
* **Criação de Malwares:** Desenvolver rootkits, keyloggers e outros malwares performáticos e difíceis de detectar.

#### Aplicações para Blue Team
* **Engenharia Reversa e Análise de Malware:** Entender o código desmontado (Assembly) de um malware requer uma base sólida em C/C++.
* **Análise de Vulnerabilidades:** Auditar o código-fonte de aplicações escritas nessas linguagens em busca de falhas de segurança.

#### Recursos Recomendados
* **Livros:**
    * (PT-BR) *C - Completo e Total* (Herbert Schildt): Um clássico para aprender a linguagem C.
    * (EN) *Hacking: The Art of Exploitation* (Jon Erickson): O melhor livro para entender a exploração de software, com exemplos práticos em C e Assembly.
* **Cursos:**
    * (PT-BR) **[Curso de Linguagem C - Pietro Martins](https://www.youtube.com/playlist?list=PLesCEcYj003SwVdufCQM5FIbrOd0GG1M4)**: Curso universitário gratuito e de alta qualidade.

## 5. Perl

Perl é uma linguagem mais antiga, mas que ainda tem um lugar especial no coração de muitos profissionais de segurança, especialmente administradores de sistemas e Red Teamers "old school".

* **Por que é importante?** Perl é extremamente poderosa para manipulação de texto e processamento de expressões regulares (regex), o que a torna excelente para análise rápida de logs e extração de informações. Muitas ferramentas e exploits clássicos foram escritos em Perl.

#### Aplicações para Red Team
* **Scripts Rápidos:** Ótima para criar scripts de automação "sujos e rápidos" durante um pentest.
* **Processamento de Texto:** Extrair e-mails, senhas ou outras informações de grandes arquivos de texto.
* **Exploits Clássicos:** Muitos exploits para aplicações web mais antigas disponíveis no Exploit-DB são escritos em Perl.

#### Aplicações para Blue Team
* **Análise de Logs:** Criar scripts complexos com regex para encontrar padrões específicos em logs de servidores web, firewalls, etc.

#### Recursos Recomendados
* **Livros:**
    * (EN) *Learning Perl* (Randal L. Schwartz): Também conhecido como "O Livro do Lhama", é a referência para iniciantes.
* **Tutoriais:**
    * Tutoriais em sites como o [Perl Maven](https://perlmaven.com/) e a documentação oficial ([perldoc.perl.org](https://perldoc.perl.org/)).

## 6. Go (Golang)

Go é uma linguagem moderna criada pelo Google, que está ganhando imensa popularidade em cibersegurança devido à sua performance e simplicidade. Muitas das ferramentas de linha de comando mais rápidas e eficientes que você usa hoje são escritas em Go (ex: Nuclei, Subfinder, Katana).

  * **Por que é importante?** Go compila para um **único binário estático**, o que significa que o programa roda em qualquer sistema (Windows, Linux, Mac) sem precisar de dependências ou bibliotecas externas. É extremamente rápido, ótimo para tarefas concorrentes (fazer várias coisas ao mesmo tempo, como escanear múltiplos alvos) e mais difícil de ser analisado por engenharia reversa, tornando-o um favorito para desenvolvimento de malwares modernos.

#### Aplicações para Red Team (Ataque)

  * **Desenvolvimento de Malwares e C2:** Muitos malwares e frameworks de C2 (Command and Control) modernos são escritos em Go por ser de difícil detecção (anti-forense) e multi-plataforma.
  * **Ferramentas de Rede de Alta Performance:** Ideal para criar scanners de rede, enumeradores de subdomínios e fuzzers que precisam ser muito rápidos.
  * **Automação de API:** Interagir de forma eficiente com APIs de serviços em nuvem e outras ferramentas.

#### Aplicações para Blue Team (Defesa)

  * **Desenvolvimento de Agentes de Segurança:** Criar agentes leves e performáticos para monitorar endpoints ou redes sem consumir muitos recursos.
  * **Processamento de Dados em Alta Velocidade:** Ferramentas para analisar grandes volumes de tráfego de rede ou logs de forma rápida e concorrente.
  * **Análise de Malware em Go:** Saber a linguagem ajuda a fazer a engenharia reversa de malwares escritos nela.

#### Recursos Recomendados

  * **Livros:**
      * (EN) *Black Hat Go* (Tom Steele, Chris Patten, Dan Kottmann): O livro essencial, focado em criar ferramentas de segurança ofensiva com Go.
      * (EN) *The Go Programming Language* (Alan Donovan, Brian Kernighan): Considerado a "bíblia" da linguagem Go, excelente para construir uma base sólida.
      * (EN) *Go for Cybersecurity* (Cyril Anderson, Jose Maldonado): Outro livro excelente com exemplos práticos e atuais.
  * **Cursos e Canais:**
      * (PT-BR) **[Aprenda Go](https://www.youtube.com/c/aprendago)**: Um dos melhores e mais completos canais em português para aprender Go do zero.
      * (PT-BR) **[Curso de Go (Golang) - Full Cycle](https://www.google.com/search?q=https://www.youtube.com/playlist%3Flist%3DPL5-wUj1I46ngh_GvAfa3kALqA5b505aJG)**: Playlist muito boa para quem está começando.
      * (EN) **[A Tour of Go](https://go.dev/tour/welcome/1)**: O tour interativo oficial para aprender a sintaxe.

## 7. JavaScript

JavaScript é a linguagem da web. Se algo acontece no seu navegador, é quase certo que há JavaScript envolvido. Para quem atua com segurança de aplicações web (AppSec), tanto no ataque quanto na defesa, entender JavaScript não é opcional, é obrigatório.

  * **Por que é importante?** Todo navegador executa JavaScript. Conhecê-la permite entender e explorar vulnerabilidades do lado do cliente, como Cross-Site Scripting (XSS), Cross-Site Request Forgery (CSRF), e ataques a APIs. Além disso, com Node.js, você pode usar JavaScript para criar ferramentas de automação do lado do servidor.

#### Aplicações para Red Team (Ataque)

  * **Exploração de XSS:** Criar payloads para roubar cookies de sessão, interceptar digitação (keylogging), fazer capturas de tela do navegador da vítima ou redirecionar usuários.
  * **Engenharia Social:** Desenvolver páginas de phishing interativas e convincentes que simulam o comportamento de sites legítimos.
  * **Automação de Navegador:** Usar frameworks como Puppeteer ou Selenium para automatizar ações em aplicações web complexas durante um pentest (ex: preencher formulários, testar senhas, etc.).
  * **Bypass de Defesas do Lado do Cliente:** Entender como a lógica de segurança implementada no navegador pode ser contornada.

#### Aplicações para Blue Team (Defesa)

  * **Análise de Código-Fonte (SAST):** Revisar o código JavaScript de uma aplicação em busca de falhas de segurança e más práticas.
  * **Detecção de XSS e Magecart:** Analisar ataques que injetam JavaScript malicioso em sites (especialmente e-commerce) para roubar dados de cartão de crédito e informações pessoais.
  * **Análise de Scripts Maliciosos:** Entender o que um script ofuscado encontrado em um site comprometido está fazendo.

#### Recursos Recomendados

  * **Livros:**
      * (EN) *Eloquent JavaScript* (Marijn Haverbeke): Um dos melhores livros sobre a linguagem, disponível gratuitamente online.
      * (EN) *Bug Bounty Bootcamp* (Vickie Li): Embora não seja um livro só sobre JS, ele mostra na prática como JavaScript é usado para encontrar bugs reais em programas de bug bounty.
  * **Cursos e Plataformas:**
      * (PT-BR) **[Curso de JavaScript - Gustavo Guanabara](https://www.youtube.com/playlist?list=PLHz_AreHm4dlsK3Nr9GVvXCbpQyHQl1o1)**: Curso completo e excelente para aprender a base da linguagem do zero.
      * (PT-BR) **[Rocketseat](https://www.rocketseat.com.br/)**: Embora focado em desenvolvimento, seus materiais gratuitos são ótimos para aprender JS moderno.
      * (EN) **[PortSwigger Web Security Academy](https://portswigger.net/web-security)**: A melhor plataforma do mundo para aprender e praticar a exploração de vulnerabilidades web. Quase todos os laboratórios envolvem entender ou manipular JavaScript.

### Contribua com este Guia!

Este guia é um documento vivo e sempre pode ser melhorado. Se você conhece um ótimo livro, curso ou canal, especialmente em português, que não está listado aqui, **não hesite em contribuir!**

Leia nosso **[Guia de Contribuição](../../CONTRIBUINDO.md)** e envie um Pull Request para ajudar a próxima geração de profissionais de cibersegurança.


