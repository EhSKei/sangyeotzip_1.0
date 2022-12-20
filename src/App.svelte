<script>
    import Router from "svelte-spa-router";
    import Layout from "./lib/Layout.svelte";
    import routes from "./routes";
    import 'aos/dist/aos.css';


</script>

<Layout>
    <Router routes="{routes}" restoreScrollState="{true}"/>
</Layout>
