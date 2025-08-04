# 🧩 Desafio 04 — Começa com "Olá"

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que verifique se uma string **começa com a palavra "Olá"**, respeitando acentuação e posição.

---

## 📌 Requisitos

- A string deve **iniciar com "Olá"**, exatamente nessa grafia.    
- Deve respeitar o acento na letra "á".  
- Não pode conter caracteres ou números após "Olá".  
- Não deve aceitar variações como "olá", "OLÁ", "OlÁ", etc.

---

## 📥 Exemplos de Entrada

✅ `Olá, tudo bem?`  
✅ `Olá mundo`  
❌ `Olá123` — contém número após "Olá"
❌ `olá, tudo bem?` — sem letra maiúscula  
❌ `Oi, tudo bem?` — não começa com "Olá"  
❌ `Tudo começa com Olá` — "Olá" não está no início
❌ `Oláá` — contém letra repetida

---

## 💡 Dica

Use a **âncora de início (`^`)** para garantir que "Olá" esteja no começo da string.  
Lembre-se de **escapar caracteres especiais**, se necessário.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **"Olá" com letras maiúsculas ou minúsculas**, como `olá`, `OLÁ`, `OlÁ`, etc.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_04.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 03](./desafio_03.md)  
- [Próximo desafio → Desafio 05](./desafio_05.md)

---

🔖 _Tags: regex, iniciante, validação, início, olá, expressão regular_
