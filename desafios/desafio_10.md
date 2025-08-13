# 🧩 Desafio 10 — Verificar se uma string contém apenas letras maiúsculas

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que verifique se uma string contém **somente letras maiúsculas**, sem espaços, números ou símbolos.

---

## 📌 Requisitos

- A string deve conter **apenas letras maiúsculas de A a Z**  
- Não deve conter letras minúsculas, números, espaços ou símbolos  
- Pode ter qualquer quantidade de letras, desde que todas sejam maiúsculas  
- A string pode estar vazia (dependendo da regra que você quiser aplicar)

---

## 📥 Exemplos de Entrada

✅ `ABC`  
✅ `HELLO`  
✅ `REGEX`  
❌ `Abc` — contém letra minúscula  
❌ `ABC123` — contém números  
❌ `ABC!` — contém símbolo  
❌ `ABC DEF` — contém espaço  
❌ `abc` — todas minúsculas

---

## 💡 Dica

Use **classes de caracteres** para definir o intervalo de letras maiúsculas (`[A-Z]`)  
Combine com **quantificadores** e **âncoras** para garantir que toda a string siga o padrão

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **palavras maiúsculas dentro de frases**, como `HOJE É UM DIA FELIZ`, ignorando espaços entre as palavras.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_10.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 09](./desafio_09.md)  
- [Próximo desafio → Desafio 11](./desafio_11.md)

---

🔖 _Tags: regex, iniciante, maiúsculas, letras, validação, expressão regular_