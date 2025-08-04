# ✅ Resposta — Desafio 04

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Começa com "Olá"  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
/^Olá(?![a-zA-ZÀ-ÿ]|\d)/
```

---

## 🔍 Explicação

- `^` garante que a string **comece** com "olá"  
- `olá` é a palavra exata que queremos validar (minúscula e com acento)  
- `(?![a-zA-ZÀ-ÿ]|\d)` é uma negação lookahead que impede letras latinas (inclusive acentuadas) ou dígitos imediatamente após "olá"
    - Isso bloqueia variações como oláá, oláabc, oláç, olá1, etc.
    - Permite espaços, pontuação, símbolos e fim de string após "olá


---

## 🧠 Desafio Extra — Aceitar variações de maiúsculas/minúsculas

```regex
/^Olá(?![a-zA-ZÀ-ÿ]|\d)/i
```

🔍 Essa versão usa o modificador `/i` para tornar a expressão **case-insensitive**, permitindo:

✅ Exemplos válidos:  
- `Olá, tudo bem?`    
- `oLá`  
- `olá mundo`  
- `Olá!`

❌ Exemplos inválidos:  
- `Oláá` — contém acento extra  
- `Oláabc` — contém letras coladas  
- `Tudo começa com Olá` — "Olá" não está no início  
- `` — string vazia

---

- [Voltar ao Desafio 04](../desafios/desafio_04.md)  
- [Próximo desafio → Desafio 05](../desafios/desafio_05.md)

---

🔖 _Tags: regex, iniciante, olá, início, validação, expressão regular_
