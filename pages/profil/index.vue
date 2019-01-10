<template>
  <div class="container">
    <div class="columns is-mobile is-multiline is-centered">
      <div class="column is-narrow">
        <h5>Compétences</h5>
        <div style="position: relative;">
          <v-chart-radar 
            :chartdata="skillChart.data" 
            :options="skillChart.options"
            class="isChart"
          />
        </div>
      </div>
      <div class="column is-narrow">
        <h5>Technologies</h5>
        <v-chart-radar 
          :chartdata="techChart.data" 
          :options="techChart.options"
          class="isChart"
        />
      </div>
      <div class="column is-narrow">
        <h5>Personnalité</h5>
        <v-chart-radar 
          :chartdata="personalityChart.data" 
          :options="personalityChart.options"
          class="isChart"
        />
      </div>
    </div>
  </div>
</template>

<script>
import vChartRadar from '@/components/v-chart-radar'
export default {
  layout: 'default',
  components: {
    vChartRadar
  },
  data () {
    return {
      skillChart: {
        data: {
          labels: ['Conception', 'Back', 'Front', 'Devops', 'UX / UI', 'Agile'],
          datasets: [
            {
              label: '2017',
              data: [4, 6, 2, 3, 2, 4]
            },
            {
              label: '2019',
              data: [8, 7, 7, 5, 6, 5],
              borderColor: '#4fc08d'
            }
          ],
          min: 0
        },
        options: {
          responsive: true,
          maintainAspectRatio: false,
          scale: {
            ticks: {
              display: false,
              beginAtZero: true,
              max: 10
            }
          }
        }
      },
      techChart: {
        data: {
          labels: ['Vue', 'React', 'Angular', 'Symfony', 'Express', 'Adonis'],
          datasets: [
            {
              label: '2019',
              data: [9, 6, 5, 5, 8, 6],
              borderColor: '#4fc08d'
            },
          ]
        },
        options: {
          legend: {
            display: false
          },
          responsive: true,
          maintainAspectRatio: false,
          scale: {
            ticks: {
              display: false,
              beginAtZero: true,
              max: 10
            }
          }
        }
      },
      personalityChart: {
        data: {
          labels: ['Calme', 'Créatif', 'Perseverant', 'Autonome', 'Positif'],
          datasets: [
            {
              label: 'Alexis',
              data: [9, 10, 8, 10, 8],
              borderColor: '#4fc08d'
            },
          ],
        },
        options: {
          legend: {
            display: false
          },
          responsive: true,
          maintainAspectRatio: false,
          scale: {
            ticks: {
              display: false,
              beginAtZero: true,
              max: 10
            }
          }
        }
      }
    }
  }
}
</script>

<style scoped>
.isChart {
  position: relative;
  margin: auto;
  max-height: 312px;
  max-width: 312px;
}
</style>
