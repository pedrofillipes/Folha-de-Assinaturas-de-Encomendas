# 📝 Folha de Assinaturas de Encomendas

Sistema simples para geração e impressão de folha de assinaturas para controle de encomendas em condomínios.

## 📦 Funcionalidade

- Escolha da torre (A, B, C, D, E) ou opção "ADMINISTRAÇÃO"
- Colagem dos dados brutos do sistema
- Geração de uma tabela filtrada, ordenada e pronta para impressão
- Fallback para exibir a tabela na própria página, caso pop-ups estejam bloqueados
- Impressão otimizada (com instruções de remoção de cabeçalho/rodapé do navegador)

## ⚙️ Tecnologias

- HTML5  
- CSS3 com variáveis  
- JavaScript (puro)  
- Google Fonts (Montserrat)

## 🧠 Regras aplicadas

- **Torres A e B**:
  - Remove todas as ocorrências de "SALA" da unidade
  - Oculta os campos "Data:" e "Hora:" na célula "Retirada"

- **ADMINISTRAÇÃO**:
  - Reconhece unidades com valor `"administracao"` (minúsculo e sem acento)
  - Exibe como `"ADM"` na tabela
  - Também oculta "Data:" e "Hora:" na célula "Retirada"

- Os campos da unidade são convertidos para **maiúsculas** automaticamente
- A tabela é impressa sem quebrar linhas (`break-inside: avoid`)
- Colunas com **largura fixa** e **negrito nas colunas 3 (Unidade) e 5 (Destinatário)**
- Evita duplicatas com base em chave única: `data + unidade + morador + código`

## 🚨 Resiliência e Validações

- Verifica se `window.open` funcionou para gerar nova aba
- Caso falhe (por bloqueio de pop-up), exibe a tabela no próprio HTML
- Valida se há pelo menos 7 colunas por linha
- Alerta o usuário se não houver registros válidos
- Evita registros duplicados usando um `Set` inteligente

## 🖨️ Instruções de uso

1. Abra o arquivo `index.html` no navegador
2. Escolha a torre desejada (ou "ADMINISTRAÇÃO")
3. Cole os dados brutos copiados do sistema
4. Clique em **"Gerar para Impressão"**
5. Se o navegador bloquear pop-ups, a tabela aparecerá abaixo do formulário
6. No diálogo de impressão, **desmarque a opção “Cabeçalhos e rodapés”** para melhor resultado

## 📁 Estrutura do Projeto

```
📁 projeto/
├── index.html
├── style.css
├── vars.css
└── main.js
```

## ✍️ Autor

Pedro Oliveira  
https://github.com/pedrofillipes
