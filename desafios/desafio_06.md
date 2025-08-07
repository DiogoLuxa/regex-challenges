# 🧩 Desafio 06 — Validar um CEP Brasileiro

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que valide se uma string representa um **CEP brasileiro** no formato padrão.

---

## 📌 Requisitos

- O CEP deve estar no formato `00000-000` (cinco dígitos, hífen, três dígitos)  
- Deve conter **apenas números e um hífen** na posição correta  
- Não deve aceitar espaços, letras ou símbolos extras  
- Não deve aceitar formatos alternativos como `00000000` ou `00.000-000`

---

## 📥 Exemplos de Entrada

✅ `12345-678`  
✅ `00000-000`  
❌ `12345678` — sem hífen  
❌ `12.345-678` — contém ponto  
❌ `abcde-123` — contém letras  
❌ `12345_678` — símbolo incorreto  
❌ `1234-5678` — quantidade de dígitos incorreta

---

## 💡 Dica

Use **quantificadores** para definir a quantidade exata de dígitos e **caracteres fixos** como o hífen.  
Combine com **âncoras** para garantir que toda a string siga o padrão.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **CEPs sem hífen**, como `12345678`, além do formato com hífen.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_06.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 05](./desafio_05.md)  
- [Próximo desafio → Desafio 07](./desafio_07.md)

---

🔖 _Tags: regex, iniciante, validação, CEP, Brasil, expressão regular_