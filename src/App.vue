<template>
  <div class="container">
    <global-header :user="currentUser"></global-header>
    <column-list :list="list"></column-list>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import 'bootstrap/dist/css/bootstrap.min.css'
import ColumnList, { ColumnProps } from './components/ColumnList.vue'
import GlobalHeader, { UserProps } from './components/GlobalHeader.vue'

const currentUser: UserProps = {
  isLogin: true,
  name: 'codehzy'
}

const testData: ColumnProps[] = [
  {
    id: 1,
    title: 'test1的专栏',
    description:
      '这是阿达克鲁赛德拉可适当卡事件代理卡事件代理看俺就打了卡就是来打开俺就',
    avatar:
      'https://avatars.githubusercontent.com/u/58018918?s=400&u=320faab333c28272b64af629375158aba1290587&v=4'
  },
  {
    id: 2,
    title: 'test2的专栏',
    description:
      '这是阿达克鲁赛德拉可asdasd适当卡事件代理卡事件代理看俺就打了卡就是来打开俺就',
    avatar: 'https://avatars.githubusercontent.com/u/1905176?v=4'
  },
  {
    id: 2,
    title: 'test2的专栏',
    description:
      '这是阿达克鲁赛德拉可asdasd适当卡事件代理卡事件代理看俺就打了卡就是来打开俺就',
    avatar: undefined
  },
  {
    id: 2,
    title: 'test2的专栏',
    description:
      '这是阿达克鲁赛德拉可asdasd适当卡事件代理卡事件代理看俺就打了卡就是来打开俺就',
    avatar: 'https://avatars.githubusercontent.com/u/1905176?v=4'
  },
  {
    id: 2,
    title: 'test2的专栏',
    description:
      '这是阿达克鲁赛德拉可asdasd适当卡事件代理卡事件代理看俺就打了卡就是来打开俺就',
    avatar: 'https://avatars.githubusercontent.com/u/1905176?v=4'
  }
]

export default defineComponent({
  name: 'App',
  components: {
    ColumnList,
    GlobalHeader
  },
  setup() {
    return {
      list: testData,
      currentUser
    }
  }
})
</script>

<style></style>
