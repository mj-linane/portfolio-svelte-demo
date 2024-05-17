<!-- Long Sales Page For Selling Subscription Apple Deliveries  To High Schoolers -->
<script>
	import Hero from '$lib/components/Hero.svelte';
	import LongProductDescription from '$lib/components/LongProductDescription.svelte';
	import PriceCardGrid from '$lib/components/PriceCardGrid.svelte';

	const priceTiers = [
		{
			priceTier: 'Basic',
			price: 9.99,
			features: ['3 apples per week', 'Choose from 3 apple types', 'Free delivery']
		},
		{
			priceTier: 'Standard',
			price: 14.99,
			features: ['5 apples per week', 'Choose from 5 apple types', 'Free delivery']
		},
		{
			priceTier: 'Premium',
			price: 19.99,
			features: ['7 apples per week', 'Choose from 7 apple types', 'Free delivery']
		}
	];
</script>

<Hero
	title="Fresh Apple Deliveries for High Schoolers"
	subtitle="Subscribe to receive weekly apple deliveries"
	alt="Image of fresh apples"
/>

<LongProductDescription productHeadline="Apples for High Schoolers">
	<p>
		Are you tired of the same old snack options, high in sugar and low in nutrition? Do you find
		yourself reaching for unhealthy choices when hunger strikes, only to feel guilty later? It's
		time to revolutionize your snacking habits with our subscription service that delivers fresh,
		delicious apples straight to high schoolers like you every single week.
	</p>
	<p>
		Picture this: crisp, juicy apples, bursting with flavor and packed with nutrients, delivered
		right to your doorstep. No more settling for stale snacks from vending machines or unhealthy
		options from fast-food joints. With our subscription service, you'll have access to a variety of
		apple types, including the ever-popular Honeycrisp, the sweet and tangy Fuji, and the classic
		Granny Smith. Each week, you'll be greeted with a new selection, ensuring that your taste buds
		never get bored.
	</p>
	<p>
		But it's not just about the variety; it's about the quality too. We take pride in sourcing our
		apples from local orchards, ensuring that they're picked at the peak of freshness and flavor.
		Unlike mass-produced apples that travel long distances and sit on shelves for weeks, our apples
		are guaranteed to be fresh and delicious. From the moment you take your first bite, you'll taste
		the difference that local sourcing makes.
	</p>
	<p>
		But don't just take our word for it. Our satisfied customers rave about the quality of our
		apples, with many reporting that they've never tasted anything like them before. Whether you're
		looking for a healthy snack to fuel your busy days at school or a refreshing treat to enjoy
		after sports practice, our apples are the perfect choice.
	</p>
	<p>
		And the best part? Signing up is quick and easy. Simply visit our website, choose your
		subscription plan, and start receiving your weekly apple deliveries. With flexible options to
		fit any budget and schedule, there's no reason not to give it a try.
	</p>
	<p>
		So why wait? Take the first step towards a healthier, happier you by signing up for our
		subscription service today. With fresh, delicious apples delivered straight to your door every
		week, you'll wonder how you ever lived without it. Join the apple revolution and make snacking
		great again!
	</p>
</LongProductDescription>

<PriceCardGrid {priceTiers} />
