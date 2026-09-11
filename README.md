# IC

Repositório de materiais, ferramentas e experimentos desenvolvidos durante atividades de iniciação científica e projetos acadêmicos.

## Conteúdo

| Pasta | Descrição |
| --- | --- |
| [`Banco_de_questoes`](./Banco_de_questoes) | Banco de questões e provas, com destaque para materiais do POSCOMP. |
| [`Feedbacks`](./Feedbacks) | Relatórios e documentos de feedback de atividades e avaliações. |
| [`HTML`](./HTML) | Avaliadores e protótipos desenvolvidos em HTML e LaTeX. |
| [`PYTHON`](./PYTHON) | Ferramentas Python para processar questões e avaliar respostas de modelos de linguagem. |

## Avaliação de questões com IA

O diretório [`PYTHON`](./PYTHON) contém uma ferramenta que:

- lê questões de múltipla escolha em LaTeX;
- remove as marcações das respostas corretas;
- embaralha as alternativas para evitar padrões previsíveis;
- envia as questões para um modelo de linguagem;
- compara as respostas recebidas com o gabarito;
- calcula uma pontuação, inclusive para questões com múltiplas alternativas corretas.

Consulte a [documentação completa do avaliador](./PYTHON/README.md) para conhecer o formato das questões, as configurações e os comandos disponíveis.

### Execução rápida

Entre no diretório principal da ferramenta:

```bash
cd PYTHON/Main
```

Configure a chave da API e o modelo utilizado no arquivo `Main.py`. Depois, execute:

```bash
python Main.py \
  --caminho_testes caminho/para/as/questoes \
  --instrucao caminho/para/instrucao.tex
```

Também é possível executar a ferramenta sem argumentos, utilizando os caminhos padrão definidos no projeto:

```bash
python Main.py
```

> **Importante:** nunca publique chaves de API no repositório. Prefira variáveis de ambiente ou um arquivo local que esteja listado no `.gitignore`.

## Banco de questões

O material do POSCOMP está organizado por ano e inclui cadernos de prova, gabaritos e arquivos auxiliares. Para mais detalhes, consulte o [README do banco de questões](./Banco_de_questoes/POSCOMP/Provas_Poscomp%282004-2025%29/README.md).

## Tecnologias

- Python
- LaTeX
- HTML
- Modelos de linguagem

## Organização do projeto

Este repositório reúne materiais de pesquisa, documentos de apoio e código experimental. Alguns arquivos gerados por compiladores e ferramentas acadêmicas são mantidos junto dos projetos para facilitar a reprodução dos resultados.

## Licença

Nenhuma licença específica foi definida para este repositório. Consulte o autor antes de reutilizar código, documentos ou materiais.
