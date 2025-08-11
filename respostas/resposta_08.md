# ✅ Resposta — Desafio 08

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Verificar se uma string contém a palavra "regex"  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
regex
```

---

## 🔍 Explicação

- A expressão busca literalmente pela palavra `"regex"`  
- Não usa âncoras, permitindo que a palavra apareça em qualquer parte da string  
- A correspondência é **case-sensitive**, ou seja, só aceita `"regex"` em letras minúsculas  
- Não valida variações como `"Regex"`, `"REGEX"` ou `"ReGeX"`  

✅ Exemplos válidos:  
- `estou aprendendo regex`  
- `regex é poderoso`  
- `vamos usar regex hoje`

❌ Exemplos inválidos:  
- `Regex é legal` — letra maiúscula  
- `REGEX` — todas maiúsculas  
- `reGex` — mistura de maiúsculas  
- `expressão regular` — não contém "regex"

---

## 🧠 Desafio Extra — Aceitar qualquer combinação de maiúsculas e minúsculas

```regex
(?i)regex
```

🔍 Essa versão usa a **flag `(?i)`** para tornar a busca **case-insensitive**:

✅ Exemplos válidos:  
- `regex`  
- `Regex`  
- `REGEX`  
- `ReGeX`  
- `estou estudando Regex agora`

❌ Exemplos inválidos:  
- `expressão regular` — não contém "regex"  
- `re.gex` — contém ponto no meio  
- `` — string vazia

---

- [Voltar ao Desafio 08](../desafios/desafio_08.md)  
- [Próximo desafio → Desafio 09](../desafios/desafio_09.md)

---

🔖 _Tags: regex, iniciante, busca, palavra, expressão regular_
