<template>
<div class="overallDivs">  
  <card class="cardSigup text-center">
   <btn id="button" v-on:click.native="slack" type="button" class="googleButtons btn btn-google-plus">ChatBox</btn>
<a href="https://slack.com/oauth/authorize?client_id=372028459318.370611099329&scope=admin,incoming-webhook"><img alt="Add to Slack" height="40" width="139" src="https://platform.slack-edge.com/img/add_to_slack.png" srcset="https://platform.slack-edge.com/img/add_to_slack.png 1x, https://platform.slack-edge.com/img/add_to_slack@2x.png 2x" /></a>
  </card>
</div>
<!-- <ui-auth
    firebase="playground"
    google='email'
></ui-auth> -->
</template>
<script>
import Btn from '../components/Button';
import Column from '../components/Col';
import Row from '../components/Row';
import Container from '../components/Container';
import Card from '../components/Card';
import CardBody from '../components/CardBody';

export default {
  // el: '#button',
  name: 'JustDeploy',
  components: {
    Btn,
    Column,
    Row,
    Container,
    Card,
    CardBody,
  },
  data(){
    return {
      // firebase: 'playground',
      // providers: ['google'],
      // scopes: {
      //   google: 'email',
      // }
    };
  },
  methods: {
    slack() {
      console.log("hfgsdjh");
    }
  }
};
</script>
<style>
.overallDivs{
    margin-top: 4em;
    padding: 7% 0;
}
.cardSigup{
    width: 50% !important;
    margin: auto !important;
    height: 650px !important;
    border-radius: 4px !important;
  }
  .logoImgs{
    margin: 4em auto 2em auto !important;
    width: 35% !important;
  }
  .googleButtons{
    margin: 2em auto 3em auto !important;
    background: #ca3523 !important;
    border-radius: 3px !important;
    text-transform: none !important;
    width: 50% !important;
    height: 9% !important;
    font-size: 17px !important;
  }
 @media only screen and (min-width: 300px) and (max-width: 639.98px)
 {
 .cardSigup{
   width: 100% !important;
   height: 650px !important;
   padding: 1em !important;
 }
 .googleButtons{
    font-size: 14px !important;
    width: 80% !important;
 }
 .logoImgs{
     margin: 4em auto 2em auto !important;
    width: 60% !important;
 }
}
@media only screen and (min-width: 640px) and (max-width: 800px){
 .cardSigup {
    width: 70% !important;
   padding: 2em !important;
 }
 .googleButtons{
    font-size: 14px !important;
    width: 70% !important;
 }
 }
</style>