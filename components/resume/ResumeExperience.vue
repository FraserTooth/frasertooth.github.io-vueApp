<template>
  <v-card width="60vw">
    <v-flex class="text-center">
      <v-card-title class="headline">Experience</v-card-title>
      <v-card-subtitle>Places I've worked.</v-card-subtitle>

      <v-list-group>
        <template v-slot:activator>
          <v-list-item-title>KiWi Power Ltd. (2017 - 2019)</v-list-item-title>
        </template>

        <v-list-item>
          <v-list-item-content>
            <p>
              Worked with
              <a href="https://www.kiwipowered.com/">KiWi Power</a> for 2 years in a variety of roles as the company grew to be a world leader in Demand Response
            </p>
          </v-list-item-content>
        </v-list-item>

        <v-list-group no-action sub-group>
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Head of Hardware Solutions (01/2019 – 04/2019)</v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item>
            <v-list-item-content>
              <p>Led a team supporting the work of the Technology, Sales, Installation and Operational teams to solve Hardware challenges.</p>
              <p>Our work involved acting as 'subject matter experts' for our hardware, business systems and 3rd party integrations.</p>
              <p>Led the certification process for our IoT Energy Management Product 'Fruit' to achieve UL2900-2-2 and UL Safety Certification</p>
              <p>Onboarding of new manufacturers. Ran the hiring process in the Firmware team</p>
              <p>Engagement with external partners to assist in the technical analysis of new business opportunities.</p>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>

        <v-list-group sub-group no-action>
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Product Owner (01/2018 – 04/2019)</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item>
            <v-list-item-content>
              <p>Ownership of all legacy and new Internet of Things hardware, guiding the firmware team, developing specifications with business owners and managing feature priorities.</p>
              <p>Also wrote TDD code for bug fixing and small features in the ‘Electric Imp platform’ language Squirrel and companion testing framework ‘Nutkin’.</p>
              <p>Role involved Agile management, documentation, business analysis using MySQL and Python, basic Android app development, physical hardware builds, policy engagement and lobbying, testing, prototyping and competitor research.</p>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>

        <v-list-group sub-group no-action>
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Support/QA Engineer (01/2017 – 01/2019)</v-list-item-title>
            </v-list-item-content>
          </template>
          <v-list-item>
            <v-list-item-content>
              <p>My role was to own the resolution of operational problems, support product development and solve unique project challenges.</p>
              <p>QA tasks: Bug diagnostics in our hardware and web services, automation of manual team tasks and ensuring commissioning best practice.</p>
              <p>Support tasks: sourcing and testing equipment, automated testing maintenance and code level bug analysis in C & Squirrel.</p>
              <p>Also supported various one-off projects such as an ‘SQL/Influx to modbus to voltages’ interface built with a RaspberryPi and NodeRed.</p>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
      </v-list-group>

      <v-list-group>
        <template v-slot:activator>
          <v-list-item-title>Peter Brett Associates (06/2015 – 01/2017)</v-list-item-title>
        </template>

        <v-list-item>
          <v-list-item-content>
            <p>
              Worked at
              <a href="https://www.peterbrett.com/">Peter Brett Associates</a> as a graduate engineer.
            </p>
          </v-list-item-content>
        </v-list-item>

        <v-list-group no-action sub-group>
          <template v-slot:activator>
            <v-list-item-content>
              <v-list-item-title>Graduate M&E Engineer (06/2015 – 01/2017)</v-list-item-title>
            </v-list-item-content>
          </template>

          <v-list-item>
            <v-list-item-content>
              <p>Member of the Buildings team specialising in electrical distribution and lighting for new builds, retrofits, highways and car parks.</p>
              <p>Used Amtech, Dialux and AutoCad regularly as well using Excel to perform automatic design checks.</p>
              <p>Projects include London Underground LED lighting renovations, environmental lighting assessments for planning and ‘Local Government House’ Refurbishment.</p>
              <p>Co-ordinator for local college STEM partnership, where we built an LED art installation using Arduino.</p>
            </v-list-item-content>
          </v-list-item>
        </v-list-group>
      </v-list-group>
    </v-flex>
  </v-card>
</template>
