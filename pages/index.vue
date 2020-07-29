<template>
  <div class="relative">
    <div class="h-screen">
      <div class="flex flex-col">
        <!-- 
          Header Content ( Landing Page )

          PARAMETERS
          :imgURL (URL for Background)
          :header_txt ( Header Text )
          :second_header ( Header 2 Text)
          :descriptions ( Descriptions )
        -->
        <HeaderContent
          imgURL="https://gdp.alicdn.com/imgextra/i2/2585692843/O1CN01J6WKsw1Ws8ceqWix4_!!2585692843.jpg"
          header_txt="DORAEMON TRADING"
          second_header="WE ARE DORAEMON FANATIC"
          descriptions="A Doraemon a day, keep your problems away."
        ></HeaderContent>
        <!-- 
          About Content 

          PARAMETERS
          :imgURL ( URL for about us )
        -->
        <AboutContent
          imgURL="https://img.alicdn.com/imgextra/i3/2585692843/O1CN0129PKx81Ws8UptNUUd_!!2585692843.jpg"
        >
          <template v-slot:about>We want to spread the posivity of Doraemon to the world.</template>
        </AboutContent>

        <ServiceContent>
          <template v-slot:services>
            <!-- 

              Service 

              PARAMETERS

              :imgURL (image url)
            -->
            <Service imgURL="/img/icon1.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon2.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon3.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon4.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon4.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>
          </template>
        </ServiceContent>

        <!-- 
          Portfolio
        -->
        <PortfolioContent>
          <template v-slot:portfolio>
            <!-- 
              Project

              PARAMETERS
              :imgURL ( img URL for Project )
              :name ( Name of the Project )
              :project ( Name of Project Type)
              :projectURL ( Link Address to project)
            -->
            <Project
              imgURL="https://img.alicdn.com/imgextra/i3/2585692843/O1CN01plbbEB1Ws8UrY7yMI_!!2585692843.jpg"
              name="Crafting"
              project="Kitchenware"
              projectURL="https://github.com/billyponpon/company-template"
            />

            <Project
              imgURL="https://img.alicdn.com/imgextra/i3/2585692843/O1CN01plbbEB1Ws8UrY7yMI_!!2585692843.jpg"
              name="Project Name"
              project="Project Type"
              projectURL="https://github.com/billyponpon/company-template"
            />

            <Project
              imgURL="https://img.alicdn.com/imgextra/i3/2585692843/O1CN01plbbEB1Ws8UrY7yMI_!!2585692843.jpg"
              name="Project Name"
              project="Project Type"
              projectURL="https://github.com/billyponpon/company-template"
            />

            <Project
              imgURL="https://img.alicdn.com/imgextra/i3/2585692843/O1CN01plbbEB1Ws8UrY7yMI_!!2585692843.jpg"
              name="Project Name"
              project="Project Type"
              projectURL="https://github.com/billyponpon/company-template"
            />
          </template>
        </PortfolioContent>
        <ContactContent
          address="Level 11, Menara KEN TTDI, No.37 Jalan Burhanuddin Helmi, Taman Tun Dr. Ismail"
          email="support@thelead.io"
          phone="6016-473 7281"
          imgURL="/img/lead-white-logo.png"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: "Doraemon Portfolio"
    };
  }
};
</script>