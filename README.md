# projeto_2_match.io

    valor = float(input("Digite o valor do emprestimo:R$  "))
    salario = float(input("Digite seu salário: R$ "))
    meses = int(input("Quantos meses para pagar: "))
		taxaDeJuros = float(0.03*meses)

		prestacao = valor/meses
		prestacaoTotal = prestacao*taxaDeJuros + prestacao
		valorTotalEmprestimo = float(prestacaoTotal * meses)

		#Validação de renda
		if prestacaoTotal > salario * 0.3:
			print("Infelizmente você não pode obter o empréstimo")
		else:
			print(f'Valor da prestação mensal é: R${prestacaoTotal:,.2f} --- Empréstimo OK')

			print(f'O valor total do emprestimo ficou em: R${valorTotalEmprestimo: ,.2f}')
