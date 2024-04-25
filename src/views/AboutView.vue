<script lang="tsx">
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'AboutView',
  setup: () => {
    return () => (
      <div class="about">
        <h1>This is an about page</h1>
      </div>
    )
  }
})
</script>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
