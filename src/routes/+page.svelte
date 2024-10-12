<script>
    import { createCollapsible, melt } from '@melt-ui/svelte'
    const { open, root, content, trigger } = createCollapsible()
  </script>
   
  <div {...$root} use:root>
    <button {...$trigger} use:trigger>{$open ? 'Close' : 'Open'}</button>
    <div {...$content} use:content>Obi-Wan says: Hello there!</div>
  </div>