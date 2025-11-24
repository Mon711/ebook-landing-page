<script>
	import authorPic from '$assets/my_pic.jpg';
</script>

<section class="author-section">
	<h2 class="mb-l">About the author</h2>
	<div class="author-container">
		<div class="author-text">
			<p class="mb-s">
				Mrinal Sood is an ambitious and results-oriented Developer who combines a solid foundation
				in full-stack web technologies with a rapid, hands-on pivot into the field of Artificial
				Intelligence. Proficient across multiple languages, including Python, JavaScript, C, and
				C++, Mrinal has proven capabilities in frameworks like Django, Flask, and Laravel, as
				demonstrated by the development of several full-stack projects such as an auction-based
				e-commerce site and a Twitter-like social network.
			</p>
			<p>
				What truly sets Mrinal apart is a forward-looking focus on modern AI integration and applied
				knowledge of Large Language Models (LLMs). Mrinal currently works as a Part-Time Developer
				integrating open-source LLMs like LLaMA and Qwen into a technology platform, utilizing
				serverless GPUs and vLLM for efficient inference and deployment.
			</p>
		</div>
		<img src={authorPic} alt="Author Mrinal Sood" />
	</div>
</section>

<style>
    .author-section{
        padding: 80px 0;
        margin-left: 12vw;
        margin-right: 20vw;
        max-width: 1150px;
    }

	.author-container {
		display: flex;
		justify-content: space-between;
	}

	.author-container img {
		width: 40%;
        object-fit: cover;
		border: 6px solid black;
		box-shadow: 0 4px 24px rgba(0, 0, 0, 0.5);
	}

	.author-text {
		width: 55%;
	}
</style>
