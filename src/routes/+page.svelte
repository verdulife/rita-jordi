<script>
	$: cc = 'ES5321007712011300244003';
	async function copy() {
		await navigator.clipboard.writeText(cc);
		cc = 'Número copiat!';

		setTimeout(() => {
			cc = 'ES5321007712011300244003';
		}, 2000);
	}
</script>

<section id="land" class="col xfill">
	<img class="contain xfill" src="/chair-2.png" alt="Rita & Niubó" />

	<article class="col xfill">
		<h1 class="title tcenter xfill">Rita & Jordi</h1>

		<p class="text tcenter xfill">
			Després de 7 anys de prova en què hem aconseguit l'excel•lent, hem decidit que ens casem!
		</p>

		<xdiv />

		<p class="text tcenter xfill">
			<small class="text tcenter xfill">El proper</small>
			<br />
			<strong>17 de desembre<br />a les 12 h</strong>
			<br />
			<small class="text tcenter xfill">a l'Ajuntament de Sitges</small>
		</p>

		<xdiv />

		<p class="text tcenter xfill">Ens acompanyeu?</p>
	</article>
</section>

<section id="info" class="col xfill">
	<p class="text tcenter xfill">
		I per celebrar-ho tots junts, us esperem a les 17 h a la Discoteca Ricky's. Música en viu,
		pica-pica, pastis, copes...
		<br /><br />
		...i molta felicitat, fins que el cos aguanti!
		<br /><br />
		Us esperem a tots!
	</p>
</section>

<section id="bank" class="col acenter xfill">
	<p class="text tcenter xfill">Molts ens heu demanat<br />el nº de compte</p>
	<h2 class="text tcenter row fcenter nowrap xfill" on:click={copy}>
		<span class="grow">{cc}</span>
		<img src="/copy.svg" alt="Copiar" />
	</h2>
</section>

<section id="contact" class="col acenter xfill">
	<p class="text tcenter xfill">Preguem confirmació per whatsapp</p>

	<a
		class="text btn pri round"
		href="https://api.whatsapp.com/send?phone=0034649417078"
		target="_blank"
	>
		Rita 649.417.078
	</a>

	<a
		class="text btn pri round"
		href="https://api.whatsapp.com/send?phone=0034633141179"
		target="_blank"
	>
		Niubó 633.141.179
	</a>
</section>

<footer class="title tcenter xfill">Rita & Jordi 2022</footer>

<style lang="scss">
	#land {
		padding-bottom: 20%;

		article {
			gap: 20px;
			margin-top: 20px;
			padding: 0 20px;

			h1 {
				color: var(--color-pri);
				font-size: 60px;
			}

			p {
				font-size: 18px;

				small {
					font-size: 16px;
					text-transform: uppercase;
				}

				strong {
					font-size: 30px;
					line-height: 1;
					padding: 5px 0;
				}
			}
		}
	}

	#info {
		gap: 40px;
		background: var(--color-pri);
		color: #fff;
		font-size: 18px;
		padding: 20% 20px;
	}

	#bank {
		padding: 20% 20px;

		h2 {
			background: #fff;
			border: 1px solid #999;
			border-radius: 0.25em;
			margin-top: 20px;

			span {
				font-size: 16px;
				margin-bottom: -4px;
				padding: 0 10px;
			}

			img {
				width: 40px;
				background: var(--color-pri);
				padding: 12px;
			}
		}
	}

	#contact {
		gap: 10px;
		padding: 0 20px 30% 20px;

		a.btn {
			width: 70%;
			color: #fff;
			font-size: 18px;
		}
	}

	footer {
		position: fixed;
		bottom: 0;
		left: 0;
		background: #000;
		color: #fff;
		font-size: 20px;
		padding: 12px;
	}
</style>
