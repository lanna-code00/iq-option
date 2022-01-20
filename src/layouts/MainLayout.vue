<template>
  <q-layout view="hHh lpr lFf" class="all-background">

    <q-header bordered class="text-grey-6 main-header">
      <q-toolbar>

        <q-toolbar-title>
      <div class="row justify-start q-gutter-lg">
          <q-avatar size="sm" class="q-py-sm">
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg">
          </q-avatar>
          <span class="q-ml-sm q-py-sm text-body1">iq option</span> 
            
                
                <div class="listfont-div">
                  <q-btn 
                 flat 
                 round 
                 color="grey-6" 
                 icon="fas fa-th-list"
                 size="md"
                 class="list_button"
                />
                </div>
<!-- 
              <div class="top-divs">
                 <div class="text-body1 q-py-sm">
                   <div>
                     <q-icon name="fas fa-envelope" class="q-ml-sm" color="yellow"/>
                     <span class="q-ma-sm">Field Content</span>
                     <span class="text-caption">Field Content</span>
                     <div class="row">
                     </div>
                   </div>
                    
                 </div>
              </div>
              
                <div>

                </div>

                   <q-btn 
                 flat 
                 round 
                 color="grey-5" 
                 icon="far fa-heart"
                 size="sm" 
                />

                <q-btn 
                 flat 
                 round 
                 color="grey-5" 
                 icon="fas fa-trash"
                 size="sm" 
                /> -->
        </div>
        </q-toolbar-title>
  
      </q-toolbar>
    </q-header>

    <q-drawer show-if-above v-model="leftDrawerOpen" side="left" bordered class="sidebar-drawer bg-blue-grey-10">
      <div class="row ">
      <div class="col-3">
            <q-list bordered class="qlistSidebar">
            <div >
            <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-lock" />
              </q-item-section>
            </q-item>
           <span class=" text-weight-medium text-center text-changes q-ma-sm text-grey-8">TOTAL
            </span>
              <span class=" text-weight-medium text-center text-changes q-ma-sm text-grey-8 ">PROFITS
            </span>
            </div>  

            <div>
           <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-clock" />
              </q-item-section>

            </q-item>
              <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 ">TRADING
            </span>
              <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 ">HISTORY
            </span>
            </div>

            <div>
              <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-comments" />
              </q-item-section>
            </q-item>
             <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">CHATS $  
            </span>
                <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">SUPPORT </span>
            </div>

            <div>
             <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-award" />
              </q-item-section>
            </q-item>
              <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">LEADER  
            </span>
                <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">BOARD </span>
            </div>

            <div>
             <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-chart-line" />
              </q-item-section>
            </q-item>
              <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">MARKET  
            </span>
                <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">ANALYSIS </span>
       </div>

            <div>
             <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-play-circle" />
              </q-item-section>
            </q-item>
            <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">VIDEO  
            </span>
                <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">TUTORIALS </span>
            </div>

            <div>
            <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class" name="fas fa-ellipsis-h" />
              </q-item-section>
            </q-item>
            <span class="q-ml-md q-mt-sm text-weight-medium text-center text-changes q-ma-sm text-grey-8 justify-center">MORE  
            </span>
            </div>

            </q-list>
      </div>
      <div class="col-9 qListNotifs">
        
        <q-list >
         <q-item class="notifs">
        <q-item-section avatar class="q-mt-lg q-mb-md">
          <q-circular-progress
        show-value
        class="text-grey-8"
        :value="value"
        size="35px"
        track-color="grey-8"
        color="grey-5"
      />
        </q-item-section>

        <q-item-section class="q-mt-lg q-mb-md">
          <q-item-label caption lines="2" class="text-grey-5">Secondary line text. Lorem ipsum dolor sit amet, consectetur adipiscit elit.</q-item-label>
        </q-item-section>

        <q-item-section side top>
          <q-icon name="fas fa-times" color="grey-8" />
        </q-item-section>
      </q-item>
      
      <q-separator color="grey-8"></q-separator>

         <q-item>
        <q-item-section avatar class="">
          <q-icon name="fas fa-check-circle" class="check-class" color="positive" />
        </q-item-section>

        <q-item-section class="">
          <q-item-label lines="1" class="text-grey-5 text-strike">Secondary line text. </q-item-label>
        </q-item-section>
      </q-item>

      <q-separator color="grey-8"></q-separator>

      <q-item clickable v-ripple>
        <q-item-section avatar top>
          <q-badge rounded size="md" color="grey-8" label="2" />
        </q-item-section>

        <q-item-section class="">
          <q-item-label class="text-white">Single line item</q-item-label>
          <q-item-label caption lines="4" class="text-grey-5">Secondary line text. This is what am going to be doing. Is this </q-item-label>
        </q-item-section>
      </q-item>

      <q-separator color="grey-8"></q-separator>

      <q-item>
        <q-item-section avatar class="">
          <q-badge rounded size="md" color="grey-8" label="3" />
        </q-item-section>

        <q-item-section class="">
          <q-item-label lines="1" class="text-grey-5">Your Fist Forecast</q-item-label>
        </q-item-section>
      </q-item>

      <q-separator color="grey-8"></q-separator>

      <q-item>
        <q-item-section avatar class="">
          <q-icon name="fas fa-check-circle" class="check-class" color="positive" />
        </q-item-section>

        <q-item-section class="">
          <q-item-label lines="1" class="text-grey-5 text-strike">Confirm your email</q-item-label>
        </q-item-section>
      </q-item>

      <q-separator color="grey-8"></q-separator>

    <q-item clickable v-ripple>
        <q-item-section avatar top>
          <q-badge rounded size="md" color="grey-8" label="5" />
        </q-item-section>

        <q-item-section class="">
          <q-item-label class="text-white">Top up your account</q-item-label>
          <q-item-label class="text-grey-5">
          </q-item-label>
        </q-item-section>
      </q-item>
        <div class="row q-mb-md">
          <div class="col-12 q-px-md">
            <q-btn unelevated color="positive" class="stretch-button" label="deposit" />

          </div>
        </div>

      <q-separator color="grey-8"></q-separator>

        </q-list>
      </div>
    </div>
    </q-drawer>

   <q-drawer show-if-above v-model="rightDrawerOpen" side="right" bordered>
      <!-- drawer content -->
     </q-drawer> 

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer class="text-white main-footer">
      <q-toolbar>
        <q-toolbar-title>
          
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>

  </q-layout>
