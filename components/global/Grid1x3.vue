<template>
  <div class="row">
    <span
      v-for="child in children"
      :key="child.title"
      class="col-lg-4 pr-sm-4 pr-lg-5"
    >
      <ThreeColumnChild
        :title="child.title"
        :desc="child.desc"
        :icon="child.icon"
      />
    </span>
  </div>
</template>

<script>
export default {
  props: {
    children: Array,
  },
}
</script>
