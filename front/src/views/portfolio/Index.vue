
<script>
  // Extensions
  import View from '@/views/View'

  // Mixins
  import LoadSections from '@/mixins/load-sections'

  export default {
    name: 'Portfolio',

    metaInfo: { title: 'Portfolio' },

    extends: View,

    mixins: [
      LoadSections([
        'portfolio',
      ]),
    ],

    props: {
      id: {
        type: String,
        default: 'portfolio',
      },
    },
  }
</script>
