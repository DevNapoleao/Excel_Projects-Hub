# BABU | Simulador de Investimentos em FIIs

![Visão geral do projeto](imagens/painel.png)

Planilha em Excel para **planejar, simular e acompanhar investimentos em Fundos Imobiliários (FIIs)**. Com poucas informações, ela mostra quanto patrimônio você pode acumular e quanto pode receber de dividendos por mês em diferentes horizontes de tempo.

> Projeto de **educação financeira**. Os resultados são simulações e **não são recomendação de investimento**.

---

## O que o projeto faz

- **Configurações:** você informa salário, percentual do salário que será investido e rendimento mensal esperado da carteira.
- **Investimento mensal:** calcula o valor aportado por mês, o patrimônio acumulado no prazo escolhido e os dividendos mensais estimados.
- **Cenários:** projeta o resultado em 2, 5, 10, 20 e 30 anos.
- **Perfil e distribuição de FIIs:** divide o aporte mensal entre tipos de fundos (papel, tijolo, híbridos, FoFs, desenvolvimento, entre outros), com gráfico em rosca.

## Como usar

1. Baixe o arquivo `.xlsx` deste repositório.
2. Abra no Microsoft Excel.
3. Altere apenas as células em **verde-água** (salário, percentuais, anos, perfil e % de cada tipo de FII).
4. O restante é calculado automaticamente.

## Como o cálculo funciona

O patrimônio considera **aportes mensais com reinvestimento** dos rendimentos, usando a função financeira `FV` do Excel:

```
Patrimônio = FV(rendimento mensal; meses; -aporte mensal)
Dividendos mensais = Patrimônio × rendimento mensal
```

## Tecnologias

- Microsoft Excel (fórmulas e gráficos)
- Design da planilha com tema escuro e paleta verde-água

## Estrutura do repositório

```
.
├── BABU_investimentos.xlsx
├── imagens/
│   ├── banner.png
│   └── painel.png
└── README.md
```

## Aviso

Rentabilidade passada não garante rentabilidade futura. Os valores usados na planilha são exemplos e devem ser ajustados à sua realidade. Antes de investir, avalie seu perfil e, se necessário, consulte um profissional habilitado.

## Autor

**[Seu nome]**
[LinkedIn](https://www.linkedin.com/in/seu-perfil) | [E-mail](mailto:seu@email.com)

Se o projeto foi útil para você, deixe uma estrela no repositório.
