<script setup>
import WelcomeItem from './WelcomeItem.vue'
import DocumentationIcon from './icons/IconDocumentation.vue'
import ToolingIcon from './icons/IconTooling.vue'
import EcosystemIcon from './icons/IconEcosystem.vue'
import CommunityIcon from './icons/IconCommunity.vue'
import SupportIcon from './icons/IconSupport.vue'
</script>

<template>
  <WelcomeItem>
    <template #icon>
      <DocumentationIcon />
    </template>
    <template #heading>Details</template>

    Hello
    
    I am Labiba Tanjim, studying bachelors of IT at deakin university. My hobby is to read books and my aim is to be a software developer.
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>Experience</template>

    This have worked with 
    <a href="https://www.kmart.com.au/womens/" >Kmart</a>
    <a href="https://www.lovisa.com.au/collections/gold-plated?gclid=CjwKCAjw4P6oBhBsEiwAKYVkq8_Zl8_1V1WslSnZGrQ0Rbdkq8cOcbgYb_DPwp_vjx3K_ZhDrRwu7BoCKA0QAvD_BwE&gclsrc=aw.ds&utm_campaign=Branded%20Search%20AU&utm_medium=cpc&utm_source=Google">Lovisa</a> 
    
    

    <br />

    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <EcosystemIcon />
    </template>
    <template #heading>Skills</template>

    I am proficient at:
    Communication
    Presenting
    Commitment
    Data managing
    Programming Languages
    
   
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <CommunityIcon />
    </template>
    <template #heading>Contact</template>

    Ask your question or contact at
    <a href="labibatanjimrida@gmail.com" target="_blank" rel="noopener">Email</a>, or
    Phonw 09897643
    <a href="https://news.vuejs.org" target="_blank" rel="noopener">Facebook</a> 


    <a href="https://twitter.com/vuejs" target="_blank" rel="noopener">LinkedIn</a>
    
  </WelcomeItem>

  <WelcomeItem>
    <template #icon>
      <SupportIcon />
    </template>
    <template #heading>Thanks</template>

    Thanks for spending your valuable time in my porfolio. Hope to hear from you soon!
    
  </WelcomeItem>
</template>
