<template>
  <div>
    <!-- <Header /> -->
    <!-- <div v-if="isLoading">is loading</div>
    <div v-if="isError">err</div>
    <div v-if="hospitals && hospitals.length"> -->
      <!-- <Hospitalcard
        v-for="item in hospitals"
        :key="item.id"
        :address="item.address.woreda"
        :availability="item.availability"
        :photo="item.photo"
        :phoneNumbers="item.phoneNumbers"
        :emails="item.emails"
      /> -->
    <!-- </div> -->
    <detailSocialMediaPage />
  </div>
</template>

<script>
import detailSocialMediaPage from './components/detail-social-media-page'
//  import Header from '../components/Header';
// import Hospitalcard from '@/components/Hospitalcard';
// import { useGetHospitadataQuery } from "@/redux/hosApi";

export default {
  components: {
    detailSocialMediaPage
    // Header,
    // Hospitalcard
  },
  
};
</script>
