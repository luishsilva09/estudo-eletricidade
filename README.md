# Estudo de Eletricidade

Página única (HTML + JavaScript, sem dependências) para estudar e testar cálculos de eletricidade básica.

## Abas

- **1ª Lei de Ohm:** V = R · I e potência (P = V · I). Preencha dois campos e a página acha os outros dois.
- **2ª Lei de Ohm (resistividade):** R = ρ · L / A, com correção por temperatura. Inclui tabela de materiais.
- **Queda de tensão:** ΔV = k · ρ(T) · L · I / S, com seção mínima para o limite escolhido.
- **Equivalente:** resistência equivalente em série e em paralelo, com desenhos e fórmulas de atalho.
- **Circuito:** grade para montar um circuito de resistores (com diagonais e fios) entre A e B, e animação passo a passo da redução por série e paralelo até a resistência equivalente. Na animação, o circuito aparece ampliado e uma lousa ao lado vai escrevendo as contas de cada passo. Pontes que não reduzem são resolvidas por análise nodal. Se você informar a tensão entre A e B, depois da Req a animação volta ao circuito original: corrente total, tensão em cada nó, corrente (com sentido) em cada resistor e a verificação das leis de Kirchhoff, a 1ª em cada nó com 3 ou mais ligações e a 2ª em cada laço independente (laços = ramos − nós + 1, contando a fonte A–B). Também funciona na ponte de Wheatstone. Com a ferramenta Fonte dá para colocar fontes de tensão na grade (com polaridade); aí A e B deixam de ser usados e a animação resolve o circuito pelas leis de Kirchhoff: nós e referência, correntes de malha com a 2ª lei em cada malha, sistema pela regra de Cramer (até 3 incógnitas), corrente em cada ramo, tensão em cada nó, conferência das duas leis e balanço de potência. Voltas só de fontes, fonte em curto e circuito sem caminho fechado são avisados. Tem desfazer/refazer, troca do número dos resistores e das fontes (R1 ↔ R2, E1 ↔ E2), atalhos de teclado e tela cheia para dar aula. O circuito fica salvo no navegador.
- **Notação:** operações em notação científica e conversão de prefixos (T, G, M, k, m, µ, n, p).
- **Matemática:** contas com frações (soma, subtração, multiplicação e divisão, com simplificação), regra de três direta e inversa e porcentagem.

As divisões aparecem como fração empilhada (numerador em cima, denominador embaixo).

Cada aba traz fórmula, legenda dos símbolos, explicação, exemplo resolvido e exercícios com resposta antes da calculadora.

Os campos aceitam prefixos: `4k7` ou `4,7k` = 4.700, `250m` = 0,25, `10µ` = 0,00001, `2M` = 2.000.000 (m minúsculo é mili, M maiúsculo é mega).

## Como usar

Abra o `index.html` no navegador. As fontes vêm do Google Fonts; sem internet a página usa fontes do sistema.

## Observações

- Cobre e alumínio usam ρ e α de uma tabela de livro didático (cobre 0,0173 e 0,004; alumínio 0,0278 e 0,0032). Os demais materiais são valores típicos a 20 °C e variam com pureza e liga.
- A queda de tensão é um cálculo resistivo simples, sem reatância nem fator de potência. Confirme limites e seções no projeto e na NBR 5410.
