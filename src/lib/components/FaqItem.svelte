<script>
	import chevronDown from '$assets/icons/chevron-down.svg';
</script>

<button class="container">
	<div class="question-and-answer">
		<p class="question mb-s">
			Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis, odit?
		</p>
		<p class="answer">
			Lorem ipsum, dolor sit amet consectetur adipisicing elit. Laudantium explicabo et deleniti,
			ullam ipsum reiciendis assumenda odio omnis numquam impedit provident quaerat eius autem
			nostrum quia beatae iusto aut suscipit voluptatem, error itaque fugiat repellendus aperiam.
			Rem obcaecati doloremque, neque tempora iste est quas dignissimos dolores accusamus aperiam,
			qui voluptas.
		</p>
	</div>
	<img src={chevronDown} alt="" />
</button>

<style>
	.container {
		display: flex;
		justify-content: space-between;
		align-items: flex-start;
		padding: 12px 0;
		border-bottom: 1px solid grey;
		text-align: left;
	}

	.question-and-answer {
		padding-right: 150px;
		flex-grow: 1;
	}

	.answer {
		max-height: 0;
		overflow: hidden;
		opacity: 0;
		transition:
			max-height 0.3s ease-out,
			opacity 0.3s ease-out;
	}

	button img {
		width: 24px;
		height: 24px;
		transition: transform 0.3s linear;
	}

	.question {
		font-weight: 600;
	}

	.container-expanded img {
		transform: rotate(180deg);
	}

	.container-expanded .answer {
		max-height: unset;
		opacity: 1;
	}
</style>
