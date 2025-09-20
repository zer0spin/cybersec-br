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

O processo é o mesmo: edite **dois arquivos**.

1.  Encontre uma vaga interessante que possa servir como um bom material de estudo.
2.  Vá para a pasta `/analise-de-mercado/`.
3.  Use o **[TEMPLATE.md](./analise-de-mercado/TEMPLATE.md)** como base para criar sua análise.
4.  Abra o arquivo **[README.md](./analise-de-mercado/README.md)** da pasta e adicione sua análise à tabela.

---

Muito obrigado por ajudar a construir esta comunidade\! ❤️
