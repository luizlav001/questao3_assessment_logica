# questao3_assessment_logica
def gastos_mensal(renda_familiar, gastos_moradia, gastos_educacao, gastos_transportes):
  renda_familiar = float(input("Informe  a renda familiar. R$: "))
  gastos_moradia = float(input("Informe os gastos com moradia. R$: "))
  gastos_educacao = float(input("Informe os gastos com educação. R$: "))
  gastos_transportes = float(input("Informe os gastos com transportes. R$: "))

  limite_moradia = renda_familiar * 30 / 100
  limite_educacao = renda_familiar * 20 / 100
  limite_transportes = renda_familiar * 15 / 100

  porc_moradia =  gastos_moradia * 100 / renda_familiar
  porc_educacao = gastos_educacao * 100 / renda_familiar
  porc_transportes =  gastos_transportes * 100 / renda_familiar

  desp_moradia = 30
  desp_educacao = 20
  desp_transportes = 15 

  if porc_moradia > desp_moradia:
    print(f"Seus gastos totais com moradia comprometem {porc_moradia : .1f}% de sua renda total. O máximo recomendado é de 30%. Por tanto, idealmente, o máximo de sua renda comprometida com moradia deveria ser de R$: {limite_moradia} ")
  else:
    print(f"Seus gastos totais com moradia  comprometem {porc_moradia : .1f}% de sua renda total. O máximo recomendado é de 30%. Seus gastos estão dentro da margem recomendada.")


  if porc_educacao > desp_educacao:
    print(f"Seus gastos totais com educação comprometem {porc_educacao : .1f}% de sua renda total. O máximo recomendado é de 20%. Por tanto, idealmente, o máximo de sua renda comprometida com educação deveria ser de R$: {limite_educacao}")
  else:
    print(f"Seus gastos totais com educação comprometem {porc_educacao : .1f}% de sua renda total. O máximo rcomendado é de 20%. seus gastos estão dentro da margem recomendada. ")

  if porc_transportes > desp_transportes:
    print(f"Seus gastos totais com educação comprometem {porc_transportes : .1f}% de sua renda total. O máximo recomendado é de 15%. Por tanto, idealmente, o máximo de sua renda comprometida com educação deveria ser de R$: {limite_transportes}")
  else:
    print(f"Seus gastos totais com educação comprometem {porc_transportes : .1f}% de sua renda total. O máximo rcomendado é de 15%. seus gastos estão dentro da margem recomendada. ")




gastos_mensal(renda_familiar, gastos_moradia, gastos_educacao, gastos_transportes)
