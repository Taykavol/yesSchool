<template>
  <div class="  ">
    <b-tabs type="is-boxed" position="is-centered" :multiline="true" expanded>
      <b-tab-item   >
          <div  slot="header" class="text-2xl font-semibold">
              Английский язык
          </div>
          <div class="flex flex-wrap justify-evenly mx-4">
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          </div>
      </b-tab-item>
      <b-tab-item label=" язык" >
          <div slot="header" class="text-2xl font-semibold ">
              Немецкий язык
          </div>
         <div class="flex flex-wrap justify-evenly">
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          </div>
      </b-tab-item>
      <b-tab-item label="Японский язык" >
          <div  slot="header" class="text-2xl font-semibold">
              Японский язык
          </div>
          <div class="flex flex-wrap justify-evenly">
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          <Card src="https://previews.123rf.com/images/luplupme/luplupme1907/luplupme190700594/129453972-british-english-language-learning-class-vector-illustration-brittish-flag-logo-england-dictionary-bi.jpg"/>
          </div>
      </b-tab-item>
    </b-tabs>
  </div>
</template>

<script>
import GalleryEng from '@/components/GalleryEng'
import Card from '@/components/Card'
export default {
    components:{
        GalleryEng,Card
    }
};
</script>

<style lang="scss" scoped>
.tabSlot {
    &:hover {
    }
    &:visited {
    }
}
</style>
