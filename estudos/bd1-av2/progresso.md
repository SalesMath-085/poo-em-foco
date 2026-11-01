# Checklist de estudos — AV2 Banco de Dados I

**Como usar:** marque `[x]` no lugar de `[ ]` quando concluir um assunto. O símbolo **★** sinaliza um tema sem questão direta na revisão ou com lacuna especialmente importante. Este arquivo é a fonte de dados do site de estudos. As marcações sincronizadas pelo site e as atualizações feitas neste arquivo representam o mesmo progresso.

## Aula 8 — Armazenamento
- [ ] Hierarquia de armazenamento: cache, RAM, HDD e SSD
- [ ] Diferenças de custo, capacidade e tempo de acesso
- [ ] Geometria de discos: pratos, trilhas, cilindros, setores e cabeçotes
- [ ] Endereçamento e mapeamento lógico dos blocos
- [ ] Tempo de acesso: seek, latência rotacional e transferência
- [ ] Cálculos de capacidade, taxa de transferência e tempo de acesso
- [ ] Acesso sequencial × acesso randômico
- [ ] ★ Memória flash e SSD: funcionamento, tipos e degradação
- [ ] ★ Comparação de desempenho SSD × HDD
- [ ] ★ Big Data e escalabilidade vertical × horizontal

## Aula 9 — Representação de Dados
- [ ] Diferença entre blocos, setores, registros e campos
- [ ] Registros de formato e tamanho fixos
- [ ] Registros de formato e tamanho variáveis
- [ ] Registros híbridos e campos repetidos
- [ ] Representação de valores NULL
- [ ] ★ BLOBs: armazenamento dentro e fora do banco
- [ ] Representação de inteiros, ponto flutuante, CHAR, VARCHAR e datas
- [ ] Separação de registros dentro de blocos
- [ ] Alocação espalhada × não espalhada
- [ ] Cálculo do tamanho dos registros, fator de bloco e desperdício
- [ ] Agrupamento e divisão de registros
- [ ] Buffer, buffer pool, frames e pinned blocks
- [ ] Reposição de páginas (LRU, CLOCK), páginas sujas e escrita
- [ ] Endereçamento de blocos e registros: referências físicas × indiretas
- [ ] Pointer swizzling
- [ ] Inserção e remoção física × lógica; tombstones

## Aula 10 — Organização de Arquivos
- [ ] Arquivos não ordenados (heap files)
- [ ] Arquivos ordenados (sequenciais)
- [ ] Comparação de custos de busca, inserção e remoção
- [ ] Hash estático: funções hash, buckets e colisões
- [ ] Overflow e encadeamento de blocos
- [ ] ★ Hash extensível: diretório e profundidades global e local
- [ ] ★ Split de buckets e expansão do diretório
- [ ] Ordenação externa: merge-sort de 2 vias
- [ ] Merge-sort externo multi-vias e cálculo de passagens

## Aula 11 — Indexação
- [ ] Índice primário, de cluster e secundário
- [ ] Índices densos × esparsos e âncoras de bloco
- [ ] Cálculos de entradas, fator de bloco e tamanho de índice
- [ ] Índices multinível: fan-out, altura e custo de busca
- [ ] Árvores de busca e propriedades de balanceamento
- [ ] Árvore-B: ordem, nós, chaves e ponteiros
- [ ] Árvore-B: busca e inserção, divisão de nós
- [ ] Árvore-B: remoção, redistribuição e fusão
- [ ] Árvore B+: estrutura de nós internos e folhas
- [ ] Árvore B+: busca por igualdade e intervalo
- [ ] Árvore B+: inserção e remoção
- [ ] Diferenças e vantagens entre árvores B e B+
- [ ] Ocupação, altura, custo e otimizações de árvores B+
- [ ] ★ Hash extensível aplicado à indexação

## Aula 12 — Processamento de Consultas
- [ ] SQL como linguagem declarativa e etapas do processamento
- [ ] Parser: análise sintática, semântica e permissões
- [ ] Catálogo do banco de dados e estatísticas
- [ ] Conversão de SQL para álgebra relacional
- [ ] Representação de consultas em árvores
- [ ] Otimizador e seleção de planos de execução
- [ ] Construção e comparação de planos equivalentes
- [ ] ★ SQL EXPLAIN: leitura e interpretação de planos

## Aula 13 — Otimização de Consultas
- [ ] Otimização heurística × baseada em custos
- [ ] Regras de comutatividade e associatividade
- [ ] Transformações de seleção e projeção
- [ ] Pushdown de seleções e projeções
- [ ] Reordenação de junções e equivalência de árvores
- [ ] Estatísticas: T(R), S(R), B(R) e V(R,A)
- [ ] Seletividade de predicados: igualdade e intervalos
- [ ] Estimativas de cardinalidade de seleção e junção
- [ ] Estimativas para produto cartesiano e expressões complexas
- [ ] Estimativa de custo de E/S e comparação entre planos
- [ ] ★ Programação dinâmica de Selinger

## Aula 14 — Execução de Consultas
- [ ] Seleção por varredura linear (file scan)
- [ ] Seleção por índices primários e secundários
- [ ] Seleções por igualdade, intervalo, AND, OR e índices compostos
- [ ] Algoritmos de seleção A1–A10 e comparação de custos
- [ ] Nested-loop join: execução e fórmulas de custo
- [ ] Block nested-loop join: buffers e custo
- [ ] Indexed nested-loop join: uso de índices e custo
- [ ] Merge-join / sort-merge join
- [ ] Hash-join: particionamento, memória e custo
- [ ] Comparação e escolha dos algoritmos de junção
- [ ] Algoritmos para eliminação de duplicatas
- [ ] Agregações: GROUP BY, COUNT e demais operações
- [ ] UNION, INTERSECTION e DIFFERENCE
- [ ] Materialização × pipelining

---

> Base: lista específica da AV2, slides de BD e 83 questões de revisão. Transações (aula 15) não estão incluídas na lista específica informada.