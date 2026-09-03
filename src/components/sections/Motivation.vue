<script setup>
import motivation from '../mds/motivation.mdx';
import motivationInsight from '../mds/motivation_insight.mdx';
</script>

<template>
  <div v-animate-onscroll="'animated fadeInUp'">
    <el-row justify="center">
        <el-col :xs="28" :sm="24" :md="20" :lg="16" :xl="12">
          <h1>Motivation</h1>
            <div class="caption-box">
                <el-image src="./motivation.png" class="caption-img" fit="cover" />
                <motivation class="caption-text" />
            </div>
            <div class="insight-box">
                <motivationInsight />
            </div>
        </el-col>
    </el-row>

  </div>
</template>

<style scoped>

.caption-box {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 20px 0;
    gap: 40px;
}

.caption-img {
  width: 150%;
  max-width: 420px;
  border-radius: 12px;
  border: 1px solid var(--pcd-border);
  box-shadow: var(--pcd-shadow-soft);
}

.caption-text {
    margin-left: 10px;
}

/* Key Insight 强调框 */
.insight-box {
    margin: 20px 0;
    padding: 14px 20px;
    border-left: 4px solid var(--pcd-accent);
    border-radius: 0 10px 10px 0;
    background: rgba(50, 115, 220, 0.06);
}

.insight-box p {
    margin-block: 0.3em;
}

</style>
