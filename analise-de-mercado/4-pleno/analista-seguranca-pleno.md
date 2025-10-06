# Analista de Segurança da Informação Pleno

## 1. Informações Gerais
* **Nível:** Pleno
* **Modalidade:** Híbrido (Vitória/ES)
* **Tipo de Contrato:** Contrato Cooperado (PJ)
* **Nível de Inglês:** Não especificado, mas altamente recomendável (pelo menos leitura técnica).
* **Empresa (setor):** Empresa Confidencial de Tecnologia/Serviços.
* **Publicada em 19/09/2025**

## 2. "Traduzindo" as Responsabilidades

* **Responsabilidade:** Administrar, monitorar e otimizar soluções de WAF, garantindo proteção contra ataques em aplicações web.
    * **Tradução:** Você será responsável pela segurança das aplicações web (sites, sistemas). Sua função é configurar e ajustar o "muro" (WAF) que bloqueia ataques como SQL Injection e XSS, garantindo que só o tráfego legítimo passe.

* **Responsabilidade:** Gerenciar e operar soluções EDR, analisando incidentes e respondendo a ameaças.
    * **Tradução:** Você vai gerenciar o "antivírus com superpoderes" (EDR) instalado nos computadores da empresa. Seu trabalho é investigar os alertas que ele gera, entender se um ataque está acontecendo e responder para conter a ameaça.

* **Responsabilidade:** Administrar e aplicar segurança em Active Directory, com foco em Identity & Access Management (IAM), MFA e revisões de permissões.
    * **Tradução:** Você será responsável pelo "cartório" da empresa, o Active Directory, que diz quem é quem e o que cada um pode acessar. Sua missão é garantir que as permissões estejam corretas, que o acesso seja seguro (com MFA) e que ninguém tenha mais privilégios do que o necessário.

* **Responsabilidade:** Implementar políticas de identidade e acesso em ambientes híbridos (on-premises e cloud), alinhadas ao modelo Zero Trust.
    * **Tradução:** A empresa tem sistemas tanto no escritório (on-premises) quanto na nuvem. Você vai criar regras de acesso que funcionam nos dois lugares, seguindo a filosofia de "nunca confie, sempre verifique" (Zero Trust).

* **Responsabilidade:** Aplicar melhorias de segurança e compliance em Google Workspace, incluindo SSO e controles de acesso.
    * **Tradução:** Você vai "blindar" o ambiente do Google da empresa (Gmail, Drive, etc.), configurando regras de acesso, login único (SSO) e outras políticas para evitar vazamento de dados.

* **Responsabilidade:** Desenvolver automações para processos de segurança e gestão de identidade.
    * **Tradução:** Em vez de fazer tarefas repetitivas manualmente, você vai criar scripts para automatizá-las, como gerar relatórios de permissões ou bloquear um IP suspeito em vários lugares ao mesmo tempo.

* **Responsabilidade:** Apoiar iniciativas de privacidade de dados (LGPD), desde atendimento a titulares até elaboração de evidências para auditorias.
    * **Tradução:** Você vai ajudar a empresa a cumprir a lei de proteção de dados (LGPD), respondendo a solicitações de usuários sobre seus dados e coletando provas de que a empresa está fazendo tudo certo para auditorias.

* **Responsabilidade:** Monitorar, investigar e responder a incidentes de segurança, com recomendações técnicas e planos de ação.
    * **Tradução:** Quando um alarme de segurança disparar, você será um dos detetives que vai investigar o que aconteceu, entender o impacto e ajudar a criar um plano para consertar o problema e evitar que ele ocorra novamente.

## 3. Decifrando os Requisitos (Hard Skills)

#### Requisito: Experiência consolidada em segurança da informação (nível pleno).
* **O que é?** A empresa espera que você não seja um iniciante. Você já deve ter alguma experiência de trabalho na área, sabe usar as ferramentas e consegue resolver problemas com autonomia.
* **Por que pedem?** Para que você possa assumir as responsabilidades descritas sem precisar de treinamento intensivo do zero.
* **Como estudar?** A experiência vem com o tempo, mas pode ser acelerada com laboratórios práticos (home labs), projetos e contribuições que simulem desafios do mundo real.

#### Requisito: Conhecimento em soluções WAF de mercado.
* **O que é?** Um firewall específico para aplicações web que protege contra ataques da camada 7 (HTTP/S).
* **Por que pedem?** É a principal linha de defesa para qualquer serviço exposto na internet.
* **Como estudar?** Pratique com o WAF da Cloudflare (possui plano gratuito) para entender as regras. Estude o OWASP Top 10 para entender os ataques que um WAF mitiga.

#### Requisito: Vivência com EDR/XDR.
* **O que é?** Ferramentas de segurança para computadores e servidores (endpoints) que detectam e respondem a ameaças avançadas.
* **Por que pedem?** É a principal ferramenta para combater ransomware e malwares modernos.
* **Como estudar?** Use soluções open-source como Wazuh ou Elastic Security em um laboratório caseiro para simular detecções e alertas.

#### Requisito: Experiência em gestão de identidade e acessos em Active Directory (integração com nuvem).
* **O que é?** Gerenciar usuários e permissões no Active Directory (AD) da Microsoft e conectá-lo a serviços de nuvem como o Microsoft 365 ou Google Workspace.
* **Por que pedem?** Gerenciar quem tem acesso a quê é a base da segurança interna. Ambientes híbridos (local + nuvem) são a realidade da maioria das empresas.
* **Como estudar?** Crie um laboratório com Windows Server para praticar a administração de um AD. Estude os fundamentos do Microsoft Entra ID (antigo Azure AD) em uma conta de testes.

