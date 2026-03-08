<script lang="ts">
	let {
		emoji,
		name,
		tagline,
		description,
		url,
		githubUrl,
		status = 'live'
	}: {
		emoji: string;
		name: string;
		tagline: string;
		description: string;
		url: string;
		githubUrl: string;
		status?: string;
	} = $props();
</script>

<div
	class="bg-bg-surface border-2 border-border-subtle rounded-sm p-6
		shadow-[2px_2px_0px_#0e0e1e] transition-all duration-150 ease-out
		hover:border-primary hover:shadow-[3px_3px_0px_#C8860A] hover:-translate-x-px hover:-translate-y-px
		group"
>
	<div class="flex items-start justify-between mb-4">
		<div class="flex items-center gap-3">
			<span class="text-3xl">{emoji}</span>
			<div>
				<h3 class="text-sm mb-1 text-text">{name}</h3>
				<p class="text-xs text-text-muted font-mono">{tagline}</p>
			</div>
		</div>
		{#if status === 'live'}
			<span class="font-pixel text-[0.55rem] text-primary bg-bg-elevated border border-border-subtle rounded-sm px-2 py-1">
				LIVE
			</span>
		{/if}
	</div>
	<p class="text-sm text-text-muted leading-relaxed mb-4">{description}</p>
	<div class="flex items-center justify-between text-xs text-text-muted">
		<a
			href={url}
			target="_blank"
			rel="noopener noreferrer"
			class="group-hover:text-primary transition-colors duration-150"
		>Visit app →</a>
		<a
			href={githubUrl}
			target="_blank"
			rel="noopener noreferrer"
			class="hover:text-primary transition-colors duration-150"
		>GitHub</a>
	</div>
</div>
