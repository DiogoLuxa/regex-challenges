# ✅ Resposta — Desafio 01

### 🧩 Apenas Letras  
🔹 Nível: Iniciante  
🔹 Categoria: Validação Simples

---

## 🧪 Expressão Regular

```regex
^[A-Za-z]+$
```

---

## 🔍 Explicação

- `^` e `$` são âncoras que garantem que toda a string siga o padrão.  
- `[A-Za-z]` define o intervalo de letras maiúsculas e minúsculas.  
- `+` exige pelo menos uma letra (não aceita string vazia).

---

## 🧠 Desafio Extra — Com Acentos

```regex
^[A-Za-zÀ-ÿ]+$
```

🔍 Essa versão permite letras acentuadas e cedilha, mantendo a restrição contra números e símbolos.  
Inclui o intervalo Unicode `À-ÿ`, que cobre a maioria dos caracteres latinos acentuados.

---

#### 📎 [Voltar ao Desafio 01](../desafios/desafio_01.md)  
#### ➡️ [Próximo desafio → Desafio 02](../desafios/desafio_02.md)

🔖 _Tags: regex, iniciante, letras, acentos, validação, expressão regular_
