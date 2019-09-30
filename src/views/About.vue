<template>
  <div class="about">
    <v-layout row>
      <v-flex xs12 sm12>
        <v-card>
          <v-toolbar color="indigo" dark>
            <v-toolbar-title>Habilidades</v-toolbar-title>

            <v-spacer></v-spacer>
          </v-toolbar>
          <v-list>
            <v-list-tile v-for="item in items" :key="item.title" avatar @click>
              <v-list-tile-action>
                <v-icon v-if="item.icon" color="pink">star</v-icon>
              </v-list-tile-action>

              <v-list-tile-content>
                <v-list-tile-title v-text="item.title"></v-list-tile-title>
              </v-list-tile-content>
            </v-list-tile>
          </v-list>
        </v-card>
      </v-flex>
    </v-layout>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        { title: "Desenvolvedor FullStack" },
        {
          title:
            "Experiência com frontend web com ReactJS, Angular 7, JSP, JSF/Primefaces"
        },
        { title: "Experiência Mobile com React Native" },
        {
          title:
            " Experiência com Backend Web com Node, Spring Boot, Java, JDBC e JPA/Hibernate"
        },
        { title: "Experiência com RESTful Web Service e SOAP" },
        {
          title: "Experiência com relatórios utilizando o Jasper Studio"
        },
        { title: "Experiência com GIT, Maven, Yarn e Npm" },
        {
          title:
            "IDEs utilizadas para desenvolvimento Eclipse, Netbeans e VS Code"
        },
        {
          title: "Banco de dados utilizados Mysql, Sql Server e Postgres"
        }
      ]
    };
  }
};
</script>
