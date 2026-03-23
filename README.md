# King's Throne - Hero Strategy Calculator 👑

Este é um projeto de uso estritamente **pessoal** desenvolvido como ferramenta de apoio para um hobby: o jogo King's Throne. O objetivo principal é automatizar cálculos complexos de progressão de atributos (Kingdom Power) para heróis específicos, facilitando a tomada 
de decisão estratégica sobre investimentos de recursos.

## 🚀 Funcionalidades

A calculadora foi estruturada para refletir fielmente as mecânicas de cálculo do jogo, dividindo as operações em quatro pilares fundamentais (Military, Fortune, Provisions e Inspiration).

### 1. Cálculo de Atributos em Tempo Real
- **Quality Bonus:** Aplica a fórmula quadrática baseada no nível do herói:  
  `0.1 * (Base Quality + Beast Skill Quality) * (Level² + Level + 98)`
- **Soma Modular:** Consolida bônus de Tomos (Tomes), Vínculos (Bonds), Feras (Beasts), Equipamentos e Artefatos de forma independente para cada atributo.

### 2. Projeção de Nível (Level Up)
- Permite prever o ganho de poder bruto ao elevar um herói de um nível `X` para um nível `Y`.
- Utiliza a **Qualidade Total** informada pelo usuário para entregar uma estimativa de crescimento global de atributos.

### 3. Projeção de Upgrade de Paragon (Flexível)
- Calcula o impacto percentual de melhorias de Paragon.
- **Lógica de Escopo:** O usuário pode selecionar quais atributos serão afetados pelo upgrade (Ex: apenas Military, ou Military + Fortune).
- **Precisão Matemática:** Multiplica apenas a base permitida (Quality + Tome + Bond), excluindo bônus fixos que não escalam com Paragon, como Equipamentos e Artefatos.

## 🛠️ Tecnologias Utilizadas

- **HTML5 & CSS3:** Interface limpa e funcional projetada para uso rápido durante o gameplay.
- **JavaScript (Vanilla):** Lógica de processamento de dados e tratamento de strings (conversão automática de sufixos numéricos K, M, B e normalização de separadores decimais).

## 📝 Nota de Desenvolvimento

Este projeto foi desenvolvido utilizando assistência de Inteligência Artificial para a codificação da lógica matemática e estruturação do front-end, visando otimizar o tempo de desenvolvimento para um projeto de uso particular. 

O foco principal foi a **utilidade prática** e a **precisão dos dados**, garantindo uma margem de erro mínima (aproximadamente 0,01%) em relação aos valores exibidos nos servidores oficiais do jogo.

---
**Disclaimer:** Este software não possui fins lucrativos e não realiza modificações nos arquivos do jogo ou interações diretas com servidores. É apenas uma ferramenta de cálculo externa.
