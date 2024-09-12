
## Lista
const meta1 = {
	texto: "Ler um livro toda semana",
	checked: false
}F
const metas = [
	meta1,
	{
		value: "Ir para a academia 5 vezes na semana",
		checked: false
	}
]
console.log(metas[0].texto)
console.log(metas[1].value)

## Estrutura de condições
function start() {
	let count = 0
	while (count < 10) {
		console.log(count);
		count = count + 1
	}
}
start()

## retorna um objeto e so quero o select
const { select } = require("@inquirer/prompts")

## async await | promisse
const { select } = require("@inquirer/prompts")
async function start() {
	while (true) {
		const opcao = await select({
			message: "Menu >",
			choices: [
				{
					name: "Cadastrar meta",
					value: "cadastrar"
				},
				{
					name: "Listar metas",
					value: "listar"
				},
				{
					name: "Sair",
					value: "sair"
				}
			]
		})
		switch (opcao) {
			case "cadastrar":
				console.log("Vamos cadastrar")
				break
			case "listar":
				console.log("Vamos listar");
				break
			case "sair":
				console.log("Até a proxima");
				return
		}
	}
}
start()

## Arrays e objetos

## Spreed operator (...)