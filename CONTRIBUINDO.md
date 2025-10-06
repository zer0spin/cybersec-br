# Como Contribuir para a Comunidade Brasileira de Cibersegurança

Este repositório é um esforço coletivo para criar uma base de conhecimento rica e acessível para todos os interessados em cibersegurança no Brasil. Toda contribuição, não importa o tamanho, é valorizada.

## Tipos de Contribuição

* 📄 **Adicionar seu Perfil:** Apresente-se à comunidade para fazer possíveis amizades e expandir seu networking.
* 💡 **Compartilhar um Projeto:** Quem não é visto, não é lembrado, né? Então mostre seus melhores projetos.
* 📈 **Criar uma Análise de Mercado:** Ajude a "dissecar" uma vaga e transformá-la em um guia de estudos para iniciantes.
* 🔗 **Sugerir um Link ou Ferramenta:** Encontrou um recurso incrível? Não guarde para ti, honre o nome "comunidade"!
* ✍️ **Escrever ou Melhorar um Guia:** Compartilhe seu conhecimento de mercado.
* 🐛 **Corrigir Erros:** Encontrou um link quebrado ou um erro de digitação? Nos ajude a corrigir.

---
## Guia Rápido para Contribuir (O Processo Geral)

Se você não está familiarizado com o Git e o GitHub, não se preocupe! O processo geral é sempre o mesmo.

### Passo 1: Faça um "Fork" do Repositório

Clique no botão **"Fork"** no canto superior direito da página do repositório `zer0spin/cybersec-br`. Isso criará uma cópia exata do nosso projeto na sua própria conta do GitHub.

### Passo 2: Clone o Seu Fork

No seu repositório "forkado" (que estará em `https://github.com/SEU-USUARIO/cybersec-br`), clique no botão verde **"< > Code"** e copie a URL. Agora, no seu computador, abra um terminal e execute o seguinte comando:

```bash
git clone [https://github.com/SEU-USUARIO/cybersec-br.git](https://github.com/SEU-USUARIO/cybersec-br.git)
````

*Lembre-se de substituir `SEU-USUARIO` pelo seu nome de usuário do GitHub.*

### Passo 3: Crie uma "Branch"

É uma boa prática criar uma "branch" (ramificação) para cada nova contribuição. Isso mantém seu trabalho organizado e isolado.

```bash
cd cybersec-br
git checkout -b minha-contribuicao-incrivel
```

*Dê um nome descritivo para sua branch (ex: `feat/adiciona-perfil-zer0spin`, `fix/corrige-faq-gramatica`).*

### Passo 4: Faça Suas Alterações

Adicione ou edite os arquivos localmente no seu editor de código preferido, seguindo as instruções específicas para o seu tipo de contribuição (veja na próxima seção).

### Passo 5: Salve Suas Alterações (Commit)

Após fazer as alterações, salve-as com um "commit", que é como um ponto de salvamento no histórico do projeto.

```bash
# Adiciona todos os arquivos modificados para serem salvos
git add .

# Cria o "commit" com uma mensagem descritiva
git commit -m "feat: Adiciona perfil de Fulano de Tal"
```

*Use uma mensagem de commit clara. Boas práticas sugerem o uso de prefixos como `feat:` (nova funcionalidade), `fix:` (correção de bug), `docs:` (mudanças na documentação).*

### Passo 6: Envie as Alterações para o Seu Fork

Envie as alterações da sua máquina para o seu repositório forkado no GitHub.

```bash
git push origin minha-contribuicao-incrivel
```

### Passo 7: Abra um "Pull Request"

Volte para a página do seu fork no GitHub (`https://github.com/SEU-USUARIO/cybersec-br`). Você verá uma mensagem destacada sugerindo a criação de um **"Pull Request" (PR)**. Clique no botão "Compare & pull request".

Preencha o PR com um título claro e uma breve descrição do que você fez. Depois, clique em **"Create Pull Request"**.

Pronto\! Agora, um dos mantenedores do projeto irá revisar sua contribuição e, se estiver tudo certo, irá integrá-la ao repositório principal.

-----

## Instruções Específicas por Tipo de Contribuição

Aqui detalhamos o que fazer no **Passo 4** para os principais tipos de contribuição.

