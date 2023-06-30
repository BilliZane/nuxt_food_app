<template>
  <div>
    <label :for="select">What {{ select }} do you want?</label>
    <select
      @change="$emit('change', $event.target.value)"
      :id="select"
      name="select"
    >
      <option value>-- Pleace select a {{ select }}</option>
      <option v-for="option in selectOptions" :value="option" :key="option">
        {{ option }}
      </option>
    </select>
  </div>
</template>

<script>
export default {
  props: {
    select: {
      type: String,
      default: 'cusine'
    },
    selectOptions: {
      type: Array,
      default: () => ['tacos', 'pizza', 'dim sum']
    }
  }
}
</script>
