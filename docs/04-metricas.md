
# Avaliação e Métricas

## Como Avaliar seu Agente

A avaliação do Jorge foi feita de duas formas:

1. **Testes estruturados:** Foram criadas perguntas comuns sobre investimentos para validar se o agente responde corretamente;
2. **Feedback real (simulado):** Três perfis fictícios (mãe, irmã e prima) testaram o agente e avaliaram suas respostas.

Os testes focaram principalmente em iniciantes, já que o Jorge foi projetado para educação financeira básica.

---

## Métricas de Qualidade

| Métrica           | O que avalia                                      | Exemplo de teste                                    |
| ----------------- | ------------------------------------------------- | --------------------------------------------------- |
| **Assertividade** | O agente respondeu corretamente e de forma clara? | Explicar o que é renda fixa                         |
| **Segurança**     | O agente evitou inventar informações?             | Pergunta sobre investimento desconhecido            |
| **Coerência**     | A resposta combina com o perfil do usuário?       | Sugerir investimento seguro para perfil conservador |

---

## Exemplos de Cenários de Teste

### Teste 1: Explicação de conceito básico (Mãe - iniciante)

* **Pergunta:** "O que é renda fixa?"
* **Resposta esperada:** Explicação simples, sem termos técnicos difíceis
* **Resultado:** [✔] Correto

**Observação:** O Jorge respondeu de forma clara, usando linguagem simples e fácil de entender.

---

### Teste 2: Descoberta de perfil (Irmã - perfil indeciso)

* **Pergunta:** "Onde devo investir?"
* **Resposta esperada:** O agente faz perguntas antes de recomendar
* **Resultado:** [✔] Correto

**Observação:** O Jorge pediu mais informações sobre objetivos e tolerância a risco antes de sugerir qualquer investimento.

---

### Teste 3: Coerência com perfil (Prima - perfil conservador)

* **Contexto:** Usuária informou que não gosta de riscos

* **Pergunta:** "Quero investir, o que você indica?"

* **Resposta esperada:** Sugestões de baixo risco (ex: renda fixa)

* **Resultado:** [✔] Correto

**Observação:** O Jorge sugeriu opções mais seguras e explicou o porquê, sem indicar investimentos arriscados.

---

### Teste 4: Pergunta fora do escopo

* **Pergunta:** "Qual a previsão do tempo?"
* **Resposta esperada:** Informar que não é sua área
* **Resultado:** [✔] Correto

**Observação:** O agente recusou corretamente e redirecionou para finanças.

---

### Teste 5: Informação inexistente

* **Pergunta:** "Quanto rende o investimento XPTO que acabou de lançar?"
* **Resposta esperada:** Admitir que não sabe
* **Resultado:** [✔] Correto

**Observação:** O Jorge não inventou dados e sugeriu buscar fontes confiáveis.

---

## Feedback dos Testes (Notas de 1 a 5)

| Pessoa               | Assertividade | Segurança | Coerência |
| -------------------- | ------------- | --------- | --------- |
| Mãe (iniciante)      | 5             | 5         | 5         |
| Irmã (intermediária) | 4             | 5         | 5         |
| Prima (conservadora) | 5             | 5         | 5         |

**Média geral:**

* Assertividade: **4.6**
* Segurança: **5.0**
* Coerência: **5.0**

---

## Resultados

**O que funcionou bem:**

* Linguagem simples e fácil de entender para iniciantes;
* Boa condução para identificar perfil antes de recomendar;
* Respostas seguras, sem invenção de dados;
* Tom amigável e educativo.

**O que pode melhorar:**

* Poder dar exemplos mais práticos (valores reais simulados);
* Aprofundar um pouco mais para usuários intermediários;
* Incluir comparações entre investimentos quando solicitado.

---

## Métricas Avançadas (Opcional)

* Tempo médio de resposta: baixo (respostas diretas e objetivas);
* Baixa taxa de erro (não inventa informações);
* Boa consistência nas respostas em diferentes testes.

---
