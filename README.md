# practicaNum3josemirlopezstg
practica numero 3
<script>alert("calculadora practica3")<;</script>
<input type="text" id="n11" placeholder="ingresa un numero">
<input type="text" id="n22" placeholder="ingresa segundo numero">

<select id="op">
    <option value="+">+</option>
    <option value="-">-</option>
    <option value="*">*</option>
    <option value="/">/</option>
</select>
    
<button id="calcular2">Calcular</button>

<output id="r2"></output> 
<script>
    
    document.querySelector('#calcular2').addEventListener('click', () =>{
        const n1 = parseInt(document.querySelector('#n11').value);
        const n2 = parseInt(document.querySelector('#n22').value);
        const op2 = document.querySelector('#op').value;
        let r;
        if(op2 == '+'){
            r = n1 + n2;
        }else if( op2 == '-'){
            r = n1 - n2;
        }else if(op2 == '*'){
            r = n1 * n2;
        }else if(op2 == '/'){
            r = n1 / n2;
        }
        document.querySelector('#r2').innerHTML = r;
    });

</script>
