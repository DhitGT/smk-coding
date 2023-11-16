<script lang="ts" setup>
const categoryStore = useCategoryStore();

let result;
result = "{'name':'topi','description' : 'khusus topi'}";
await categoryStore.createCategory(result);
if (!categoryStore.status) {
}
</script>
<template>
  <section>
    <div class="container">
      <FormsCategoryForm />
    </div>
  </section>
</template>
