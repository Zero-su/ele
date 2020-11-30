<template>
  <div style="margin: 20px;">
    <el-date-picker
      v-model="value1"
      type="datetimerange"
      format="yyyy-MM-dd HH:mm"
      :isDivide="true"
      range-separator="至"
      start-placeholder="开始日期"
      end-placeholder="结束日期">
    </el-date-picker>

    <el-date-picker
      v-model="value4"
      type="datetimerange"
      format="yyyy-MM-dd HH:mm"
      :isDivide="false"
      range-separator="至"
      start-placeholder="开始日期"
      end-placeholder="结束日期">
    </el-date-picker>
    
    <el-time-picker
    v-model="value2"
    :isDivide="true"
    format="HH:mm"
    placeholder="任意时间点">
    </el-time-picker>

    <el-time-picker
    v-model="value3"
    :isDivide="false"
    format="HH:mm"
    placeholder="任意时间点">
  </el-time-picker>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        value1: [],
        value4: [],
        value2: '',
        value3: '',
        input: 'Hello Element UI!'
      };
    }
  };
</script>
