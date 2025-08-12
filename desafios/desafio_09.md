# 🧩 Desafio 09 — Validar uma data no formato `dd/mm/yyyy`

- [Voltar ao Sumário](../SUMARIO.md)  

### 📘 Nível: Iniciante  
### 🔹 Categoria: Validação Simples

---

## 🎯 Objetivo

Criar uma expressão regular que valide se uma string representa uma **data no formato `dd/mm/yyyy`**, com barras como separadores.

---

## 📌 Requisitos

- A data deve estar no formato `dd/mm/yyyy`  
- Deve conter **dois dígitos para o dia**, **dois para o mês** e **quatro para o ano**  
- Os separadores devem ser **barras (`/`)**  
- Não deve aceitar espaços, letras ou outros símbolos  
- Não precisa validar se a data é real (ex: `31/02/2023` ainda é aceita)

---

## 📥 Exemplos de Entrada

✅ `01/01/2023`  
✅ `31/12/1999`  
✅ `15/08/2020`  
❌ `1/1/2023` — dia e mês com apenas 1 dígito  
❌ `01-01-2023` — separador incorreto  
❌ `01/01/23` — ano com apenas 2 dígitos  
❌ `data: 01/01/2023` — contém texto antes  
❌ `01/01/2023.` — contém símbolo após

---

## 💡 Dica

Use **quantificadores** para definir a quantidade exata de dígitos e **caracteres fixos** como as barras.  
Combine com **âncoras** para garantir que toda a string siga o padrão.

---

## 🧠 Desafio Extra

Adapte a expressão para aceitar **datas válidas dentro de uma frase**, como `Hoje é 01/01/2023`, sem exigir que a string seja apenas a data.

---

## ✍️ Solução

> [Ver solução](../respostas/resposta_09.md) 🔍  
> Tente resolver por conta própria antes de consultar! 😉

---

- [Desafio anterior → Desafio 08](./desafio_08.md)  
- [Próximo desafio → Desafio 10](./desafio_10.md)

---

🔖 _Tags: regex, iniciante, data, formato, expressão regular_