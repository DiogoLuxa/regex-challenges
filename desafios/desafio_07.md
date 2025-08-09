# 🧩 Desafio 07 — Validar um CPF com ou sem pontuação

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que valide se uma string representa um **CPF brasileiro** no formato tradicional ou sem pontuação.

---

## 📌 Requisitos

- O CPF deve estar no formato `000.000.000-00`
- Deve conter **apenas números**, com pontuação  
- Pontuação permitida: **pontos e hífen** nas posições corretas  
- Não deve aceitar espaços, letras ou símbolos extras  
- Não deve aceitar formatos incompletos ou com pontuação fora de lugar
- Não deve aceitar formatos sem pontuação

---

## 📥 Exemplos de Entrada

✅ `123.456.789-00`  
❌ `123456789-00` — faltam os pontos  
❌ `123.456.789.00` — pontuação incorreta  
❌ `abc.def.ghi-jk` — contém letras  
❌ `123_456_789-00` — símbolo incorreto  
❌ `1234567890` — quantidade de dígitos incorreta

---

## 💡 Dica

Use **grupos de dígitos** com quantificadores e **caracteres fixos** como ponto e hífen.  
Combine com **âncoras** para garantir que toda a string siga o padrão.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **ambos os formatos** — com pontuação (`000.000.000-00`) ou sem (`00000000000`).

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_07.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 06](./desafio_06.md)  
- [Próximo desafio → Desafio 08](./desafio_08.md)

---

🔖 _Tags: regex, iniciante, CPF, Brasil, validação, expressão regular_