### Como Adicionar Seu Perfil

Para manter nosso índice organizado, pedimos que você edite **dois arquivos**.

  * **Passo 4.1: Crie seu arquivo de perfil**

    1.  Vá para a pasta `/comunidade/membros/`.
    2.  Copie o conteúdo do nosso **[TEMPLATE.md](./comunidade/membros/TEMPLATE.md)**.
    3.  Crie um novo arquivo chamado `seu-usuario.md` (use seu usuário do GitHub).
    4.  Cole o conteúdo e preencha com suas informações.

  * **Passo 4.2: Adicione-se ao índice de membros**

    1.  Abra o arquivo **[README.md](./comunidade/membros/README.md)** da pasta de membros.
    2.  Copie uma linha da tabela e cole no local correto para manter a **ordem alfabética** do seu nome/nick.
    3.  Preencha a linha com suas informações resumidas e crie o link para o seu perfil (ex: `[Seu Nome](./seu-usuario.md)`).

Após alterar os **dois arquivos**, siga para o Passo 5.

### Como Adicionar Seu Projeto

Assim como nos perfis, pedimos que você edite **dois arquivos**.

1.  Vá para a pasta `/projetos/`.
2.  Use o **[TEMPLATE.md](./comunidade/projetos/TEMPLATE.md)** como base para criar seu arquivo `nome-do-projeto.md`.
3.  Abra o arquivo **[README.md](./comunidade/projetos/README.md)** da pasta, adicione uma nova linha na tabela da categoria correta e preencha com as informações do seu projeto.

### Como Adicionar uma Análise de Mercado

**Etapa 1: Criar a Análise Individual de Vaga**

1.  Encontre uma vaga interessante que possa servir como um bom material de estudo.
2.  Identifique o nível da vaga (Estágio, Júnior, Pleno, Sênior, etc.)
3.  Vá para a pasta correspondente em `/analise-de-mercado/[nivel]/`
4.  Use o **[TEMPLATE.md](./analise-de-mercado/TEMPLATE.md)** como base para criar sua análise detalhada.
5.  Salve o arquivo com um nome descritivo (ex: `analista-soc-pleno.md`)

**Etapa 2: Atualizar o README da Categoria**

1.  Abra o **README.md** da pasta do nível correspondente (ex: `/analise-de-mercado/4-pleno/README.md`)
2.  Adicione uma nova linha na tabela de análises disponíveis
3.  Atualize o contador de vagas se necessário

**Etapa 3: Atualizar o RESUMO.md da Categoria (Opcional mas Recomendado)**

Após adicionar várias análises em uma categoria, é importante atualizar o arquivo RESUMO.md para refletir as estatísticas consolidadas.

#### 🤖 Como Gerar/Atualizar um RESUMO.md

Os arquivos `RESUMO.md` são documentos analíticos que consolidam insights de **todas as vagas** de uma categoria. Eles contêm estatísticas, tendências e recomendações baseadas em dados reais.

**Metodologia Recomendada:**

Use um LLM (Claude, ChatGPT, etc.) com o seguinte prompt estruturado:

