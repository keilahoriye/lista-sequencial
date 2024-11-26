# Atividade lista-sequencial
O objetivo da atividade é implementar o redimensionamento dinâmico em uma lista sequencial ordenada (previamente fornecida para ser usada, se for interessante) em C ou C++.
A lista deve ser capaz de expandir ou reduzir seu tamanho automaticamente conforme os elementos são inseridos ou removidos.

## Requisitos específicos:
- A lista deve ter inicialmente capacidade de 50 elementos.
- Quando a capacidade máxima for atingida, o tamanho da lista deve ser duplicado utilizando alocação dinâmica de memória.
- Quando o número de elementos cair para 25% da capacidade, o tamanho da lista deve ser reduzido pela metade para economizar memória.

### Funções implementadas:
- resize: para dobrar o tamanho da lista quando atingir a capacidade e para reduzir o tamanho pela metade quando o número de elementos cair para 25% da capacidade.
- realloc: para redimensionar o vetor de forma dinâmica, alterando sua capacidade para o novo tamanho desejado sem perder os dados já armazenados (utilizada dentro de resize)

### Outras mudanças realizadas:
- Usuário pode interagir com o código, dizendo quantos elementos quer inserir e quantos quer excluir. Dessa forma, é possível ver o código dinamicamente alocando memória conforme o necessário.
- Foram priorizadas a busca binária e a possibilidade de inserir elementos repetidos.
- Ao final, a lista é reiniciada, zerando tudo o que foi feito, para liberar espaço.
