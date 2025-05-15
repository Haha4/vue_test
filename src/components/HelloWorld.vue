<template>
   <el-dialog v-model="dialogVisible" append-to-body title="Tips" width="500" draggable>
    <span>It's a draggable Dialog</span>
    <template #footer>
      <div class="dialog-footer">
        <el-button @click="dialogVisible = false">Cancel</el-button>
        <el-button type="primary" @click="dialogVisible = false">
          Confirm
        </el-button>
      </div>
    </template>
  </el-dialog>

</template>
<script setup>
import { ref } from 'vue'
defineProps({
  msg: String,
})
const dialogVisible = ref(false)
const dialogOverflowVisible = ref(false)
defineExpose({
  dialogVisible,
  dialogOverflowVisible,
})

const count = ref(0)
</script>
<style scoped>
.read-the-docs {
  color: #888;
}
</style>
