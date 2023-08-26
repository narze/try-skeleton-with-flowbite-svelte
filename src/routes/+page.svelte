<script lang="ts">
	import { LightSwitch } from '@skeletonlabs/skeleton';
	import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';

	import TimelineComponent from '$lib/TimelineComponent.svelte';
	import { Alert, Checkbox } from 'flowbite-svelte';
	import { DarkMode } from 'flowbite-svelte';
</script>

<div class="container h-full mx-auto flex justify-center items-center">
	<div class="space-y-5">
		<h1 class="h1">Let's get cracking bones! Also with Flowbite Svelte!</h1>

		<div class="container grid grid-cols-2 gap-x-8">
			<div class="space-y-4">
				<h1 class="prose-xl dark:prose-invert">Skeleton</h1>

				<code>LightSwitch</code>
				<LightSwitch />

				<div class="flex flex-col gap-4 place-items-start">
					<code>class="variant-soft-primary"</code>
					<button class="btn variant-soft-primary">Button</button>
				</div>

				<code>Accordion</code>

				<Accordion class="variant-soft-primary rounded" autocollapse={true}>
					<AccordionItem>
						<!-- <svelte:fragment slot="lead">(icon)</svelte:fragment> -->
						<svelte:fragment slot="summary"
							><span class="font-medium"
								>Proident ut in sunt anim commodo anim occaecat ex ea ad dolore sint magna minim.</span
							></svelte:fragment
						>
						<svelte:fragment slot="content"
							>Occaecat dolor cupidatat sunt do in minim proident do eiusmod. Do minim est irure
							dolor mollit voluptate magna. Commodo veniam ad officia Lorem.</svelte:fragment
						>
					</AccordionItem>
					<AccordionItem>
						<!-- <svelte:fragment slot="lead">(icon)</svelte:fragment> -->
						<svelte:fragment slot="summary"
							><span class="font-medium">Tempor eu laboris amet ut nostrud est.</span
							></svelte:fragment
						>
						<svelte:fragment slot="content"
							>Labore consequat ipsum enim anim irure magna esse pariatur eu dolore culpa officia.
							Elit proident incididunt eu et esse ipsum labore duis officia irure elit eiusmod irure
							et. Enim reprehenderit aliqua non quis ut do exercitation Lorem commodo est nulla ut
							magna. Excepteur ipsum id nostrud nulla quis aute incididunt quis. Ipsum esse ullamco
							laboris mollit et sunt. Nostrud amet ipsum minim dolore. Tempor fugiat commodo labore
							commodo officia et incididunt amet aute est aliqua laboris.</svelte:fragment
						>
					</AccordionItem>
					<!-- ... -->
				</Accordion>
			</div>

			<div class="space-y-4">
				<h1 class="prose-xl dark:prose-invert">Flowbite</h1>

				<code>DarkMode</code>
				<DarkMode btnClass="btn block" />

				<code>TimelineComponent</code>
				<TimelineComponent />

				<code>Alert</code>
				<Alert>
					<span class="font-medium">Info alert!</span>
					Change a few things up and try submitting again.
				</Alert>

				<div class="flex flex-col items-start gap-y-4">
					<code>Checkbox</code>
					<Checkbox>Default checkbox</Checkbox>
					<Checkbox checked>Checked state</Checkbox>
				</div>
			</div>
		</div>
	</div>
</div>
