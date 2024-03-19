<script>
    import {page} from '$app/stores';
</script>

<h1>Oops, something hasn't worked properly, use the error code and contact me with your problem.</h1>
<h1>{$page.status}: {$page.error.message}</h1>