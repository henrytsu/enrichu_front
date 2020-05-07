<template>
    <aside id="aside">
      <div class="menu-toggle" @click.prevent="collapse">
        <i class="iconfont icon-outdent" v-show="!collapsed" title="收起"></i>
        <i class="iconfont icon-indent" v-show="collapsed" title="展开"></i>
      </div>
    </aside>
</template>