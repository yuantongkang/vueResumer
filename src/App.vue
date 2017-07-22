<template>
  <div class=page>
    <header>
      <Topbar/>
    </header>
    <main>
      <ResumeEditor />
      <ResumePreview />
    </main>
  </div>
</template>



<script>
import 'normalize.css/normalize.css'
import './assets/reset.css'
import Topbar from './components/Topbar'
import ResumePreview from './components/ResumePreview'
import ResumeEditor from './components/ResumeEditor'


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
.page {
  height: 100vh;
  display: flex;
  flex-direction: column;
}

.page>main {
  flex-grow: 1;
}

.page>main {
  min-width: 1024px;
  max-width: 1440px;
  align-self: center;
  width: 100%;
  margin-top: 16px;
  margin-bottom: 16px;
  display: flex;
  justify-content: space-between;
  padding: 0 16px;
}

#resumeEditor {
  width: 35%;
  background: #444;
}

#resumePreview {
  flex-grow: 1;
  margin-left: 16px;
  background: #777;
}
</style>
