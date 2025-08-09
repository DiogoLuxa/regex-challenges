# ✅ Resposta — Desafio 07

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Validar um CPF Brasileiro  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
\b\d{3}\.\d{3}\.\d{3}-\d{2}\b
```

---

## 🔍 Explicação

- `\b` garante que o CPF esteja **isolado**, sem letras ou símbolos colados  
- `\d{3}` valida **três dígitos numéricos**  
- `\.` exige a presença de um **ponto** após os três primeiros grupos  
- `-` exige a presença de um **hífen** após os nove dígitos  
- `\d{2}` valida os **dois dígitos finais** do CPF  
- A expressão valida apenas o formato `000.000.000-00`  
- Não permite letras, espaços ou símbolos extras

---

## 🧠 Desafio Extra — Aceitar CPF sem pontuação

```regex
\b\d{3}\.\d{3}\.\d{3}-\d{2}\b|\b\d{11}\b
```

🔍 Essa versão usa o operador `|` para aceitar dois formatos distintos:

✅ Exemplos válidos:  
- `123.456.789-00`  
- `00000000000`  
- `CPF: 98765432100`  

❌ Exemplos inválidos:  
- `123456789-00` — faltam os pontos  
- `123.456.789.00` — pontuação incorreta  
- `abc.def.ghi-jk` — contém letras  
- `123_456_789-00` — símbolo incorreto  
- `1234567890` — quantidade de dígitos incorreta  
- `` — string vazia

---

- [Voltar ao Desafio 07](../desafios/desafio_07.md)  
- [Próximo desafio → Desafio 08](../desafios/desafio_08.md)

---

🔖 _Tags: regex, iniciante, CPF, Brasil, validação, expressão regular_