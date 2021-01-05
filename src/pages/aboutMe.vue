<template>
  <q-page padding>
    <!-- content -->
    <div class="q-pa-md">
      <q-card class="My card">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/hDbVPuUYWN4" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
        </iframe>
        <q-card-section>
            <div class="text-h6">What is vue.js?</div>
            <div class="my-card text-subtitle1 bg-green text-white">VUE</div>
        </q-card-section>
        <br>
        <q-card-section class="q-pt-none" >
          <div class="borders text-h5">ในสายตาของคนทั่วไปมันคือ Angular ผสมกับ React เพื่อจัดการกับ Reactive Component หรือ คอมโพแนนท์อัจฉริยะที่สามารถอัพเดทตัวเองได้ แต่ในสายตาของผู้ใช้นั้น Vue.js คือ ศาสดาองค์ที่สองเลยทีเดียว
คุณลักษณะของ Vue.js
การจัดการประสิทธิภาพที่ดีกว่า -- Vue.js มีการทำงานแบบ reactive มันรู้ได้เองด้วยว่าจุดไหนของ template ควร render ใหม่หรือไม่ต้องทำอะไร ในเอกสารกล่าวว่ากระบวนการนี้ไม่จำเป็นต้องใช้ shouldComponentUpdate หรือ immutable เหมือน React แม้แต่น้อย
Component System -- Vue.js มีความเหมือน React ตรงที่มีความเป็นคอมโพแนนท์ เราสามารถห่อหุ้มโค๊ดของ UI Component ที่สัมพันธ์กันไว้ใต้คอมโพแนนท์เดียวกันได้เช่นเดียวกับ React
สนับสนุนการใช้งาน JSX และ Hyperscript -- Vue.js นั้นดูยังไงก็คล้าย Angular มากกว่า React เพราะ template ของ Vue.js นั้นเป็น HTML-centric เหมือน Angular กล่าวคือ Vue.js เลือกใช้หนทางในการเพิ่มไวยากรณ์ใหม่ลงไปใน template เพื่อจัดการการแสดงผลหรือเหตุการณ์ต่างๆ</div>
          </q-card-section>
              </q-card>
    </div>
            <q-card class="my-cards">
      <q-card-section horizontal>
        <q-img
          class="col-5"
          src="https://www.borntodev.com/wp-content/uploads/2020/07/facebook-cover-blog-1.jpg"
        />
        <q-card-section>
          {{ ivue }}
        </q-card-section>
      </q-card-section>

      <q-separator />

      <q-card-actions>
        <q-btn flat round icon="east" />
        <q-btn flat>
          More Info
        </q-btn>
        <q-btn flat>
          Goto website
        </q-btn>
        <q-btn flat color="primary">
          Facebook
        </q-btn>
      </q-card-actions>
    </q-card>
          <q-card
      class="my-cardz text-white"
      style="background: radial-gradient(circle, #7ade7a 0%, #018801 100%)"
    >
          <q-card-section>
            <div class="text-h6">Vue.js 101</div>
            <div class="text-subtitle2">by BorntoDev</div>
          </q-card-section>
        <q-card-section class="q-pt-none">
          {{ ivue }}
        </q-card-section>
          </q-card>
    <div class="left">
    <q-btn icon="home" to="/" label="Go Home" outline color="green" />
    </div>

  </q-page>
</template>

<script>
export default {
  data () {
    return {
      ivue: 'Vue อ่านว่า “วิว” เหมือนกับคำว่า view เลย โดยเป็น “progressive framework” สำหรับสร้าง user interface ซึ่ง progressive ก็คือการที่ Vue.js นั้นใช้เป็นเหมือนส่วนเพิ่มความสามารถที่เอาไปใช้งานกับ HTML ซึ่งชื่อ Vue นั้นก็มีที่มาจากการที่ library นี้จะโฟกัสที่การจัดการในส่วนของ view เท่านั้น เพื่อให้สามารถนำ Vue ไปใช้งานร่วมกับ Library อื่นๆได้สะดวก และยังเหมาะกับการทำ Single-Page Applications (SPA) หรือเว็บที่ไม่ต้องเปลี่ยนหน้าบ่อยๆนั่นเอง'
    }
  }
}
</script>
<style lang="sass" scoped>
.my-card
  width: 100%
  max-width: 300px
  position: relative
  margin: 10px
  overflow: auto
.borders
  border-style: solid
  border-color: green
  margin: 10px
.left
  margin: 0 600px
  position: relative
.right
  margin: auto
  text-align: center
  width: 100%
.my-cards
  float: right
  right: 200px
  overflow: auto
  width: 100%
  max-width: 600px
.my-cardz
  width: 100%
  max-width: 300px
  position: relative
  left: 200px
  margin: 10px
  overflow: auto
</style>
