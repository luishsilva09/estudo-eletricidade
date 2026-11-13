# Estudo de Eletricidade

Página única (HTML + JavaScript, sem dependências) para estudar e testar cálculos de eletricidade básica.

## Abas

- **1ª Lei de Ohm:** V = R · I e potência (P = V · I). Preencha dois campos e a página acha os outros dois.
- **2ª Lei de Ohm (resistividade):** R = ρ · L / A, com correção por temperatura. Inclui tabela de materiais.
- **Queda de tensão:** ΔV = k · ρ(T) · L · I / S, com seção mínima para o limite escolhido.
- **Equivalente:** resistência equivalente em série e em paralelo, com desenhos e fórmulas de atalho.
- **Notação:** operações em notação científica e conversão de prefixos (T, G, M, k, m, µ, n, p).

Cada aba traz fórmula, legenda dos símbolos, explicação, exemplo resolvido e exercícios com resposta antes da calculadora.

Os campos aceitam prefixos: `4k7` ou `4,7k` = 4.700, `250m` = 0,25, `10µ` = 0,00001, `2M` = 2.000.000 (m minúsculo é mili, M maiúsculo é mega).

## Como usar

Abra o `index.html` no navegador. As fontes vêm do Google Fonts; sem internet a página usa fontes do sistema.

## Observações

- Cobre e alumínio usam ρ e α de uma tabela de livro didático (cobre 0,0173 e 0,004; alumínio 0,0278 e 0,0032). Os demais materiais são valores típicos a 20 °C e variam com pureza e liga.
- A queda de tensão é um cálculo resistivo simples, sem reatância nem fator de potência. Confirme limites e seções no projeto e na NBR 5410.
