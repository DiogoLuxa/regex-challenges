# ✅ Resposta — Desafio 06

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Validar um CEP Brasileiro  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
\b\d{5}-\d{3}\b
```

---

## 🔍 Explicação

- `\b` é um delimitador de palavra que garante que o CEP esteja **isolado**, sem letras ou símbolos colados  
- `\d{5}` valida exatamente **cinco dígitos numéricos**  
- `-` exige a presença de um **hífen** após os cinco dígitos  
- `\d{3}` valida exatamente **três dígitos numéricos** após o hífen  
- A expressão valida apenas o formato `00000-000`  
- Não permite letras ou símbolos extras antes ou depois do CEP

---

## 🧠 Desafio Extra — Aceitar CEP sem hífen

```regex
\b\d{5}-\d{3}\b|\b\d{8}\b
```

🔍 Essa versão usa o operador `|` para aceitar dois formatos distintos:

✅ Exemplos válidos:  
- `12345-678`  
- `00000-000`  
- `12345678`  
- `CEP: 12345678`

❌ Exemplos inválidos:  
- `12.345-678` — contém ponto  
- `1234-5678` — quantidade de dígitos incorreta  
- `abcde-123` — contém letras  
- `12345_678` — símbolo incorreto  
- `` — string vazia

---

- [Voltar ao Desafio 06](../desafios/desafio_06.md)  
- [Próximo desafio → Desafio 07](../desafios/desafio_07.md)

---

🔖 _Tags: regex, iniciante, CEP, Brasil, validação, expressão regular_