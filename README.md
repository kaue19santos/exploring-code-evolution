# Explorando evolução de código

Neste exercício, iremos explorar a evolução de código em sistemas reais.

Iremos utilizar a ferramenta [GitEvo](https://github.com/andrehora/gitevo).
Essa ferramenta analisa a evolução de código em repositórios Git nas linguagens Python, JavaScript, TypeScript e Java, e gera relatórios `HTML` como [este](https://andrehora.github.io/gitevo-examples/python/pandas.html).

Mais exemplos de relatórios podem ser podem ser encontrados em https://github.com/andrehora/gitevo-examples.

# Passo 1: Selecionar repositório a ser analisado

Selecione um repositório relevante na linguagem de sua preferência (Python, JavaScript, TypeScript ou Java).
Você pode encontrar projetos interessantes nos links abaixo:

- Python: https://github.com/topics/python?l=python
- JavaScript: https://github.com/topics/javascript?l=javascript
- TypeScript: https://github.com/topics/typescript?l=typescript
- Java: https://github.com/topics/java?l=java

# Passo 2: Instalar e rodar a ferramenta GitEvo

> [!NOTE]
> Antes de instalar a ferramenta, é recomendado criar e ativar um [ambiente virtual Python](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/#create-and-use-virtual-environments).

Instale a ferramenta [GitEvo](https://github.com/andrehora/gitevo) com o comando:

```
$ pip install gitevo
```

Execute a ferramenta no repositório selecionado utilizando o comando abaixo (ajuste conforme a linguagem do repositório).
Substitua `<git_url>` pela URL do repositório que será analisado:

```shell
# Python
$ gitevo -r python <git_url>

# JavaScript
$ gitevo -r javascript <git_url>

# TypeScript
$ gitevo -r typescript <git_url>

# Java
$ gitevo -r java <git_url>
```

Por exemplo, para analisar o projeto Flask escrito em Python:

```
$ gitevo -r python https://github.com/pallets/flask
```

> [!NOTE]
> Essa etapa pode demorar alguns minutos pois o projeto será clonado e analisado localmente.

# Passo 3: Explorar o relatório de evolução de código

Após executar a ferramenta [GitEvo](https://github.com/andrehora/gitevo), é gerado um relatório `HTML` contendo diversos gráficos sobre a evolução do código.

Abra o relatório `HTML` e observe com atenção os gráficos.

# Passo 4: Explicar um gráfico de evolução de código

Selecione um dos gráficos de evolução e explique-o com suas palavras.
Por exemplo, você pode:

- Detalhar a evolução ao longo do tempo
- Detalhar se as curvas estão de acordo com boas práticas
- Explicar grandes alterações nas curvas
- Explorar a documentação do repositório em busca de explicações para grandes alterações
- etc.

Seja criativo!

# Instruções para o exercício

1. Crie um `fork` deste repositório (mais informações sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Adicione o relatório `HTML` no seu fork.
3. No Moodle, submeta apenas a URL do seu `fork`.

Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork:

1. Repositório selecionado: https://github.com/angular/angular
2. Gráfico selecionado: <img width="719" height="347" alt="Screenshot 2026-11-06 at 21 10 22" src="https://github.com/user-attachments/assets/2512af84-c9ed-4892-8f73-b1c06c6a4587" />
3. Explicação: O gráfico apresenta a evolução da média de linhas de código por arquivo TypeScript no projeto Angular, entre 2021 e 2026. É possível observar um crescimento moderado entre 2021 e 2023, seguido por uma redução em 2024. Entretanto, a partir de 2025, ocorre um aumento expressivo, passando de aproximadamente 118 para 179 linhas por arquivo em 2026, representando um crescimento de aproximadamente 51% em relação a 2024. Esse comportamento pode ser analisado considerando o contexto de transformação das ferramentas de desenvolvimento. A partir de 2021, ferramentas como GitHub Copilot começaram a popularizar a geração automática de código. Posteriormente, com a chegada do ChatGPT, do GitHub Copilot Chat e de ferramentas mais avançadas, como Claude Code, a utilização de inteligência artificial no desenvolvimento de software ganhou novas possibilidades. É interessante observar que o crescimento mais expressivo da média de linhas por arquivo acontece justamente durante esse período de popularização das ferramentas de IA generativa. Isso levanta a hipótese de que a evolução dessas ferramentas possa ter influenciado a produtividade e a maneira como o código é produzido. Entretanto, não é possível estabelecer uma relação direta de causalidade entre esses acontecimentos e os dados apresentados. O crescimento também pode estar relacionado a novas funcionalidades, refatorações, mudanças arquiteturais e outras decisões tomadas pela equipe de desenvolvimento do Angular.



