<template>
  <div id="app">
  <Card>
    <StyledImage :src="mainImage"/>
    <Title>Fashion</Title>
    <Text>
Fashion is populaar especially in clothing , footwear, lifestyle, accessories, makeup, hairstyle and body.
    </Text>
    <BottomRow>
      <AuthorImage :src="authorImage"></AuthorImage>
      <Author>Bob</Author>
      <MdHeartEmptyIcon w="70px" h="70px"></MdHeartEmptyIcon>
      <IconText>340</IconText>
      <IosChatboxesIcon w="20px" h=20px></IosChatboxesIcon>

      <IconText>340</IconText>
    </BottomRow>
  </Card>  
  </div>
</template>


<script>
import styled from 'vue-styled-components';
import MdHeartEmptyIcon from 'vue-ionicons/dist/md-heart-empty.vue'
import IosChatboxesIcon from 'vue-ionicons/dist/ios-chatboxes.vue'
    
const Card = styled.div`
  padding:1.5rem;
border-radius:0.5rem;
background:#f3f3f3;
width:100%;
box-shadow:8px 8px 10px #e0e0e0,-2px -2px 15px #ffffff;
`;

const StyledImage = styled.img`
max-width:100%;
border-radius:0.5rem;
transform:translateY(-40px);
box-shadow: 0 16px 24px 2px rgba(0,0,0,0.14),
0 6px 30px 5px rgba(0,0,0,0.12), 0 8px 10px -7px rgba(0,0,0,0.2);
`;


export default {
  name: "App",
  
components:{
  Card,
  MdHeartEmptyIcon,
  StyledImage,
  IosChatboxesIcon,
 
},
data:function(){
  return{
      mainImage:require("@/assets/images/blog.jpg"),
      authorImage:require("@/assets/images/author.jpg")

  }
}
};
</script>

<style>

</style>
