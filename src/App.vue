<template>
  <div id="app">
  <StyledCard>
    <StyledImage :src="mainImage"/>
    <Title>Fashion</Title>
    <StyledText>
Fashion is populaar especially in clothing , footwear, lifestyle, accessories, makeup, hairstyle and body.
    </StyledText>
    <BottomRow>
      <StyledAuthorImage :src="authorImage"/>
      <Author>Bob</Author>
      <Icon class="material-icons">favorite_border</Icon>
      <IconText>340</IconText>
      <Icon class="material-icons">chat_bubble_outline</Icon>
      <IconText>340</IconText>
    </BottomRow>
  </StyledCard>  
  </div>
</template>


<script>
import styled from 'vue-styled-components';


const StyledCard = styled.div`
height:100%;
  padding:1.5rem;
border-radius:0.5rem;
background:#f3f3f3;
max-width:50vh;
margin-top:50px;
box-shadow:8px 8px 10px #e0e0e0,-2px -2px 15px #ffffff;
`;

const StyledImage = styled.img`
max-width:100%;
border-radius:0.5rem;
box-shadow: 0 16px 24px 2px rgba(0,0,0,0.14),
0 6px 30px 5px rgba(0,0,0,0.12), 0 8px 10px -7px rgba(0,0,0,0.2);
`;

const Title = styled.h1`
color:#522cad;
font-size:2.075rem;
margin-bottom:0.5rem;
`;

const StyledText = styled.div`
color:#888888;
font-size:0.9rem;
line-height:1.5;
margin-bottom:1rem;
`;

const BottomRow = styled.div`
display:flex;
align-items:center;
justify-content:space-between;
`;

const StyledAuthorImage = styled.img`
width:50px;
height:50px;
object-fit:cover;
border:2px solid #522cad;
padding:5px;
border-radius:50%;

`;

const Author = styled.div`
margin-left:1rem;
flex:1;
color:#522cad;
`;
const Icon = styled.span`
margin:0 0.5rem 0 1.5rem;
color:#522cad;
`;

const IconText = styled.div`
color:#888888;
`;
export default {
  name: "App",
  
components:{
  StyledCard,
  StyledImage,
  Title,
  StyledText,
  BottomRow,
  StyledAuthorImage,
  Author,
  IconText,
  Icon,

},
data:function(){
  return{
      mainImage:require("@/assets/images/blog.jpg"),
      authorImage:require("@/assets/images/author-1.jpg")

  }
}
};
</script>

<style>
#app{
  display:flex;
  flex:1;
  justify-content:center;
  align-items:center;
  height:100%;
  width:100%;
}
</style>
