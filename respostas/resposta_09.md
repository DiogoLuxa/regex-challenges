# ✅ Resposta — Desafio 09

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Validar uma data no formato `dd/mm/yyyy`  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
^\d{2}/\d{2}/\d{4}$
```

---

## 🔍 Explicação

- `^` e `$` são **âncoras** que garantem que a string seja **exatamente** uma data no formato esperado  
- `\d{2}` representa **dois dígitos numéricos** para o dia e o mês  
- `\d{4}` representa **quatro dígitos numéricos** para o ano  
- As **barras (`/`)** são usadas como separadores fixos  
- Não aceita espaços, letras ou símbolos extras  
- Não valida se a data é real (ex: `31/02/2023` ainda é aceita)

✅ Exemplos válidos:  
- `01/01/2023`  
- `31/12/1999`  
- `15/08/2020`

❌ Exemplos inválidos:  
- `1/1/2023` — dia e mês com apenas 1 dígito  
- `01-01-2023` — separador incorreto  
- `01/01/23` — ano com apenas 2 dígitos  
- `data: 01/01/2023` — contém texto antes  
- `01/01/2023.` — contém símbolo após

---

## 🧠 Desafio Extra — Aceitar datas dentro de frases

```regex
\b\d{2}/\d{2}/\d{4}\b
```

🔍 Essa versão usa **delimitadores de palavra (`\b`)** para encontrar datas **dentro de frases**, sem exigir que a string seja apenas a data:

✅ Exemplos válidos:  
- `Hoje é 01/01/2023`  
- `A reunião será em 15/08/2020`  
- `Datas como 31/12/1999 são importantes`

❌ Exemplos inválidos:  
- `01-01-2023` — separador incorreto  
- `1/1/2023` — dígitos incompletos  
- `data:01/01/2023.` — sem espaço ou com símbolo grudado

---

- [Voltar ao Desafio 09](../desafios/desafio_09.md)  
- [Próximo desafio → Desafio 10](../desafios/desafio_10.md)

---

🔖 _Tags: regex, iniciante, data, formato, expressão regular_