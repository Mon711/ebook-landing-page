<script>
	import { FaqItem, Button } from '$components';
	import twitterIcon from '$assets/icons/x-icon.webp';
</script>

<section class="faq-section">
	<h2 class="mb-l">Frequently asked questions</h2>
	<div class="faq-container">
		<FaqItem />
	</div>
	<div class="additional-info">
		<Button class="mt-s">BUY NOW</Button>
		<p class="mt-m">Any other questons?</p>
		<a href="https://x.com/MrinalSood3">
			<p>
				Hit me up on X <img src={twitterIcon} class="twitter-icon" alt="" />
			</p>
		</a>
	</div>
</section>
