<script>
	import { estado } from './Estado.js'
	import { trocarEstadoDoJogo } from './Estado.js'
</script>

<h1>
	IMC
</h1>

<br><br>

<div class='menu' on:click={() => trocarEstadoDoJogo('imc')}>
	Saiba seu IMC
</div>

<div class='menu' on:click={() => trocarEstadoDoJogo('sobre')}>
	Sobre
</div>

