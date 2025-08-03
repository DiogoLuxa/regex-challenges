# 🧩 Desafio 03 — Número de Telefone com 8 ou 9 Dígitos

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que valide se uma string representa um **número de telefone com 8 ou 9 dígitos**, sem espaços ou símbolos.

---

## 📌 Requisitos

- A string deve conter **apenas números**.  
- Deve ter **exatamente 8 ou 9 dígitos**.  
- Não pode conter letras, espaços, símbolos ou estar vazia.

---

## 📥 Exemplos de Entrada

✅ `12345678`  
✅ `912345678`  
❌ `1234567` — apenas 7 dígitos  
❌ `1234567890` — 10 dígitos  
❌ `91234-5678` — contém símbolo  
❌ `telefone123` — contém letras  
❌ `` (string vazia)

---

## 💡 Dica

Use **quantificadores** para definir o número de dígitos permitidos.  
Combine com **âncoras** para garantir que toda a string siga o padrão.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **números com DDD**, no formato `11912345678` (2 dígitos de DDD + 8 ou 9 dígitos).

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_03.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 02](./desafio_02.md)  
- [Próximo desafio → Desafio 04](./desafio_04.md)

---

🔖 _Tags: regex, iniciante, validação, telefone, dígitos, expressão regular_