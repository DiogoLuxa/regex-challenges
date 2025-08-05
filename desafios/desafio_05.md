# 🧩 Desafio 05 — Termina com "fim"

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que verifique se uma string **termina com a palavra "fim"**, respeitando grafia e posição.

---

## 📌 Requisitos

- A string deve **terminar com "fim"**, exatamente nessa grafia.  
- Pode conter qualquer conteúdo antes de "fim".  
- Não deve aceitar variações como "Fim", "FIM", "fim!", "fim123", etc.  
- Deve rejeitar strings que contenham "fim" no meio ou início.

---

## 📥 Exemplos de Entrada

✅ `até o fim`  
✅ `chegamos ao grande fim`  
❌ `fim de tudo` — "fim" está no início  
❌ `Fim` — letra maiúscula  
❌ `fim!` — contém símbolo após "fim"  
❌ `fim123` — contém números após "fim"  
❌ `o fim está próximo` — "fim" não está no final

---

## 💡 Dica

Use a **âncora de fim (`$`)** para garantir que "fim" esteja no final da string.  
Evite aceitar letras, números ou símbolos após a palavra.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **"fim" com letras maiúsculas ou minúsculas**, como `Fim`, `FIM`, `fIm`, etc.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_05.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 04](./desafio_04.md)  
- [Próximo desafio → Desafio 06](./desafio_06.md)

---

🔖 _Tags: regex, iniciante, validação, fim, encerramento, expressão regular_