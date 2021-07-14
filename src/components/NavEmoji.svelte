<script>
import { onMount } from 'svelte';
import { getRandomEmoji } from '../utils/emoji';

let emoji = '';
onMount(() => {
    emoji = getRandomEmoji();
});
</script>
<style lang="scss">
    .emoji {
        font-size: var(--h1-text-size);
    }
</style>

<span aria-hidden="true" class="emoji">{emoji}</span>