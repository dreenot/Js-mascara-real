# Js-mascara-real
mascara javascript para campos html na moeda real

## Funçoes disponíveis:
**bonoros(valor, minimo);**
*converte qualquer número para esse formato R$100.000,00
mesmo se estiver no padrão estrangeiro invertendo vírgula por pontos ou incluir letras e símbolos
se for inserído um número menor que o mínimo ele é substituído pelo mínimo*
**ex: $999,999.99 retorna R$999.999,99
ex: 2 retorna R$2,00**

**ibonoros(valor);**
*converte de volta para o formato que o js consegue calcular, usando ponto,
removendo letras, convertendo para número e deixando 2 casas decimais*
**ex: R$999.999,99 retorna 999999.99** 

## Como usar:
**inclua o js**
```
<script src="js/bonoro.js"></script>
```

**Inclua no seu codigo:**
```
<script type="text/javascript">
  	$("#valor").change(function(){
  		$(this).val(bonoros($(this).val(), 200));
  	});
</script>
```
