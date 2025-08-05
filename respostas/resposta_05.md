# ✅ Resposta — Desafio 05

- [Voltar ao Sumário](../SUMARIO.md)  

### 🧩 Termina com "fim"  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
/fim$/
```

---

## 🔍 Explicação

- `fim` é a palavra exata que queremos validar no final da string  
- `$` é a âncora que garante que "fim" esteja **no final** da string  
- Não há modificadores, então a validação é **case-sensitive**  
- Não permite letras, números ou símbolos após "fim"  
- Permite qualquer conteúdo antes de "fim", desde que "fim" seja a última palavra

---

## 🧠 Desafio Extra — Aceitar variações de maiúsculas/minúsculas

```regex
/fim$/i
```

🔍 Essa versão usa o modificador `/i` para tornar a expressão **case-insensitive**, permitindo:

✅ Exemplos válidos:  
- `fim`  
- `Fim`  
- `chegamos ao FIM`  
- `o grande fIm`

❌ Exemplos inválidos:  
- `fim!` — contém símbolo após "fim"  
- `fim123` — contém números após "fim"  
- `fim de tudo` — "fim" não está no final  
- `` — string vazia

---

- [Voltar ao Desafio 05](../desafios/desafio_05.md)  
- [Próximo desafio → Desafio 06](../desafios/desafio_06.md)

---

🔖 _Tags: regex, iniciante, fim, encerramento, validação, expressão regular_
