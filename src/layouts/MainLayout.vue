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
            
                
                <div class="listfont-div1">
                  <q-btn 
                 flat 
                 round 
                 color="grey-6" 
                 icon="fas fa-th-list"
                 size="md"
                 class="list_button"
                />
                </div>

              <div class="listfont-div2">
                <q-icon name="fas fa-times" class="nav-icons" side top/>
                <q-btn 
                 flat 
                 round 
                 color="grey-6" 
                 icon="fas fa-th-list"
                 size="md"
                 class="list_button q-ml-sm"
                >
                <q-item clickable v-ripple class="q-pa-m">
                  <q-item-section>
                    <q-item-label class="nav-text text-weight-bolder">EUR/JPY (0</q-item-label>
                    <q-item-label class="nav-text text-weight-regular">Caption</q-item-label>
                  </q-item-section>
                  </q-item>

                </q-btn>
              </div>

              <div class="listfont-div3">
                <q-icon name="fas fa-times" class="nav-icons" side top/>
                <q-btn 
                 flat 
                 round 
                 color="grey-6" 
                 icon="fas fa-th-list"
                 size="md"
                 class="list_button q-ml-sm"
                >
                <q-item clickable v-ripple class="q-pa-m">
                  <q-item-section>
                    <q-item-label class="nav-text text-weight-bolder">EUR/USD (0</q-item-label>
                    <q-item-label class="nav-text text-weight-regular">Caption</q-item-label>
                  </q-item-section>
                  </q-item>

                </q-btn>
              </div>

                <div class="listfont-div1">
                  <q-btn 
                 flat 
                 round 
                 color="grey-6" 
                 icon="fas fa-plus"
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
              <div class="listfont-camera">
                    <q-btn 
                  flat 
                  round 
                  color="grey-6" 
                  icon="fas fa-camera"
                  size="md"
                  class="list_button"
                  />
                </div>

                 <div class="">
                    <q-btn 
                  flat 
                  round 
                  color="grey-6" 
                  icon="fas fa-caret-down"
                  size="sm"
                  class="list_button"
                  />
                </div>

                 <div class="">
                    <span class="text-body1 q-ml-md text-weight-bolder text-amber-10">$10,000.00</span>
                </div>

                  <div class="q-ml-sm">
                  <q-btn color="positive" size="md" icon="fas fa-dollar-sign" label="Deposit" />
                </div>

      </q-toolbar>
    </q-header>

    <q-drawer show-if-above v-model="leftDrawerOpen" side="left" bordered class="sidebar-drawer bg-blue-grey-10">
      <div class="row ">
      <div class="col-3 ">
            <q-list bordered class="qlistSidebar">
            <div style="cursor:pointer">
           <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-lock" />
                <span class="text-grey-8">TOTAL</span>
                <span class="text-grey-8">PROFIT</span>
              </q-item-section>
            </q-item>
          
            </div> 

            <div style="cursor:pointer">
           <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-clock" />
                <span class="text-grey-8">TRADING</span>
                <span class="text-grey-8">HISTORY</span>
              </q-item-section>
            </q-item>
    
            </div>

            <div style="cursor:pointer">
              <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-comments" />
                <span class="text-grey-8">CHATS</span>
                <span class="text-grey-8">&SUPPORT</span>
              </q-item-section>
            </q-item>
            </div>

            <div style="cursor:pointer">
             <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-award" />
                 <span class="text-grey-8">LEADER</span>
                <span class="text-grey-8">BOARD</span>
              </q-item-section>
            </q-item>
            </div>

            <div style="cursor:pointer">
             <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-chart-line" />
                  <span class="text-grey-8">MARKET</span>
                <span class="text-grey-8">ANALYSIS</span>
              </q-item-section>
            </q-item>
       </div>

            <div style="cursor:pointer">
             <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-play-circle" />
                <span class="text-grey-8">VIDEO</span>
                <span class="text-grey-8">TUTORIALS</span>
              </q-item-section>
            </q-item>
            </div>

            <div style="cursor:pointer">
            <q-item>
              <q-item-section avatar>
                <q-icon color="grey-8" class="icons-class q-ml-sm" name="fas fa-ellipsis-h" />
                <span class="text-grey-8">MORE</span>
              </q-item-section>
            </q-item>
            </div>

            </q-list>
      </div>
      <div class="col-9 qListNotifs">
        
        <q-list>
         <q-item class="notifs" clickable>
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
          <q-icon name="fas fa-times" color="white" size="xs"/>
        </q-item-section>
      </q-item>
      
      <q-separator color="grey-8"></q-separator>

         <q-item clickable>
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

      <q-item clickable>
        <q-item-section avatar class="">
          <q-badge rounded size="md" color="grey-8" label="3" />
        </q-item-section>

        <q-item-section class="">
          <q-item-label lines="1" class="text-grey-5">Your Fist Forecast</q-item-label>
        </q-item-section>
      </q-item>

      <q-separator color="grey-8"></q-separator>

      <q-item clickable>
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
          <q-item-label class="text-white">Top up your account
            
          </q-item-label>
          <q-item-label class="text-grey-5">
          </q-item-label>
        </q-item-section>
      </q-item>
        <div class="row q-mb-md">
          <div class="col-12 q-px-md">
            <q-btn unelevated color="positive" class="stretch-button" size="sm" label="deposit" />

          </div>
        </div>

      <q-separator color="grey-8"></q-separator>
        <div class="q-mt-sm q-pa-sm">
            <span style="font-size: 12px" class="text-white float-end">Might be useful
              <span class="q-ml-xl" style="color: grey; cursor:pointer">Show more</span>  
            </span> 
        </div>

       <q-img src="https://cdn.quasar.dev/img/parallax2.jpg" class="q-ml-lg" style="width: 180px">
           <div class="absolute-top text-center" style="background: none">
            How to trade in iq option
          </div>
          <div class="absolute-full text-subtitle2 flex flex-center">
              <q-icon name="fas fa-play" class="check-class q-mt-sm" color="white" />
          </div>
        </q-img>

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
        <q-toolbar-title style="margin-top: -20px">
             <span style="font-size: 13px" class="q-mt-sm">Total portfolio</span>
        </q-toolbar-title>
             <span style="font-size: 13px; margin-top: -20px" class="q-mt-sm text-grey">
               Show position <q-icon name="fas fa-caret-down" class="check-class text-grey" color="white" />

             </span>
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
   height: 35px
.icon-div
   border: 1px solid $grey-8  
.listfont-div1 
   border-top: 1px solid
   border-top-left: 1px solid
   border-top-right: 1px solid
   border-bottom: 1px solid 
   border: 1px solid $grey-8
   height: 38px
.listfont-div2 
   background-color: #37344E 
   border-bottom: 1px solid $amber-10
   height: 38px 
.listfont-div3 
   background-color: #37344E 
   border-bottom: 1px solid $amber-10
   height: 38px
.listfont-camera
   height: 38px 
   background-color: #37344E 
.list_button 
   margin-top: -3px   
.top-divs
   background-color: #37344E 
   height: 38px
   border-radius: 50px
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
.nav-text
   font-size: 70%  
.nav-icons
   font-size: 50%
   margin-bottom: 25px
   padding: 4px  
   font-color: $grey-2        
</style>