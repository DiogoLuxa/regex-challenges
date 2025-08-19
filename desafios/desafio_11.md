# 🧩 Desafio 11 — Extrair todos os números de uma string

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Extração de Dados

---

## 🎯 Objetivo

Criar uma expressão regular que **extraia todos os números** presentes em uma string, independentemente da posição ou contexto.

---

## 📌 Requisitos

- A expressão deve identificar **todos os números inteiros** na string  
- Pode extrair números isolados ou dentro de frases  
- Não precisa validar se os números são reais, positivos ou negativos  
- Não deve extrair letras, símbolos ou partes de palavras

---

## 📥 Exemplos de Entrada

✅ `Tenho 2 gatos e 14 peixes` → extrai `2`, `14`  
✅ `O valor é 1000 reais` → extrai `1000`  
✅ `123abc456` → extrai `123`, `456`  
✅ `Números: 7, 8, 9.` → extrai `7`, `8`, `9`  
❌ `abc` — não contém números  
❌ `!@#` — apenas símbolos

---

## 💡 Dica

Use a classe de caracteres `\d` para representar **dígitos numéricos**  
Combine com o quantificador `+` para capturar **sequências de dígitos**

---

## 🧠 Desafio Extra

Adapte a expressão para extrair **números decimais**, como `3.14`, `0.99`, `100.0`, além dos inteiros.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_11.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 10](./desafio_10.md)  
- [Próximo desafio → Desafio 12](./desafio_12.md)

---

🔖 _Tags: regex, iniciante, números, extração, expressão regular_