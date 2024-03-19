<script lang="ts">
	import '../app.postcss';

    import iconImg from "$lib/assets/Icon.png";
    import {page} from '$app/stores';
    import PageFooter from "$lib/components/PageFooter.svelte";

    let icon = iconImg !== undefined ? iconImg : "./favicon.ico";

    export let data;

    // Floating UI for Popups
	import { computePosition, autoUpdate, flip, shift, offset, arrow } from '@floating-ui/dom';
    import {AppBar, AppShell, storePopup} from '@skeletonlabs/skeleton';
    import PageTransition from "$lib/components/PageTransition.svelte";
	storePopup.set({ computePosition, autoUpdate, flip, shift, offset, arrow });
</script>


<AppShell>
    <svelte:fragment slot="header">
        <AppBar>
            <svelte:fragment slot="lead"><a href="/" class="inline-flex">
                <img alt="Uleth Icon" src={icon} class="w-1/6 h-1/6"/>
                <p class="ml-2 my-auto">Cole's Portfolio</p>
            </a></svelte:fragment>
            <a rel="external" href="/project-a/" class="{$page.url.pathname === '/project-a' ? 'underline' : ''}">Project A</a>
            <a href="/project-b/" class="{$page.url.pathname === '/project-b' ? 'underline' : ''}">Project B</a>
            <a href="/project-c/" class="{$page.url.pathname === '/project-c' ? 'underline' : ''}">Project C</a>
            <svelte:fragment slot="trail"><a class="{$page.url.pathname === '/contact-me' ? 'underline' : ''}" href="/contact-me">Contact Me</a></svelte:fragment>
        </AppBar>
    </svelte:fragment>
    <!-- Router Slot -->
    <PageTransition pathname={data.pathname}>
        <slot />
    </PageTransition>
    <!-- ---- / ---- -->
    <svelte:fragment slot="pageFooter"><PageFooter/></svelte:fragment>
    <!-- (footer) -->
</AppShell>