```markdown
# Prompt para Gerar RESUMO.md de Análise de Mercado

Você é um analista de mercado de cibersegurança especializado em inteligência de carreira.

**Contexto:**
Estou atualizando o RESUMO.md da categoria [NÍVEL] da Comunidade CyberSec BR.

**Arquivos para Análise:**
[Cole aqui o conteúdo de TODAS as análises de vaga da pasta]

**Tarefa:**
Crie um documento RESUMO.md analítico seguindo EXATAMENTE esta estrutura:

## Seções Obrigatórias:

1. **Cabeçalho**
   - Título: "📊 Resumo Analítico: Vagas [Categoria]"
   - Subtítulo: "> Análise baseada em X vagas reais"

2. **💰 Faixa Salarial**
   - Tabela com média, mínima, máxima
   - Observações sobre % de vagas que não informam salário
   - Comparação CLT vs PJ

3. **📍 Modalidade de Trabalho**
   - Gráfico em ASCII art mostrando distribuição % (Remoto/Híbrido/Presencial)
   - Insights sobre tendências

4. **🛠️ Top 5-10 Tecnologias/Ferramentas**
   - Tabela ranking com: Tecnologia, Categoria, % Vagas, Importância para CyberSec
   - Baseado em DADOS REAIS das análises

5. **🎓 Formação Acadêmica**
   - Gráfico ASCII mostrando distribuição
   - Insights sobre exigências

6. **🏢 Setores que Mais Contratam**
   - Tabela com setores, %, características, maturidade em segurança

7. **🏅 Certificações Recomendadas**
   - Tabela: Cert, Nível, ROI, Custo, Prioridade
   - Top 5-7 certificações

8. **📚 Roteiro de Estudos Consolidado**
   - Fase 1, 2, 3 com timeline
   - Específico para o nível analisado
   - Certificações, habilidades, projetos

9. **🚩 Red Flags e ✅ Green Flags**
   - Listas de bandeiras vermelhas críticas
   - Bandeiras amarelas (pontos de atenção)
   - Bandeiras verdes (sinais positivos)

10. **🌍 Distribuição Geográfica**
    - Gráfico ASCII
    - Insights regionais

11. **📊 Estatísticas Rápidas**
    - Bloco de código com resumo consolidado
    - Total de vagas, faixa salarial, % remoto, etc.

12. **🎯 Conclusão**
    - Recomendações práticas para diferentes perfis
    - Como se destacar no nível

13. **🔗 Links de Navegação**
    - Links para README da pasta, página principal, guias

14. **Rodapé**
    - Data de atualização
    - Nota sobre contribuições

**Requisitos Importantes:**
- Use APENAS dados REAIS extraídos das análises fornecidas
- Não invente estatísticas - se não houver dados, indique como "Não informado"
- Use emojis para melhor visualização
- Crie tabelas bem formatadas em Markdown
- Gráficos ASCII para distribuições percentuais
- Seja específico e prático nas recomendações
- Mantenha tom educativo e focado em progressão de carreira

**Formato de Saída:**
Markdown completo pronto para salvar como RESUMO.md
```

**Instruções de Uso do Prompt:**

1. Copie o prompt acima
2. Substitua `[NÍVEL]` pela categoria (Júnior, Pleno, etc.)
3. Cole o conteúdo de TODAS as análises .md da pasta após "Arquivos para Análise:"
4. Execute no LLM de sua preferência (Claude, GPT-4, etc.)
5. Revise o output gerado
6. Salve como `RESUMO.md` na pasta da categoria
7. Valide que todos os dados batem com as análises originais

**Exemplo de Estrutura de Arquivo:**

```
analise-de-mercado/
├── 3-junior/
│   ├── README.md (índice das análises)
│   ├── RESUMO.md (análise estatística - GERADO COM PROMPT)
│   ├── analista-junior-pam.md
│   ├── analista-fraudes.md
│   └── ...
```

**Arquivo de Referência:**
Veja [analise-de-mercado/1-suporte/RESUMO.md](./analise-de-mercado/1-suporte/RESUMO.md) como exemplo de qualidade esperada.

**Etapa 4: Atualizar o README Principal**

1.  Abra o **[README.md](./analise-de-mercado/README.md)** principal da análise de mercado
2.  Atualize o contador total de vagas analisadas
3.  Se criou uma nova categoria, adicione-a na tabela de navegação

---

## 📝 Padrões de Mensagens de Commit

Para manter o histórico do projeto organizado, use os seguintes prefixos:

- `feat:` - Nova funcionalidade ou conteúdo (ex: "feat: Adiciona análise de vaga SOC Pleno")
- `docs:` - Mudanças em documentação (ex: "docs: Atualiza FAQ com pergunta sobre certificações")
- `fix:` - Correção de erros (ex: "fix: Corrige link quebrado no README")
- `chore:` - Tarefas de manutenção (ex: "chore: Reorganiza estrutura de pastas")
- `refactor:` - Refatoração de conteúdo (ex: "refactor: Melhora organização do guia Red Team")

**Exemplos de boas mensagens:**
```bash
git commit -m "feat: Adiciona análise de vaga Analista Blue Team Pleno"
git commit -m "docs: Atualiza RESUMO.md da categoria Júnior com novas estatísticas"
git commit -m "fix: Corrige faixa salarial na análise de SOC N1"
```

---

Muito obrigado por ajudar a construir esta comunidade\! ❤️
