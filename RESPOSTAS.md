# Respostas do LAB 01

Nome: Bruno Gomes Santana
Matricula: Bruno 
Dupla (M2 em diante): Arthur Reis de Oliveira

---

## M2 - Quem quebrou o painel

**Hash curto do commit que introduziu o erro:**
01ef93bf 

**Autor:**
Tarcisio Melo 

**Data:**
2026-06-15 22:38:00
**Linha alterada (antes e depois):**

```
antes: return leitura * 9 / 5 + 32;
depois: return (leitura - 32) * 5 / 9
```

---

## M3 - O segredo vazado

**O que voce esperava ver no `git status` e o que apareceu:**

**Depois do push, alguem que clonar o repositorio ainda consegue ler a chave?
Responda em duas linhas, explicando o motivo:**

Eu eperava que eu precisasse atualizar o push e o commit, mas ele me mostrou outras partes do codigo que eu precisava atualizar.

As chaves permaneceram no historico do projeto. Com o gitignore voce apenas impediu o futuro versionamento dos arquivos nas proximas versoes, nas anteriores ele ainda permanece lá.

---

## M4 - Colisao

**O que significavam os marcadores que apareceram dentro do arquivo:**

- `<<<<<<<` : O sinal de menor que indica o incio do bloco de conflito e exibe a versão do codigo que estava na minha brach.
- `=======` : O sinal de igual separa as duas versoes do código, uma que esta tentando ser atualizada e a outra que esta ja presente no codigo.
- `>>>>>>>` :O sinal de maior indica a versão recebida ou o código que esta tentando alterar de um repositório remoto.


**Qual pedaco veio de quem, e qual titulo voces decidiram manter:**
Bruno: Painel Legal
Arthur: Jeff tubaraozinho
Decidimos manter a alteração do Arthur.
---

## Casa - Incidente na linha 3

**Hash do commit que quebrou o painel:**
84fbdd1

**Hash do commit de revert:**
ac6babe

**Por que `git revert` e nao `git reset` neste caso:**
O revert ele cria um commit novo desfazendo a alteração do commit selecionado, mantendo o historioco dos comit, sendo o ideal para projetos, ja o reset ele volta o projeto ao seu estado original e some com todo o historico.
