<script>
    import VoltarMenu from './VoltarMenu.svelte'
    class imc {
        constructor(peso,altura) {
            this.peso=peso;
            this.altura=altura;
        }
    }
    
    let IMC = new imc ("", "")
    
    let total = 0
    let altura= 0
    
    function Calculo() {
        altura = (IMC.altura * IMC.altura) 
        total = altura / IMC.peso 
        alert (total)
    }
    </script>
    
    <body>
        <h3>Preencha os campos abaixo e veja seu resultado:</h3>
        <div>
            <p><b>Digite seu peso:</b></p>
            <input type="number" bind:value={IMC.peso} >
        </div>
        <div>
            <p><b>Digite sua altura:</b></p>
            <input type="number" bind:value={IMC.altura} >
        </div>
        <div>
            <button on:click={Calculo}>Calcular</button>
        </div>
    
    </body>
    <VoltarMenu/>
    
    <style>
    body {
        text-align: center;
    }
    </style>
    
    