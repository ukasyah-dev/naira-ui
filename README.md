# Naira UI

Clean and customizable Svelte component library that helps you build apps faster.

## Getting started

This library requires that you have a [SvelteKit](https://svelte.dev/docs/kit/introduction)
project with [Tailwind CSS](https://tailwindcss.com/) set up. If you haven't done so yet,
please refer to the official documentation to begin.

To install the library, run:

```bash
pnpm add -D naira-ui
```

Update `src/routes/+layout.svelte` file:

```svelte
<script lang="ts">
	import { Provider } from 'naira-ui';
	import 'naira-ui/styles.css';

	let { children } = $props();
</script>

<Provider>
	{@render children()}
</Provider>
```

That's it! You're now ready to build with Naira UI.
