<template>
  <div>
    <TopBar/>
    <ResumeEditor/>
    <ResumePreview/>
  </div>
</template>



<script>
import './assets/reset.css'
import Topbar from './components/Topbar'
import ResumeEditor from './components/ResumeEditor'
import ResumePreview from './components/ResumePreview'


export default {
  name: 'app',
  data() {
    return {
      text: "hello"
    }
  },
  components: {
    Topbar, ResumeEditor, ResumePreview
  }
}
</script>

<style >

</style>
