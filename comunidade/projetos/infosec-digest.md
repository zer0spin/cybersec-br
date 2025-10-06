# InfoSec Digest

**Autor(es):** [zer0spin](./../membros/zer0spin.md)

**Categoria:** 🛡️ Blue Team / SecOps / Defesa

**Área:** Threat Intelligence, Agregação de Notícias, Automação

## 📄 Descrição Rápida

InfoSec Digest é um **agregador moderno, seguro e de alta performance** para notícias e podcasts de cibersegurança. Com arquitetura **GitOps**, o projeto entrega conteúdo estático com atualizações automatizadas a cada hora, centralizando as principais fontes de informação de segurança em uma única interface leve e responsiva.

## 🎯 O Problema que Resolve

Profissionais de cibersegurança precisam acompanhar múltiplas fontes de notícias, blogs técnicos e podcasts para se manterem atualizados sobre ameaças, vulnerabilidades e tendências do mercado. **InfoSec Digest** centraliza essas informações em um único lugar, eliminando a necessidade de visitar dezenas de sites diferentes ou configurar múltiplos feeds RSS.

**Principais benefícios:**
- ✅ **Centralização** de conteúdo de múltiplas fontes confiáveis
- ✅ **Atualizações automáticas** a cada hora via GitHub Actions
- ✅ **Interface minimalista** e responsiva (Pico.css)
- ✅ **Segurança by design** com prevenção de XSS e arquitetura estática
- ✅ **Alta performance** com entrega via CDN (Vercel)
- ✅ **Resiliência** - falhas em feeds individuais não derrubam o sistema

## 🚀 Demonstração Rápida (Como Funciona)

O InfoSec Digest opera em dois componentes principais:

### 1️⃣ **Coleta de Dados (Backend Automatizado)**

Um workflow do GitHub Actions executa a cada hora:

```bash
# O fetcher.py busca e processa fontes configuradas
python fetcher.py

# Saída: data.json com notícias agregadas e classificadas
```

**Fluxo de Processamento:**
1. 📥 Lê lista de fontes de `sources.json` (blogs, feeds RSS, podcasts)
2. 🔍 Busca e extrai conteúdo de cada fonte
3. 🏷️ Classifica artigos usando palavras-chave de `keywords.json`
4. 📊 Gera arquivo estático `data.json` com conteúdo agregado
5. ✅ Tolera falhas: se uma fonte estiver offline, as demais continuam funcionando

### 2️⃣ **Entrega de Conteúdo (Frontend Estático)**

O site estático busca e renderiza os dados automaticamente:

```javascript
// JavaScript vanilla busca data.json
fetch('data.json')
  .then(response => response.json())
  .then(data => renderNews(data))
  // Conteúdo tratado como texto para prevenir XSS
```

### ↩️ Resultado Final

Uma interface web moderna que exibe:
- 📰 Últimas notícias de cibersegurança agregadas
- 🏷️ Classificação automática por categoria (Vulnerabilidades, Malware, Incidentes, etc.)
- 🔗 Links diretos para fontes originais
- 📅 Data e hora de atualização

## 🛠️ Tecnologias Utilizadas

* **Linguagem Principal:** Python 3.11
* **Frontend:** HTML5, Vanilla JavaScript, Pico.css (CSS framework minimalista)
* **Automação:** GitHub Actions (workflows agendados)
* **Hospedagem:** Vercel (entrega via CDN global)
* **Arquitetura:** GitOps, JAMstack (site estático)
* **SO Compatível:** 🌐 Web (multiplataforma)
* **Dependências:**
  - Python: `feedparser`, `requests`, `beautifulsoup4`
  - Nenhuma dependência no frontend (vanilla JS)

## 📺 Live Demo

* **[🔗 Acesse o InfoSec Digest ao vivo](https://infosec-digest.vercel.app)**

## 🔗 Links Oficiais

* **[📦 Repositório no GitHub](https://github.com/zer0spin/infosec-digest)**
* **[🚀 Deploy em Produção (Vercel)](https://infosec-digest.vercel.app)**

## 🌟 Destaques Técnicos

### Segurança (Security by Design)
- 🔒 Arquitetura totalmente estática (sem backend exposto)
- 🛡️ Prevenção de XSS tratando todo conteúdo como texto
- 🔐 Sem armazenamento de dados sensíveis
- ✅ Validação de fontes confiáveis

### Performance
- ⚡ Entrega via CDN global (Vercel Edge Network)
- 📦 Arquivo `data.json` otimizado e comprimido
- 🎨 CSS minimalista (Pico.css - apenas ~10KB)
- 🚀 Vanilla JavaScript (sem frameworks pesados)

### Escalabilidade
- 📈 Adicionar novas fontes é simples (editar `sources.json`)
- 🔄 Atualizações automáticas sem intervenção manual
- 🌍 Suporta fontes em múltiplos idiomas

## 🤝 Como Contribuir

Quer adicionar uma nova fonte de notícias ou melhorar o projeto?

1. Faça fork do repositório
2. Adicione a fonte em `sources.json` (seguindo o formato)
3. Teste localmente: `python fetcher.py`
4. Envie um Pull Request

---

**🎯 Use Case Ideal:** Profissionais de Blue Team, Threat Intelligence Analysts, CISOs e entusiastas que precisam se manter atualizados sobre o cenário de ameaças de forma centralizada e eficiente.
