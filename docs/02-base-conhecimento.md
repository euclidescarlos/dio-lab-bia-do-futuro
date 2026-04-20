# Base de Conhecimento

## Dados Utilizados

Descreva se usou os arquivos da pasta `data`, por exemplo:

| Arquivo | Formato | O que o Jorge faz? |
|---------|---------|---------------------|
| `historico_atendimento.csv` | CSV | Contextualizar interações anteriores |
| `perfil_investidor.json` | JSON | Explica sobr eo mundo dos investimentos com base no perfil do usuário |
| `produtos_financeiros.json` | JSON | Exemplificar todos os investimentos para escolha do usuário |
| `transacoes.csv` | CSV | Analisar padrão de gastos do cliente para recomendações |


---

## Adaptações nos Dados

Os dados da pasta `data` não foram alterados.

---

## Estratégia de Integração

### Como os dados são carregados?
Os JSON/CSV são carregados no início da sessão e incluídos no contexto do prompt com python.

### Como os dados são usados no prompt?
> Os dados vão no system prompt? São consultados dinamicamente?

Quando o chat é aberto, o Jorge busca os dados do cliente e le todos eles para poder responder e entender qual o perfil do usuário.

---

## Exemplo de Contexto Montado
```
Dados do Cliente:
- Nome: João Silva
- Perfil: Moderado
- Saldo disponível: R$ 5.000

Últimas transações:
- 01/11: Supermercado - R$ 450
- 03/11: Streaming - R$ 55
...
```
