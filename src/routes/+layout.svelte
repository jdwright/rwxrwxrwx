<script>
  // Your selected Skeleton theme:
  import '@skeletonlabs/skeleton/themes/theme-skeleton.css';

  // This contains the bulk of Skeletons required styles:
  import '@skeletonlabs/skeleton/styles/skeleton.css';

  // Finally, your application's global stylesheet (sometimes labeled 'app.css')
  import '../app.postcss';

  import { AppShell, AppBar, LightSwitch } from '@skeletonlabs/skeleton';
</script>

<AppShell class="c" style="padding: 50px 0 100px 0">
	<svelte:fragment slot="header">
    <AppBar>
      <svelte:fragment slot="lead">rwxrwxrwx</svelte:fragment>
      <svelte:fragment slot="trail"><LightSwitch /></svelte:fragment>
    </AppBar>
  </svelte:fragment>
  <slot />
</AppShell>
