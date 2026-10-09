# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

Mais detalhes no GitHub da ferramenta: https://github.com/andrehora/testminer.

---

## Passo 1: Selecionar DOIS repositórios

Escolha dois repositórios reais que possuam testes de software.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

- Tópicos: [ai](https://andrehora.github.io/testminer/#topic:ai), [llm](https://andrehora.github.io/testminer/#topic:llm), [api](https://andrehora.github.io/testminer/#topic:api), [nodejs](https://andrehora.github.io/testminer/#topic:nodejs), [android](https://andrehora.github.io/testminer/#topic:android)

- Por organização: [Google](https://andrehora.github.io/testminer/#google), [Microsoft](https://andrehora.github.io/testminer/#microsoft), [Apple](https://andrehora.github.io/testminer/#apple), [Facebook](https://andrehora.github.io/testminer/#facebook), [Netflix](https://andrehora.github.io/testminer/#netflix), 
[GitHub](https://andrehora.github.io/testminer/#github), [Apache](https://andrehora.github.io/testminer/#apache), [HuggingFace](https://andrehora.github.io/testminer/#huggingface)

## Passo 2: Explorar os repositórios selecionados

Busque os repositórios escolhidos no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar as prática de teste

Para cada repositório, escolha uma prática ou dado de teste relevante e explique com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

### Repositório 1 

Repositório: https://github.com/mockito/mockito

URL TestMiner: https://andrehora.github.io/testminer/#mockito/mockito

Explicação:

**Prática: testes de regressão**

No TestMiner, aumentando a profundidade na seção *Test Location*, dá para ver que o maior subpacote de testes se chama `bugs`, com 34 arquivos.

Cada teste desse pacote reproduz um bug que já foi encontrado e corrigido, e o nome da classe descreve o problema, como [`NPEWhenMockingThrowablesTest`](https://github.com/mockito/mockito/blob/main/mockito-core/src/test/java/org/mockitousage/bugs/NPEWhenMockingThrowablesTest.java). Vários deles também têm um comentário com o número da issue.

A ideia central dos testes de regressão é que, se alguém mexer no código no futuro e o bug voltar, o teste falha e avisa na hora. Assim, um comportamento que já foi corrigido não volta a quebrar sem ninguém perceber.

**Dado relevante: quantidade de *mocks***

O TestMiner mostra 184 arquivos como *mocks*. No entanto, a ferramenta classifica como mock qualquer arquivo de teste que tenha "mock" no nome, o que acontece com quase todo teste do Mockito.

### Repositório 2

Repositório: `<URL_DO_REPOSITÓRIO>`

URL TestMiner: `<URL_NO_TESTMINER>`

Explicação: `<SUA_EXPLICAÇÃO>`
