# 🧩 Desafio 08 — Verificar se uma string contém a palavra "regex"

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que verifique se uma string **contém a palavra "regex"** em qualquer parte do texto.

---

## 📌 Requisitos

- A string deve conter a palavra `"regex"` exatamente nessa grafia  
- Pode estar no início, meio ou fim da string  
- Deve respeitar letras minúsculas  
- Não deve aceitar variações como `"Regex"`, `"REGEX"`, `"reGex"`, etc.  
- Pode estar isolada ou dentro de uma frase

---

## 📥 Exemplos de Entrada

✅ `estou aprendendo regex`  
✅ `regex é poderoso`  
✅ `vamos usar regex hoje`  
❌ `Regex é legal` — letra maiúscula  
❌ `REGEX` — todas maiúsculas  
❌ `reGex` — mistura de maiúsculas  
❌ `expressão regular` — não contém "regex"  

---

## 💡 Dica

Não é necessário usar âncoras (`^` ou `$`) se a palavra pode aparecer em qualquer parte da string.  
Use o padrão literal `"regex"` e evite modificadores de case-insensitive.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar `"regex"` com **qualquer combinação de maiúsculas e minúsculas**, como `Regex`, `REGEX`, `ReGeX`, etc.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_08.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 07](./desafio_07.md)  
- [Próximo desafio → Desafio 09](./desafio_09.md)

---

🔖 _Tags: regex, iniciante, busca, palavra, expressão regular_