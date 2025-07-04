<script lang="ts">
    let {className, children} = $props<{
        className?: string;
        children: () => void;
    }>();
</script>

<footer class="d-footer sm:d-footer-horizontal  text-base-content p-1 {className}">
  {@render children()}
</footer>