<script lang="tsx">
import { defineComponent } from 'vue'
import TheWelcome from '../components/TheWelcome.vue'

export default defineComponent({
  name: 'HomeView',
  setup: () => {
    return () => (
      <main>
        <TheWelcome />
      </main>
    )
  }
})
</script>
