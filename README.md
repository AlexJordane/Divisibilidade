# Investigando Critérios de Divisibilidade

Material didático e investigativo elaborado para o curso de **Licenciatura em Matemática** do **Instituto Federal do Espírito Santo (Ifes)**, voltado para a compreensão estrutural dos números naturais por meio dos **Critérios de Divisibilidade**.

Mais do que apresentar regras para memorização, o texto prioriza a **demonstração e a justificativa algébrica** dos processos matemáticos que fundamentam cada procedimento de verificação, utilizando diferentes representações polinomiais na base 10.

## Links de Acesso

- **Página do Projeto (GitHub Pages):** https://alexjordane.github.io/Divisibilidade/
- **Documento em PDF:** [Divisibilidade.pdf](./Divisibilidade.pdf)
- **Código-fonte LaTeX:** [Divisibilidade.tex](./Divisibilidade.tex)
- **Repositório no GitHub:** https://github.com/AlexJordane/Divisibilidade

---

## Estrutura do Material

### Introdução — Notações de Números Inteiros na Base 10
Estabelece três formas de decompor algebricamente um número inteiro $N$ para facilitar as demonstrações:
- **1ª Notação (Expansão decimal completa):** $N = 1000a + 100b + 10c + d$.
- **2ª Notação (Isolamento do algarismo das unidades):** $N = 10a + b$.
- **3ª Notação (Isolamento dos últimos algarismos):** $N = 100a + b$, $N = 1000a + b$, e generalizações para $10^x \cdot a + b$.

### 1. Procedimentos pela Posição
Analisa os critérios que dependem apenas dos últimos algarismos do número:
- **Divisibilidade por 2 e por 5:** Justificativa a partir de $N = 10a + b$.
- **Divisibilidade por múltiplos e potências de 2 e de 5:** Critérios para $10$ ($2 \cdot 5$), $4$ ($2^2$), $8$ ($2^3$), potências de base dez ($10^x$) e potências de base dois ($2^x$).

### 2. Procedimentos pela Soma de Algarismos
Demonstra os critérios de divisibilidade por **3** e por **9** decompondo as potências de 10 na forma $999a + 99b + 9c + (a + b + c + d)$:
$$N = 9 \cdot (111a + 11b + c) + (a + b + c + d)$$

### 3. Procedimentos por Decomposição ($p_m = a + k \cdot b$)
Desenvolve um método geral baseado em $N = 10a + b$ para números primos que não dividem potências de 10, encontrando o multiplicador adequado $k$ por meio de múltiplos que terminam em $1$ ou $9$:
- **Divisibilidade por 7 ($k = -2$):** $p_7 = a - 2b$ (via $N = 10(a - 2b) + 21b$).
- **Divisibilidade por 13 ($k = 4$):** $p_{13} = a + 4b$ (via $N = 10(a + 4b) - 39b$).
- **Divisibilidade por 17 ($k = -5$):** $p_{17} = a - 5b$ (via $N = 10(a - 5b) + 51b$).
- **Divisibilidade por 19 ($k = 2$):** $p_{19} = a + 2b$ (via $N = 10(a + 2b) - 19b$).
- **Extensão para primos maiores (ex.: 23, com $k = -16$):** $p_{23} = a - 16b$ (via $23 \cdot 7 = 161$).

### 4. A Soma Alternada (Divisibilidade por 11)
Aborda a divisibilidade por **11** sob duas perspectivas complementares:
1. **Por decomposição:** $p_{11} = a - b$ (via $N = 10(a - b) + 11b$).
2. **Pela soma alternada das ordens:** Explorando a proximidade das potências de 10 em relação aos múltiplos de 11 ($10 = 11 - 1$, $100 = 99 + 1$, $1000 = 1001 - 1$, $\dots$), justificando a regra prática de somar e subtrair alternadamente os algarismos ($a - b + c - d \dots$).

---

## Como Compilar o Código LaTeX

Para gerar o PDF a partir do arquivo `Divisibilidade.tex`, utilize uma distribuição LaTeX (TeX Live, MiKTeX ou Overleaf):

```bash
pdflatex Divisibilidade.tex
pdflatex Divisibilidade.tex
```

---

## Autoria e Licença

- **Autor:** Professor Alex Jordane (Instituto Federal do Espírito Santo — Licenciatura em Matemática • Educimat), em colaboração com Inteligência Artificial (Gemini 3.1 Pro).
- **Licença:** Esta obra está licenciada sob uma Licença **Creative Commons Atribuição-NãoComercial-SemDerivações 4.0 Internacional (CC BY-NC-ND 4.0)**. O compartilhamento e a reprodução deste material são permitidos para fins didáticos, desde que citadas a fonte e a autoria.
