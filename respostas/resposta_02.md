# ✅ Resposta — Desafio 02

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Apenas Números  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
^\d+$
```

---

## 🔍 Explicação

- `^` e `$` são âncoras que garantem que toda a string siga o padrão.  
- `[0-9]` define o intervalo de dígitos de 0 a 9.  
- `+` exige pelo menos um dígito (não aceita string vazia).

---

## 🧠 Desafio Extra — Números Decimais

```regex
^\d+([.,]\d+)?$
```

🔍 Essa versão permite números com ponto ou vírgula decimal.  
A parte decimal é opcional, mas se presente, deve vir após um número inteiro.

✅ Exemplos válidos: `12.34`, `0,99`, `100`  
❌ Exemplos inválidos: `12..34`, `,99`, `.`

---

- [Voltar ao Desafio 02](../desafios/desafio_02.md)  
- [Próximo desafio → Desafio 03](../desafios/desafio_03.md)

🔖 _Tags: regex, iniciante, números, decimais, validação, expressão regular_
