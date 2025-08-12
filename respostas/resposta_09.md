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
(?<=\s)\b\d{2}/\d{2}/\d{4}\b(?=[\s])
```

## 🔍 Explicação

- `(?<=\s)` **Lookbehind positivo**: garante que antes da data exista um **espaço em branco** (como um espaço, tabulação ou quebra de linha).
- `\b` **Delimitador de palavra**: assegura que a data comece exatamente onde uma palavra começaria (evita capturar partes de palavras).
- `\d{2}/\d{2}/\d{4}` corresponde a **dois dígitos**, uma barra, **dois dígitos**, outra barra, e **quatro dígitos** — ou seja, o padrão de data `dd/mm/aaaa`.
- `\b` outro delimitador de palavra, marcando o fim da data.
- `(?=\s)` **Lookahead positivo**: garante que depois da data também exista um **espaço em branco**.

Essa expressão regular identifica datas no formato dd/mm/aaaa que estão isoladas por espaços dentro de um texto. Vamos destrinchar cada parte.

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