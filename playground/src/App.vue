<!--
 * @Author: chenanan
 * @Date: 2023-04-28 23:06:19
 * @LastEditors: chenanan
 * @LastEditTime: 2023-04-28 23:31:05
 * @Description:  
-->
<template>
  <component :is="Icon" v-for="(Icon, key) in icons" :key="key" class="icon" />
  <hr />
  <component
    :is="`ElIcon${key}`"
    v-for="key in Object.keys(icons)"
    :key="key"
    class="icon"
  />
</template>

<script lang="ts" setup>
import { icons } from '@hsmos-ui/icons-vue/global'
</script>

<style>
.icon {
  height: 48px;
  /* color: #409eff; */
}
</style>
