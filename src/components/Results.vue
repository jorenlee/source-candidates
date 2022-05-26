<template>
  <div>
    <div class="lg:mt-14 mt-5 mx-auto">
      <div class="mb-5 mx-auto block lg:w-1/12 w-4/12">
        <ul class="flex justify-between gap-2">
          <li>
            <img class="object-cover object-center lg:w-24 w-20" src="@/assets/logo/lsu-logo.png" alt="" />
          </li>
          <li>
            <img class="object-cover object-center lg:w-28 mt-1 w-24" src="@/assets/logo/source-logo.png" alt="" />
          </li>
        </ul>
      </div>
      <h1 class="text-center mb-14 text-xl font-extrabold text-transparent bg-clip-text bg-gradient-to-r from-green-400 to-green-600 lg:w-11/12 w-4/5 mx-auto">LSU Student Organization Utilizing the Realm of Computer Eclecticism <br>Election for Officers A.Y. 2022-2023<br> <span class="">List of All Candidates</span> </h1>
      <div class="mx-auto mb-20 lg:w-9/12">
        <div class="lg:grid lg:grid-cols-2 lg:gap-10 lg:justify-evenly">
          <!-- card-1 -->
            <div class="relative lg:w-10/12 w-11/12 mx-auto lg:mb-0 mb-10" v-for="(student, i) in students" :key="i">
              <!-- box-1 -->
              <div class="px-2">
                <div class="flex md:h-8 h-10 w-full rounded-t-lg border-b-2 border-slate-300 bg-green-800 shadow-lg">
                  <small class="lg:ml-24 ml-20 my-auto w-full lg:text-sm text-xs font-light tracking-tight text-white lg:whitespace-nowrap">FOR
                    <span class="uppercase">{{student.positionTitle}}</span>
                  </small>
                </div>
              </div>
              <!-- box-2 -->
              <div class="bg-gradient-to-r from-green-900 to-green-500 flex h-12 w-full rounded-lg bg-white shadow-xl">
                <div class="lg:ml-16 ml-12 mt-2">
                  <small class="lg:text-lg text-xs md:text-sm text-white font-bold whitespace-nowrap lg:mr-5 mr-3 ml-10">{{student.name}}</small> 
                  <span class="text-xs mt-3.5 text-white whitespace-nowrap">{{student.courseAndYear}}</span>
                </div>
              </div>
              <!-- circle -->
              <div class="absolute bg-white md:top-2 top-1 lg:left-6 md:left-4 -left-1 md:h-16 md:w-16 w-20 h-20 overflow-hidden rounded-full border-2 border-white shadow-md">
                <img class="rounded-full object-cover" :src="student.profileUrl" alt="" />
              </div>
            </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>


export default {
  name: 'App',
  components: {
    
  },
  data() {
    return {
      students: [
        {
          id: 1,
          name: 'Jessa Mae E. Dabon',
          positionTitle: 'President',
          courseAndYear: 'BSIT-2',
          profileUrl: require('@/assets/candidates/jessa.jpg')
        },
        {
          id: 2,
          name: 'Andres Edman G. Olario',
          positionTitle: 'President',
          courseAndYear: 'BSCS-2',
          profileUrl: require('@/assets/candidates/andres.jpg')
        },
        {
          id: 3,
          name: 'Harlie Quin Marc C. Quipit',
          positionTitle: 'Vice President',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/harlie.jpg')
        },
        {
          id: 4,
          name: 'Lord Emmanuel C. Figueras',
          positionTitle: 'Vice President',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/emman.jpg')
        },
        {
          id: 5,
          name: 'Edyr Ryle G. Ilisan',
          positionTitle: 'Secretary',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/ryle.jpg')
        },
        {
          id: 6,
          name: 'Kissy Cyrine A. Garciano',
          positionTitle: 'Secretary',
          courseAndYear: 'BSIT-2',
          profileUrl: require('@/assets/candidates/kissy.jpg')
        },
        {
          id: 7,
          name: 'Cathylyn Shaine P. Olandre',
          positionTitle: 'InfoMedia',
          courseAndYear: 'BSCS-1',
          profileUrl: require('@/assets/candidates/cathy.jpg')
        },
        {
          id: 8,
          name: 'Lucy Mae Tan',
          positionTitle: 'InfoMedia',
          courseAndYear: 'BSIT-2',
          profileUrl: require('@/assets/candidates/lucy.jpg')
        },
        
        {
          id: 9,
          name: 'Abby Kate V. Dela Pena',
          positionTitle: 'Budget and Finance',
          courseAndYear: 'BSCS-1',
          profileUrl: require('@/assets/candidates/abby.jpg')
        },
        {
          id: 10,
          name: 'Ruffa Mae L. Arañez',
          positionTitle: 'Budget and Finance',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/ruffa.jpg')
        },
        {
          id: 11,
          name: 'John Piolo H. Mutia',
          positionTitle: 'Material Preparation and Services',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/piolo.jpg')
        },
        {
          id: 12,
          name: 'Keith M. Ostia',
          positionTitle: 'Material Preparation and Services',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/keith.jpg')
        },
        {
          id: 13,
          name: 'Mark Chezter M. Barcelo',
          positionTitle: 'Logistics',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/mark.jpg')
        },
        {
          id: 14,
          name: 'Aliza Nicole M. Gumapac',
          positionTitle: 'Logistics',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/aliza.jpg')
        },
        {
          id: 15,
          name: 'Chris Heart E. Blanco',
          positionTitle: 'Public Relations and Communications',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/heart.jpg')
        },
        {
          id: 16,
          name: 'Wena Mae V. Mabasa',
          positionTitle: 'Public Relations and Communications',
          courseAndYear: 'BSIT-1',
          profileUrl: require('@/assets/candidates/wena.jpg')
        },
        {
          id: 17,
          name: 'Ruel Dean Buray',
          positionTitle: 'Public Relations and Communications',
          courseAndYear: 'BSCS-2',
          profileUrl: require('@/assets/candidates/ruel.jpg')
        },
      ]
    }
  }
}
</script>

<style>

</style>
