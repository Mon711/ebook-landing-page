<script>
	import { FaqItem, Button } from '$components';
	import xIcon from '$assets/icons/x-icon.webp';
</script>

<section class="landing-page-section">
	<h2 class="mb-l">Frequently asked questions</h2>
	<div class="faq-container">
		<FaqItem />
	</div>
	<div class="additional-info mt-m">
		<Button class="mt-s">BUY NOW</Button>
		<p class="mt-m">Any other questons?</p>
		<a href="https://x.com/MrinalSood3">
			<p>
				Hit me up on <img src={xIcon} class="x-icon" alt="" />
			</p>
		</a>
	</div>
</section>

<style>
    .additional-info{
        display: flex;
        flex-direction: column;
        align-items: center;
        color: grey;
    }

    .x-icon {
        width: 16px;
        height: 16px;
    }

    a{
        text-decoration: underline;
    }
</style>
