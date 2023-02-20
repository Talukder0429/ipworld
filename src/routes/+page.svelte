<script>
	import Fa from 'svelte-fa/src/fa.svelte';
	import { faDesktop } from '@fortawesome/free-solid-svg-icons';
	import { faVideo } from '@fortawesome/free-solid-svg-icons';
	import { faPhone } from '@fortawesome/free-solid-svg-icons';
	import { faCashRegister } from '@fortawesome/free-solid-svg-icons';
	import { faShieldAlt } from '@fortawesome/free-solid-svg-icons';

	const srcPc = '/images/pc2.jpg';
	const srcTv = '/images/webtv.jpg';
	const srcPhone = '/images/phone.jpg';
	const srcCam = '/images/ss2.jpg';
	const srcPos = '/images/pos.jpg';
</script>

<h1 class="pt-4 pb-2 text-center text-4xl">Welcome to The IPWorld Inc.</h1>
<h2 class="pb-4 text-center text-2xl">Preparing hardware and software solutions since 1996!</h2>
<div
	class="flex flex-col items-center justify-center min-h-[40vh] bg-fixed bg-center bg-cover p-4"
	style="background-image: url({srcPc});"
>
	<div class="card max-w-screen-sm">
		<Fa size="8x" icon={faDesktop} />
		<div class="text-center">
			<div class="text-3xl p-2">Laptops, Desktops, Gaming PCs</div>
			<div class="border-t border-gray-800" />
			<div class="p-4 text-lg">
				Unbelievable prices on laptops and desktops (from off-lease computer auction), as well as
				repairs. Our gaming PCs are built by experts using high grade components!
			</div>
		</div>
	</div>
</div>

<div
	class="flex flex-col items-center justify-center min-h-[40vh] bg-fixed bg-center bg-cover p-4"
	style="background-image: url({srcTv});"
>
	<div class="card max-w-screen-sm">
		<Fa size="8x" icon={faVideo} />
		<div class="text-center">
			<div class="text-3xl p-2">Web TV</div>
			<div class="border-t border-gray-800" />
			<div class="p-4 text-lg">
				Make your own TV station, with easy and reliable solutions for your very own online TV
				channel(s)!
			</div>
		</div>
	</div>
</div>

<div
	class="flex flex-col items-center justify-center min-h-[40vh] bg-fixed bg-center bg-cover p-4"
	style="background-image: url({srcPhone});"
>
	<div class="card max-w-screen-sm">
		<Fa size="8x" icon={faPhone} />
		<div class="text-center">
			<div class="text-3xl p-2">Long-Distance Calling</div>
			<div class="border-t border-gray-800" />
			<div class="p-4 text-lg">
				Pin-less long distance calling, with the cheapest rates to over 50 different countries!
			</div>
		</div>
	</div>
</div>

<div
	class="flex flex-col items-center justify-center min-h-[40vh] bg-fixed bg-center bg-cover p-4"
	style="background-image: url({srcCam});"
>
	<div class="card max-w-screen-sm">
		<Fa size="8x" icon={faShieldAlt} />
		<div class="text-center">
			<div class="text-3xl p-2">Security Surveillance System</div>
			<div class="border-t border-gray-800" />
			<div class="p-4 text-lg">
				Ensure peace of mind with our 24/7 surveillance systems, designed to cover a large perimeter
				both inside and out. Tested for Canadian weather!
			</div>
		</div>
	</div>
</div>

<div
	class="flex flex-col items-center justify-center min-h-[40vh] bg-fixed bg-center bg-cover p-4"
	style="background-image: url({srcPos});"
>
	<div class="card max-w-screen-sm">
		<Fa size="8x" icon={faCashRegister} />
		<div class="text-center">
			<div class="text-3xl p-2">Point of Sale</div>
			<div class="border-t border-gray-800" />
			<div class="p-4 text-lg">
				For restaurants and small business, operate from your smart phone and/or tablet. Easy and
				Reliable solution for your daily sales tracking solution, starting from just $500!
			</div>
		</div>
	</div>
</div>

<h2 class="pt-4 text-center text-2xl">Looking for a custom solution?</h2>
<h2 class="pb-4 text-center text-2xl">
	Don't hesitate to <a href="/contact" class="underline italic">contact us!</a>
</h2>