</template>

<script>
import { ref } from 'vue'

export default {
  data(){
    return {
      value: 43
    }
  },
  setup () {
    const leftDrawerOpen = ref(false)
    const rightDrawerOpen = ref(false)

    return {
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      },

      rightDrawerOpen,
      toggleRightDrawer () {
        rightDrawerOpen.value = !rightDrawerOpen.value
      }
    }
  }
}
</script>

<style lang="sass" scoped>
.main-header
   background-color: #1B192F
   border-bottom: 1px solid $grey-8
.main-footer
   background-color: #1B192F
.icon-div
   border: 1px solid $grey-8  
.listfont-div 
   border-top: 1px solid
   border-top-left: 1px solid
   border-top-right: 1px solid
   border-bottom: 1px solid 
   border: 1px solid $grey-8
   height: 38px
.list_button 
   margin-top: -3px   
.top-divs
   border-bottom: 1px solid $amber-10
   background-color: #37344E 
   height: 38px
.text-changes
   font-size: 10px
.icons-class
   font-size: 15px   
.qlistSidebar
    font-size: 10px
    margin: 0px
    padding: 0px
    background-color: #1B192F
    height: 92vh !important
    border-right: 1px solid $grey-8
.qlistSidebar
   q-item
     margin: 2px
     padding: 0px  
.notifs
   background-color: #29273F
.qListNotifs  
    background-color: #1B192F
.check-class
   font-size: 20px 
.stretch-button
   width: 100%        
</style>