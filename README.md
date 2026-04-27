# pesquisa-satisfacao-python
# Pesquisa de satisfaÃ§Ã£o - TudoWeb

# Contadores para as respostas
qtde_excelente = 0
qtde_ruim = 0

# Teste com 10 entrevistados (para validaÃ§Ã£o)
# Para a versÃ£o final, basta alterar o range para 50
for i in range(10):  
    print(f"\nEntrevistado {i+1}")
    nome = input("Digite o nome: ")
    idade = int(input("Digite a idade: "))
    print("OpiniÃ£o sobre o atendimento:")
    print("1 - EXCELENTE")
    print("2 - BOM")
    print("3 - RUIM")
    opiniao = int(input("Digite sua opiniÃ£o (1/2/3): "))

    # Estrutura de decisÃ£o para contar opiniÃµes
    if opiniao == 1:
        qtde_excelente += 1
    elif opiniao == 3:
        qtde_ruim += 1

# ExibiÃ§Ã£o dos resultados finais
print("\nRESULTADOS DA PESQUISA")
print(f"Quantidade de respostas EXCELENTE: {qtde_excelente}")
print(f"Quantidade de respostas RUIM: {qtde_ruim}")
