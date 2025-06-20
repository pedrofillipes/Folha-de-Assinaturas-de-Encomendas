# 📝 Folha de Assinaturas de Encomendas

Sistema simples para geração e impressão de folha de assinaturas para controle de encomendas em condomínios.

## 📦 Funcionalidade

- Escolha da torre (A, B, C, D ou E)
- Colagem dos dados brutos do sistema
- Geração de uma tabela filtrada e ordenada
- Impressão otimizada para papel (com opção de retirar cabeçalhos automáticos)

## ⚙️ Tecnologias

- HTML5
- CSS3 com variáveis
- JavaScript (puro)
- Google Fonts (Montserrat)

## 🧠 Regras aplicadas

- Torres A e B: remove "SALA" das unidades
- Torres A e B: oculta campos "Data:" e "Hora:" na célula "Retirada"
- Células de tabela não quebram na impressão (`break-inside: avoid`)
- Colunas de largura fixa com alinhamento e negrito nas colunas 3 e 5

## 🖨️ Instruções de uso

1. Abra o `index.html` no navegador
2. Escolha a torre desejada
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

---

Sinta-se à vontade para clonar, adaptar ou contribuir com melhorias!
