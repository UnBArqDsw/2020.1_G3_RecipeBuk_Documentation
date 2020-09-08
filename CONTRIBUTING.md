# Políticas de Contribuição

## Commits

- Os _Commits_ devem ser escritos em inglês;

- Devem ser curtos e objetivos;

- Devem iniciar com verbo no passado;

- Devem ser compostos por:

```
    [#numero-da-issue] Mensagem
```

### Exemplo:

```
    [#20] Implemented new text box
```

## Branches

As _branchs_ são baseadas no modelo de GitFlow e são dividas em:

- `master`: aplicação em sua versão estável;
- `dev`: versão de desenvolvimento que servirá como base para as demais _branches_.


Para a criação de uma nova _branch_, deve-se criá-la a partir da `dev` e manter o seguinte padrão:

- Os nomes das _branches_ deverão ser compostos por:

```
        numero-da-issue-nome-da-issue
```

### Exemplo:

```
        20-criacao-da-tela-de-cadastro-de-receitas
```


## Pull Requests

- Os PRs devem ser criados a partir do **template** do repositório;

- Os PRs devem englobar as modificações necessárias para **apenas** uma _issue_;

- O _merge_ das _branches_ criadas a partir da `dev` **nunca** deverá ser feito na `master`;

- Após o _merge_, se a _branch_ não tiver mais uso, ela deverá ser **apagada**