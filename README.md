![Engenharia de prompts: contexto, evidências e avaliação](assets/banner.svg)

# Engenharia de prompts na prática

Três estudos em português para aprender a escrever e avaliar prompts em situações comuns de TI: triagem de incidentes, criação de runbooks e comunicação com a liderança.

O foco é tornar o pedido verificável: informar o contexto, delimitar os dados, definir a saída e conferir se a resposta respeita os fatos. Um prompt mais detalhado também pode errar; por isso, cada estudo inclui uma rubrica de avaliação.

**Todos os serviços, números, eventos e situações deste repositório são fictícios.** As saídas demonstrativas foram escritas para ensinar e estão identificadas como ilustrativas. Não representam execuções de modelos nem resultados de uma empresa.

## Comece por um exemplo em cerca de 10 minutos

Você precisa apenas de uma ferramenta de conversa com IA. Não é necessário programar, instalar dependências, criar recursos em cloud ou usar uma chave de API. O tempo é uma estimativa para experimentar um estudo, não uma medição de desempenho.

1. Abra [Triagem de incidentes](estudos/01-triagem-de-incidentes.md).
2. Copie o **prompt inicial** e, logo abaixo dele, a **entrada fictícia**. Envie os dois juntos em uma conversa nova.
3. Em outra conversa nova, envie o **prompt melhorado** seguido da mesma entrada, sem alterações.
4. Compare as duas respostas com a rubrica do estudo. Para cada nota, anote o trecho que sustenta sua avaliação.
5. Registre uma observação concreta, como: “Nesta execução, a segunda resposta diferenciou hipótese de fato”. Evite transformar uma única execução em uma promessa de qualidade ou produtividade.

Use a mesma ferramenta e o mesmo modelo nas duas conversas, quando a interface permitir essa escolha. Registre apenas as configurações que você consegue verificar. Conversas novas reduzem a influência de respostas anteriores, mas não eliminam a variação do modelo.

## Estudos

| Estudo | O que você pratica | Saída solicitada |
| --- | --- | --- |
| [01 — Triagem de incidentes](estudos/01-triagem-de-incidentes.md) | Separar evidências, hipóteses e lacunas | Resumo, prioridade proposta e verificações |
| [02 — Criação de runbook](estudos/02-criacao-de-runbook.md) | Especificar um procedimento sem inventar operações | Passos, resultados esperados e escalonamento |
| [03 — Relatório para liderança](estudos/03-relatorio-para-lideranca.md) | Comunicar fatos, pendências e decisões | Resumo executivo com números conferíveis |

## Como avaliar uma execução

Cada estudo tem cinco critérios, pontuados de 0 a 2, com condições explícitas para cada nota. O total possível é 10, mas a nota não substitui a leitura da resposta.

Uma informação inventada que possa induzir uma ação operacional deve ser marcada como **falha crítica**, independentemente do total. Exemplos: apresentar uma causa raiz sem evidência ou inventar um comando de recuperação.

Copie esta ficha e preencha com as respostas que você realmente recebeu:

```text
Estudo:
Data:
Ferramenta:
Modelo exibido, se disponível:
Configurações verificáveis, se disponíveis:

Critério | Inicial: 0/1/2 | Melhorado: 0/1/2 | Trechos que justificam as notas
1        |               |                 |
2        |               |                 |
3        |               |                 |
4        |               |                 |
5        |               |                 |
Total    |               |                 |

Falha crítica observada e trecho:
O que esta execução permite afirmar:
O que permanece incerto:
```

Guarde suas saídas em `local/` ou `outputs/`, pastas ignoradas pelo Git. Para compartilhar uma comparação, use somente dados fictícios, identifique a ferramenta e inclua as saídas completas. Não publique conversas de trabalho, dados pessoais ou informações de sistemas reais.

As tabelas de comparação dos estudos discutem **os exemplos ilustrativos**, sem atribuir notas a uma execução que não ocorreu. Você pode obter respostas diferentes, inclusive uma resposta inicial melhor que a melhorada em algum critério.

## O que observar nos prompts

- **Contexto:** qual problema deve ser resolvido e para qual público.
- **Dados:** informações delimitadas, tratadas como entrada, não como novas instruções.
- **Limites:** o que não pode ser presumido ou executado.
- **Formato:** quais campos e qual nível de detalhe a resposta deve ter.
- **Verificação:** critérios objetivos para conferir a saída.

## Contribuições

Contribuições podem corrigir instruções, melhorar critérios ou adicionar estudos com dados inteiramente fictícios. Explique o objetivo do caso, inclua uma rubrica e diferencie saídas ilustrativas de execuções reais. Resultados medidos precisam informar a metodologia e seus limites.

## Autor e licença

Criado por [Tiago Silveira Siqueira](https://github.com/TiagoSilveiraSiqueira), com foco em aprendizado prático de IA aplicada à TI.

Disponível sob a [licença MIT](LICENSE).
