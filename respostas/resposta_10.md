# ✅ Resposta — Desafio 10

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Verificar se uma string contém apenas letras maiúsculas  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
^[A-Z]+$
```

---

## 🔍 Explicação

- `^` e `$` são **âncoras** que garantem que a string seja **exatamente composta por letras maiúsculas**
- `[A-Z]` representa **qualquer letra maiúscula do alfabeto inglês**
- `+` é um **quantificador** que exige **uma ou mais letras maiúsculas**
- Não aceita letras minúsculas, números, espaços ou símbolos
- Se quiser aceitar uma string **vazia** como válida, substitua `+` por `*`

✅ Exemplos válidos:  
- `ABC`  
- `HELLO`  
- `REGEX`

❌ Exemplos inválidos:  
- `Abc` — contém letra minúscula  
- `ABC123` — contém números  
- `ABC!` — contém símbolo  
- `ABC DEF` — contém espaço  
- `abc` — todas minúsculas

---

## 🧠 Desafio Extra 2 — Aceitar frases com palavras maiúsculas

```regex
^[A-ZÀ-ÿ]+(?: [A-ZÀ-ÿ]+)*$
```

### 🔍 Explicação

- `^[A-ZÀ-ÿ]+` exige que a frase comece com uma palavra composta **apenas por letras maiúsculas**, incluindo letras acentuadas
- `(?: [A-ZÀ-ÿ]+)*` permite **palavras subsequentes separadas por espaço**, todas em maiúsculas e com possíveis acentos

✅ Exemplos válidos:  
- `HOJE É UM DIA FELIZ`  
- `VOCÊ É INCRÍVEL`  
- `À VISTA DO FATO`  
- `ÓTIMA SOLUÇÃO`  

❌ Exemplos inválidos:  
- `Hoje é um dia feliz` — contém letras minúsculas  
- `ABC123` — contém números  
- `ABC!` — contém símbolos  
- `ABC DEF ` — espaço no final

---

- [Voltar ao Desafio 10](../desafios/desafio_10.md)  
- [Próximo desafio → Desafio 11](../desafios/desafio_11.md)

---

🔖 _Tags: regex, iniciante, maiúsculas, letras, acentuação, validação, expressão regular_