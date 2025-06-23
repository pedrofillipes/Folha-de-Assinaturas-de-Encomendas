# 📝 Folha de Assinaturas de Encomendas

Sistema simples para geração e impressão de folha de assinaturas para controle de encomendas em condomínios.

## 📦 Funcionalidade

- Escolha da torre (A, B, C, D, E) ou opção "ADMINISTRAÇÃO"
- Colagem dos dados brutos do sistema
- Geração de uma tabela filtrada e ordenada
- Impressão otimizada para papel (com opção de retirar cabeçalhos automáticos)

## ⚙️ Tecnologias

- HTML5
- CSS3 com variáveis
- JavaScript (puro)
- Google Fonts (Montserrat)

## 🧠 Regras aplicadas

- Torres A e B: remove todas as ocorrências de "SALA" da unidade (não importa a posição)
- Torres A e B: oculta campos "Data:" e "Hora:" na célula "Retirada"
- ADMINISTRAÇÃO:
  - Reconhece unidades com valor `"administracao"` (sem acento e minúsculo)
  - Substitui na tabela o nome da unidade por `"ADM"`
  - Também oculta "Data:" e "Hora:" na célula "Retirada"
- Os campos da unidade são automaticamente convertidos para maiúsculas
- Células de tabela não quebram na impressão (`break-inside: avoid`)
- Colunas com largura fixa e negrito nas colunas 3 (Unidade) e 5 (Destinatário)

## 🖨️ Instruções de uso

1. Abra o `index.html` no navegador
2. Escolha a torre desejada (ou "ADMINISTRAÇÃO")
3. Cole os dados brutos no campo de entrada
4. Clique em "Gerar para Impressão"
5. Na janela de impressão, **desmarque “Cabeçalhos e rodapés”**

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
