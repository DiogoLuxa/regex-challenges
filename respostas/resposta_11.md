# ✅ Resposta — Desafio 11

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Extrair todos os números de uma string  
🔹 Nível: Iniciante  
🔹 Categoria: Extração de Dados

---

## 🧪 Expressão Regular

```regex
\d+
```

---

## 🔍 Explicação

- `\d` representa **qualquer dígito numérico** de `0` a `9`  
- `+` é um **quantificador** que captura **uma ou mais ocorrências consecutivas** de dígitos  
- A expressão extrai **todos os números inteiros** presentes na string  
- Funciona mesmo que os números estejam misturados com texto ou símbolos

✅ Exemplos válidos:  
- `Tenho 2 gatos e 14 peixes` → extrai `2`, `14`  
- `O valor é 1000 reais` → extrai `1000`  
- `123abc456` → extrai `123`, `456`  
- `Números: 7, 8, 9.` → extrai `7`, `8`, `9`

❌ Exemplos inválidos:  
- `abc` — não contém números  
- `!@#` — apenas símbolos  

---

## 🧠 Desafio Extra — Extrair números decimais

```regex
\d+(\.\d+)?
```

### 🔍 Explicação

- `\d+` captura a **parte inteira** do número  
- `(\.\d+)?` captura a **parte decimal**, se existir  
- O grupo `(\.\d+)?` é **opcional**, permitindo que a expressão funcione tanto com inteiros quanto com decimais  
- O ponto `.` precisa ser **escapado** com `\` para não ser interpretado como caractere curinga

✅ Exemplos válidos:  
- `O valor é 3.14` → extrai `3.14`  
- `Preço: 0.99 ou 100.0` → extrai `0.99`, `100.0`  
- `123 e 456.78` → extrai `123`, `456.78`

❌ Exemplos inválidos:  
- `abc` — não contém números  
- `3,14` — vírgula não é reconhecida como separador decimal  

---

- [Voltar ao Desafio 10](../desafios/desafio_10.md)  
- [Próximo desafio → Desafio 12](../desafios/desafio_12.md)

---

🔖 _Tags: regex, iniciante, números, extração, expressão regular_