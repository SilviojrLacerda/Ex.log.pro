altura = 1.70
peso = 70
imc = peso / (altura * altura)

classificacao = ""
grau = 0

if ( imc <= 18.5){
  classificacao = "Magreza"
}
else if (imc < 25 ){
  classificacao = "Normal"
}
else if (imc < 30 ){
  classificacao = "Sobrepeso"
  grau = 1
  console.log(grau)
}
else if (imc < 39.9){
  classificacao = "Obesidade"
  grau = 2
  console.log("Cuidado! Você está acima do peso recomendado pela OMS.")
}
else if (imc > 40){
  classificacao = "Obesidade grave"
  grau = 3
  console.log("É importante procurar um médico para avaliar sua saúde")
}

console.log("Seu imc é", imc)
console.log("Sua classificação é", classificacao)
if (grau > 0)
console.log(grau)
