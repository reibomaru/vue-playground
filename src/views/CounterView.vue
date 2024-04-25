<script lang="tsx">
import { defineComponent, ref, unref } from 'vue'

export default defineComponent({
  name: 'CounterView',
  setup: () => {
    const count = ref(0)
    const handleClick = () => {
      count.value++
    }
    return () => (
      <div>
        <div>count: {unref(count)}</div>
        <button onClick={handleClick}>click me!!</button>
      </div>
    )
  }
})
</script>
