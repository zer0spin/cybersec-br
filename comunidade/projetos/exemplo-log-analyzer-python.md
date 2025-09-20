# Analisador de Logs de Acesso Web em Python

**Autor(es):** [zer0spin](./../membros/zer0spin.md)

**Categoria:** Blue Team 

**Área:** SecOps

**Sistema Operacional Compatível:** Linux

## 📄 Descrição Rápida

Um script em Python que analisa logs de acesso de servidores web (Apache/Nginx) para identificar atividades suspeitas e gerar um relatório de segurança conciso.

## 🎯 O Problema que Resolve

Analisar arquivos de log manualmente é uma tarefa demorada e sujeita a erros. Esta ferramenta automatiza a triagem inicial, permitindo que analistas de segurança foquem rapidamente nos eventos mais críticos e reduzam o tempo de resposta a incidentes.

## 🚀 Demonstração Rápida (Como Funciona)

Veja a simplicidade e o poder da ferramenta em ação.

### ↪️ Exemplo de Uso (Input)
O script precisa apenas do caminho para o arquivo de log e, opcionalmente, o nome do arquivo de saída.

```bash
# Comando para analisar um log e salvar o relatório em HTML
python log_analyzer.py --logfile /var/log/apache2/access.log --output relatorio_seguranca.html
```

### ↩️ Resultados (Output)

A ferramenta gera um relatório interativo em HTML, destacando os IPs com mais atividades suspeitas, as tentativas de ataques mais comuns (SQLi, XSS, Path Traversal) e gráficos com as estatísticas gerais de acesso.

## 🛠️ Tecnologias Utilizadas

  * **Linguagem:** Python 3
  * **Ferramentas/Bibliotecas:** Pandas, Regex, Argparse, Jinja2 (para gerar o relatório HTML).
  * **Cloud/Infra:** N/A (roda localmente em qualquer sistema com Python).
  * **SO Compatível:🐧 Linux, 🪟 Windows, 🍏 macOS** 
  * **Dependências/Instalação:** O script requer Python 3. As bibliotecas podem ser instaladas com o comando `pip install -r requirements.txt`.

### Nota sobre a compatibilidade

Por ser escrito em Python, o script é multiplataforma. A única diferença prática entre os sistemas operacionais é o formato do caminho para o arquivo de log. Ambientes Linux/macOS usam barras normais (`/`), enquanto o Windows usa barras invertidas (`\`). O exemplo de uso acima demonstra ambos os casos.

## 📺 Live Demo / Vídeo de Demonstração 

  * **[Assista a um vídeo de 2 minutos mostrando a ferramenta em ação](https://www.youtube.com/watch?v=BSlfQWpCFco)**

## 🔗 Links Oficiais

  * **[Repositório no GitHub](https://github.com/zer0spin)**
  * **[Artigo explicando a construção da ferramenta](https://x.com/zer0spin)**
