<template>
  <div>
    <md-tabs md-sync-route md-alignment="centered">
      <md-tab id="tab-home" md-label="Tabla" to="/components/tabs/home">
        <tableC :items="this.itemsTable" />  
      </md-tab>

      <md-tab id="tab-pages" md-label="DatePicker" to="/components/tabs/pages">
       <md-datepicker v-model="selectedDate" />
      </md-tab>

      <md-tab id="tab-posts" md-label="alert" to="/components/tabs/posts">
        <md-dialog-alert :md-active.sync="first" md-content="alert" md-confirm-text="Cool!" />
         <md-button class="md-accent md-raised" @click="first = true">Alert</md-button>
        </md-tab>
      <md-tab id="tab-favorites" md-label="Favorites" to="/components/tabs/favorites">
        Favorites tab
        <p>Maiores, dolorum. Beatae, optio tempore fuga odit aperiam velit, consequuntur magni inventore sapiente alias sequi odio qui harum dolorem sunt quasi corporis.</p>
      </md-tab>
    </md-tabs>
  </div>
</template>

<script>
import TableComponent from './TableComponent'
export default {
  name: 'TabContent',
  components:{
    tableC: TableComponent
  },
  data(){
      return{
          first: false,
          selectedDate:'',
          itemsTable:[
        {
          id: 1,
          name: "Shawna Dubbin",
          email: "sdubbin0@geocities.com",
          gender: "Male",
          title: "Assistant Media Planner"
        },
        {
          id: 2,
          name: "Odette Demageard",
          email: "odemageard1@spotify.com",
          gender: "Female",
          title: "Account Coordinator"
        },
        {
          id: 3,
          name: "Vera Taleworth",
          email: "vtaleworth2@google.ca",
          gender: "Male",
          title: "Community Outreach Specialist"
        },
        {
          id: 4,
          name: "Lonnie Izkovitz",
          email: "lizkovitz3@youtu.be",
          gender: "Female",
          title: "Operator"
        },
        {
          id: 5,
          name: "Thatcher Stave",
          email: "tstave4@reference.com",
          gender: "Male",
          title: "Software Test Engineer III"
        },
        {
          id: 6,
          name: "Karim Chipping",
          email: "kchipping5@scribd.com",
          gender: "Female",
          title: "Safety Technician II"
        },
        {
          id: 7,
          name: "Helge Holyard",
          email: "hholyard6@howstuffworks.com",
          gender: "Female",
          title: "Internal Auditor"
        },
        {
          id: 8,
          name: "Rod Titterton",
          email: "rtitterton7@nydailynews.com",
          gender: "Male",
          title: "Technical Writer"
        },
        {
          id: 9,
          name: "Gawen Applewhite",
          email: "gapplewhite8@reverbnation.com",
          gender: "Female",
          title: "GIS Technical Architect"
        },
        {
          id: 10,
          name: "Nero Mulgrew",
          email: "nmulgrew9@plala.or.jp",
          gender: "Female",
          title: "Staff Scientist"
        },
        {
          id: 11,
          name: "Cybill Rimington",
          email: "crimingtona@usnews.com",
          gender: "Female",
          title: "Assistant Professor"
        },
        {
          id: 12,
          name: "Maureene Eggleson",
          email: "megglesonb@elpais.com",
          gender: "Male",
          title: "Recruiting Manager"
        },
        {
          id: 13,
          name: "Cortney Caulket",
          email: "ccaulketc@cbsnews.com",
          gender: "Male",
          title: "Safety Technician IV"
        },
        {
          id: 14,
          name: "Selig Swynfen",
          email: "sswynfend@cpanel.net",
          gender: "Female",
          title: "Environmental Specialist"
        },
        {
          id: 15,
          name: "Ingar Raggles",
          email: "iragglese@cbc.ca",
          gender: "Female",
          title: "VP Sales"
        },
        {
          id: 16,
          name: "Karmen Mines",
          email: "kminesf@topsy.com",
          gender: "Male",
          title: "Administrative Officer"
        },
        {
          id: 17,
          name: "Salome Judron",
          email: "sjudrong@jigsy.com",
          gender: "Male",
          title: "Staff Scientist"
        },
        {
          id: 18,
          name: "Clarinda Marieton",
          email: "cmarietonh@theatlantic.com",
          gender: "Male",
          title: "Paralegal"
        },
        {
          id: 19,
          name: "Paxon Lotterington",
          email: "plotteringtoni@netvibes.com",
          gender: "Female",
          title: "Marketing Assistant"
        },
        {
          id: 20,
          name: "Maura Thoms",
          email: "mthomsj@webeden.co.uk",
          gender: "Male",
          title: "Actuary"
        }
      ]
      }

    },
    methods:{
        
  }
}
</script>
