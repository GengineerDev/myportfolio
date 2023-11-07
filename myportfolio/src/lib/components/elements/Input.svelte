<script>
	export let labelText = 'label';
	export let name = 'title';
	export let inputType = 'text';
	export let textarea = false;
	export let helperText = 'Helper Text';

	let projectDesc = '';
	let wordCount = 0;

	const onKeyup = () => {
		let matchWords = projectDesc.match(/\S+/g);
		wordCount = matchWords ? matchWords.length : 0;
	};
</script>

<div>
	<label for={name} class="body-1">{labelText}</label>
	{#if textarea}
		<textarea id={name} {name} bind:value={projectDesc} on:keyup={onKeyup} rows="10" class="{wordCount > 300 ? 'red-border' : ''}"/>
		<div class="helper-text">
			<p class="body-3 {wordCount > 300 ? 'red' : ''}">{wordCount > 300 ? `Keep your message within 300 words` : helperText}</p>
			<p class="body-3 {wordCount > 300 ? 'red' : ''}">{wordCount}/300 words</p>
		</div>
	{:else}
		<input type={inputType} id={name} {name} />
	{/if}
</div>

<style>
	label {
		font-family: unset;
		font-weight: unset;
		display: block;
		margin-bottom: 8px;
	}

	.helper-text {
		color: var(--main-colors-gray-4);
		display: flex;
		justify-content: space-between;
		margin-top: 8px;
		margin-bottom: 16px;
	}

	textarea,
	input {
		border: 1px solid var(--gray);
		color: var(--gray);
		font-family: 'General Sans Regular', 'Times New Roman', Times, serif;
		background: transparent;
		font-size: 24px;
		width: 100%;
	}

	textarea {
		padding: 32px 48px;
		resize: none;
	}

	input {
		padding: 16px 24px;
	}

	div {
		margin: 16px 0;
	}

    .red-border {
        border: 1px solid var(--red_border);
    }

	.red {
		color: var(--red_danger);
	}
</style>
