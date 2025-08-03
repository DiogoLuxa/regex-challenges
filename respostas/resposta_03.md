# ✅ Resposta — Desafio 03

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Número de Telefone com 8 ou 9 Dígitos  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
^\d{8,9}$
```

---

## 🔍 Explicação

- `^` e `$` são âncoras que garantem que toda a string siga o padrão.  
- `\d` representa qualquer dígito de 0 a 9.  
- `{8,9}` exige que a string tenha **exatamente 8 ou 9 dígitos**.  
- Não aceita letras, espaços, símbolos ou strings vazias.

---

## 🧠 Desafio Extra — Com DDD Opcional

```regex
^(\d{2})?\d{8,9}$
```

🔍 Essa versão permite que o número comece com um **DDD opcional** de 2 dígitos:  
- `(\d{2})?` → grupo opcional para o DDD  
- `\d{8,9}` → número de telefone com 8 ou 9 dígitos  
- A string pode ter **8, 9, 10 ou 11 dígitos**, dependendo da presença do DDD

✅ Exemplos válidos:  
- `912345678` → número com 9 dígitos  
- `12345678` → número com 8 dígitos  
- `11912345678` → DDD 11 + número com 9 dígitos  
- `2198765432` → DDD 21 + número com 8 dígitos  

❌ Exemplos inválidos:  
- `11-912345678` — contém símbolo  
- `11 987654321` — contém espaço  
- `abc11912345678` — contém letras  
- `` — string vazia

---

- [Voltar ao Desafio 03](../desafios/desafio_03.md)  
- [Próximo desafio → Desafio 04](../desafios/desafio_04.md)

---

🔖 _Tags: regex, iniciante, telefone, DDD, dígitos, validação, expressão regular_
