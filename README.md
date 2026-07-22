# 🏠 Chácara — Organizador de Quartos

Sistema web para organizar a hospedagem de participantes em quartos durante encontros religiosos (Encontro de Homens, Encontro de Mulheres) realizados na chácara da igreja.

## ✨ Funcionalidades

- 📋 **Múltiplos encontros** — Crie, selecione e gerencie vários eventos
- ⚙️ **Configuração de quartos** — Nome, cor, capacidade, número de líderes e vocação por faixa etária
- 📏 **Regras de distribuição** — Separe ou junte participantes por sobrenome, unidade, célula, faixa etária e telefone de emergência
- 📥 **Importação de Excel** — Mapeamento inteligente de colunas com confirmação manual
- 👑 **Cadastro de líderes** — Aloque líderes por quarto respeitando o limite configurado
- 🎲 **Distribuição automática** — Algoritmo que respeita vocação dos quartos (-25, +50, neutro) e regras ativas
- 🖱️ **Drag and drop** — Ajuste manual arrastando participantes entre quartos
- 📄 **Geração de PDFs** — Lista geral (vertical) + PDF público por quarto + PDF privado com dados de saúde e emergência
- 💾 **Backup e restore** — Exporte e importe todos os dados em JSON
- 🌙 **Tema escuro** — Identidade visual Charcoal & Ember

## 🚀 Como usar

1. Abra o arquivo `index.html` em qualquer navegador moderno
2. Crie um encontro na aba **Encontros**
3. Configure os quartos em **Configurar Quartos**
4. Cadastre líderes na aba **Líderes**
5. Aloque os líderes aos quartos em **Alocar Líderes**
6. Importe a planilha de participantes em **Participantes**
7. Defina as regras em **Regras**
8. Vá para **Distribuir** e clique em "Distribuir automático"
9. Ajuste manualmente se necessário (arraste os chips)
10. Gere os PDFs

## 📄 PDFs gerados

| PDF | Orientação | Conteúdo |
|---|---|---|
| Lista Geral | Vertical | Ordem alfabética: cor do quarto, nome, igreja, telefone |
| Público (por quarto) | Paisagem | Cabeçalho colorido + lista de nomes (1 folha) |
| Privado (por quarto) | Paisagem | Tabela com nome, telefone, emergência, igreja, alergias |

## 🛠️ Tecnologias

- HTML5, CSS3, JavaScript vanilla
- [SheetJS](https://sheetjs.com/) — Leitura de arquivos Excel (.xlsx, .xls, .csv)
- [jsPDF](https://github.com/parallax/jsPDF) — Geração de PDFs
- [jsPDF-AutoTable](https://github.com/davidjbradshaw/jsPDF-AutoTable) — Tabelas nos PDFs
- localStorage — Persistência dos dados (sem backend)

## 📂 Estrutura
