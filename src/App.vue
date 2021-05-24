<template>
  <div id="app">
  <Card>
    <Image :src="mainImage"/>
    <Title>Fashion</Title>
    <Text>
Fashion is populaar especially in clothing , footwear, lifestyle, accessories, makeup, hairstyle and body.
    </Text>
    <BottomRow>
      <AuthorImage :src="authorImage"/>
      <Author>Bob</Author>
      <MdHeartEmptyIcon w="70px" h="70px"/>
      <IconText>340</IconText>
      <IconText>340</IconText>

    </BottomRow>
  </Card>  
  </div>
</template>


<script>
import styled from 'vue-styled-components';
import MdHeartEmptyIcon from 'vue-ionicons/dist/md-heart-empty.vue'
    
const Card = styled.div`

`;


export default {
  name: "App",
  
components:{
  Card,
  MdHeartEmptyIcon,
  
},
data(){
return{
mainImage:require('@assets/')
}
}
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