#### Requisito: Vivência em Google Workspace com foco em identidade digital.
* **O que é?** Saber configurar as opções de segurança e identidade do painel de administração do Google Workspace (SSO, 2FA, políticas de acesso).
* **Por que pedem?** A empresa usa o ecossistema Google, e a segurança dele é crucial.
* **Como estudar?** Leia a documentação oficial do Google Workspace Admin e assista a tutoriais sobre as configurações de segurança.

#### Requisito: Conhecimentos em automação (scripts, workflows ou integrações).
* **O que é?** Saber criar pequenos programas (scripts) para automatizar tarefas repetitivas.
* **Por que pedem?** Aumenta a eficiência do time de segurança e reduz o risco de erro humano. É um sinal de maturidade profissional.
* **Como estudar?** Aprenda o básico de Python ou PowerShell. Crie um script que automatize algo simples no seu laboratório, como verificar a data de expiração de certificados.

#### Requisito: Experiência prática com LGPD aplicada à segurança e privacidade.
* **O que é?** Entender como as ferramentas e processos de segurança (criptografia, controle de acesso, etc.) ajudam a empresa a cumprir a Lei Geral de Proteção de Dados.
* **Por que pedem?** A lei exige medidas técnicas de proteção de dados, e o time de segurança é o responsável por implementá-las.
* **Como estudar?** Foque nos artigos da LGPD que falam sobre medidas de segurança e o tratamento de dados. Estude o conceito de "Privacy by Design".

## 4. Analisando os Diferenciais

* **Diferencial:** Certificações em segurança ou identidade (ex.: CompTIA Security+, ISO 27001, LGPD/DPO).
    * **Por que é um diferencial?** Valida seu conhecimento de forma estruturada. Mostra dedicação e que você tem uma base teórica sólida, o que é um ótimo critério de desempate.

* **Diferencial:** Familiaridade com SIEM e resposta a incidentes.
    * **Por que é um diferencial?** Esta vaga é mais focada em proteção e identidade (IAM), mas saber SIEM mostra que você entende também da parte de detecção. Indica que você tem uma visão 360º da segurança, o que é muito valorizado.

## 5. Habilidades Comportamentais (Soft Skills)

* **Proatividade e visão crítica:** Um profissional pleno não só executa tarefas, mas questiona "por que fazemos assim?" e propõe melhorias para evitar problemas futuros.
* **Clareza de comunicação:** Essencial para explicar um risco técnico para um gestor que não é da área e para criar documentações claras.
* **Capacidade analítica e foco em melhoria contínua:** Habilidade de analisar um incidente, entender a causa raiz e criar um plano para que ele não aconteça de novo, em vez de apenas "apagar o incêndio".

## 6. Dicas e "Bandeiras Vermelhas" (Red Flags)

* **Dica sobre o Contrato (PJ/Cooperado):** Este é o ponto mais importante para se atentar. Um contrato PJ ou Cooperado significa que você não terá os benefícios de um CLT (13º, férias remuneradas, FGTS, etc.). Em contrapartida, o salário líquido (o que cai na sua conta) tende a ser maior.      
    * **Ação:** Ao negociar, sua proposta de salário deve ser de **30% a 50% maior** do que seria em um regime CLT para compensar os benefícios, impostos e a falta de segurança jurídica.

* **Dica sobre o Escopo ("Faz-Tudo"):** A vaga cobre muitas áreas diferentes (WAF, EDR, IAM, Cloud, LGPD, Automação). Isso é típico de um analista pleno em equipes enxutas.
    * **Ponto Positivo (Green Flag 🟩):** É uma oportunidade incrível de aprendizado! Você vai mexer com muitas tecnologias diferentes e ganhar uma experiência vasta em pouco tempo.
    * **Ponto de Atenção (Yellow Flag 🟨):** Pode indicar que a equipe de segurança é pequena e que você terá muitas responsabilidades. É importante perguntar na entrevista sobre o tamanho da equipe e a maturidade dos processos para evitar um cenário de sobrecarga.

* **Dica sobre "SIEM como Diferencial":** O fato de SIEM não ser um requisito obrigatório, mas um diferencial, pode indicar duas coisas: 
    1. A empresa ain                       da não tem uma solução de SIEM madura, e esta pode ser uma oportunidade para você ajudar a implementar.
    2. A responsabilidade principal pelo SIEM pode ser de outro analista. É um bom ponto para investigar na entrevista.

* **Ausência de Red Flags Clássicas (Green Flag 🟩):** A vaga é muito bem escrita e coerente. Ela descreve as responsabilidades de um Pleno de forma realista, não pede certificações impossíveis nem anos de experiência absurdos. Isso é um sinal de que o gestor da vaga sabe o que está procurando e a empresa tem uma boa maturidade em segurança.

## 7. Sugestão de Roteiro de Estudos

Para se preparar para uma vaga como esta, seu foco deveria ser:

1.  **Certificação(ões):** A **CompTIA Security+** para a base. Para um grande diferencial, a **Microsoft SC-300 (Identity and Access Administrator)** ou a **CompTIA CySA+**.
2.  **Conhecimento Prático:** Crie um **home lab** com Windows Server (Active Directory), uma máquina Linux e uma Windows. Integre seu lab com o **Wazuh** (EDR/SIEM). Pratique a criação de regras e a análise de alertas.
3.  **Projeto para Portfólio:** Desenvolva um script em **PowerShell** que gera um relatório de saúde do seu Active Directory (ex: usuários com senhas que nunca expiram, contas inativas há mais de 90 dias).
4.  **Conceitos Teóricos:** Aprofunde-se no modelo **Zero Trust**. Estude os principais ataques do **OWASP Top 10** e como um WAF os mitiga. Entenda os conceitos de autenticação moderna (OAuth, SAML, OpenID Connect).