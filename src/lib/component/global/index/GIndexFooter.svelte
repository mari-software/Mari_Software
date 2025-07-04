<script>
	import MariLogoSvg from '$lib/asset/image/svg/MariLogoSvg.svelte';
	import DaisyUiFooter from '$lib/component/library/daisyui/footer/DaisyUiFooter.svelte';
	import DaisyUiLink from '$lib/component/library/daisyui/link/DaisyUiLink.svelte';
	import LucideFacebook from '$lib/component/library/lucide/LucideFacebook.svelte';
	import LucideInstagram from '$lib/component/library/lucide/LucideInstagram.svelte';
	import LucideTwitter from '$lib/component/library/lucide/LucideTwitter.svelte';
</script>

<section id="footer">
	<DaisyUiFooter
		className="grid grid-cols-2  bg-primary-content py-10 px-5 gap-10 "
	>
		<section class="">
			<figure>
				<MariLogoSvg className="size-14" />
			</figure>
			<h6 class="d-footer-title">mari.software</h6>
			<p class="text-xs">© 2025 mari.software All Rights Reserved</p>
		</section>

		<section class="flex flex-col items-center gap-2 text-center">
			<h6 class="d-footer-title">Follow Us</h6>
			<div class="flex gap-3">
				<LucideTwitter />
				<LucideInstagram />
				<LucideFacebook />
			</div>
		</section>

		<section class="">
			<h6 class="d-footer-title">About Mari</h6>
			<DaisyUiLink href="">About Us</DaisyUiLink>
			<DaisyUiLink href="">Contact Us</DaisyUiLink>
			<DaisyUiLink href="">FAQs</DaisyUiLink>
			<DaisyUiLink href="">Terms and Conditions</DaisyUiLink>
		</section>

		<section class="">
			<h6 class="d-footer-title">Apps</h6>
			<DaisyUiLink href="">Trending</DaisyUiLink>
			<DaisyUiLink href="">Popular</DaisyUiLink>
			<DaisyUiLink href="">New</DaisyUiLink>
			<DaisyUiLink href="">Updated</DaisyUiLink>
		</section>
	</DaisyUiFooter>
</section>
