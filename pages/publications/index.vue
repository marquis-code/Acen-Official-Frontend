<template>
  <main>
    <section class="text-gray-600 body-font">
      <div class="container px-5 py-24 mx-auto">
        <div class="flex flex-wrap w-full mb-20 flex-col items-center text-center">
          <h1 class="sm:text-3xl text-2xl font-medium title-font mb-2 text-gray-900">
            Publications
          </h1>
          <p class="lg:w-1/2 w-full leading-relaxed text-gray-500">
            We publish cutting-edge research and best practice in the field of endocrinology through seven official journals and conference abstracts. Our quarterly magazine The Endocrinologist contains opinion pieces, research and practice updates and Society news for members.
          </p>
        </div>
        <section class="text-gray-600 body-font overflow-hidden">
          <div class="container px-5 py-24 mx-auto">
            <div class="-my-8 divide-y-2 divide-gray-100">
              <div
                v-for="(item, index) in [
                  {
                    title: 'Clinical Endocrinology',
                    description: 'is the Society\'s official journal and publishes articles on the clinical aspects of endocrinology, including the clinical application of molecular endocrinology. It features reviews, original papers, commentaries, cases of the month, clinical questions, book reviews and letters. Clinical Endocrinology is essential reading not only for those engaged in research but also for those involved primarily in clinical practice.',
                    publisher: 'Wiley.',
                    editors: {
                      'Co-Editors-in-Chief': 'Prof Maralyn Druce and Prof Aled Rees',
                      'Member Benefits': ['Free access for members'],
                      '2022 Journal Impact Factor': '3.2'
                    },
                    links: [
                      {
                        title: 'View Clinical Endocrinology online',
                        url: ''
                      }, {
                        title: 'Sign-up for content alerts',
                        url: ''
                      },
                      {
                        title: 'Want to submit?',
                        url: ''
                      }
                    ]
                  },
                  {
                    title: 'Journal of Endocrinology',
                    description: ' is a leading global journal that publishes original research articles, reviews and science guidelines. Its focus is on endocrine physiology and metabolism, including hormone secretion; hormone action; biological effects. The journal publishes basic and translational studies at the organ, tissue and whole organism level. Alongside the core endocrinology topics, the journal also encourages submissions on cardiovascular, muscle and renal endocrinology as well as submissions on the immune system where this impacts the endocrine system',
                    editors: {
                      'Co-Editors-in-Chief': 'Prof Maralyn Druce and Prof Aled Rees',
                      'Member Benefits': ['No colour charges for members', 'No submission fees or page charges', 'Free access for members'],
                      '2022 Journal Impact Factor': '3.5',
                      '5-year Journal Impact Factor': '5.1'
                    },
                    links: [
                      {
                        title: 'View the Journal online',
                        url: ''
                      }, {
                        title: 'Want to submit?',
                        url: ''
                      },
                      {
                        title: 'Subscriptions and prices',
                        url: ''
                      },
                      {
                        title: 'Scope',
                        url: ''
                      },
                      {
                        title: 'Editorial board',
                        url: ''
                      },
                      {
                        title: 'Sign-up for the latest content direct to your inbox',
                        url: ''
                      }
                    ]
                  },
                  {
                    title: 'Journal of Molecular Endocrinology',
                    description: 'Journal of Molecular Endocrinology is a leading global journal that publishes original research articles and reviews. The journal focuses on molecular and cellular mechanisms in endocrinology, including: gene regulation, cell biology, signalling, mutations, transgenics, hormone-dependant cancers, nuclear receptors. Basic and pathophysiological studies at the molecule and cell level are considered, as well as human sample studies where this is the experimental model of choice. Technique studies including Omics, CRISPR or gene editing are also encouraged, provided they are set within a larger endocrinology context. Alongside the core endocrinology topics, the journal also encourages comprehensive mechanistic studies on cardiovascular, muscle and renal endocrinology as well as submissions on the immune system impact on the endocrine system.',
                    publisher: 'Bioscientifica.',
                    editors: {
                      'Co-Editors-in-Chief': 'Prof Maralyn Druce and Prof Aled Rees',
                      'Member Benefits': ['No colour charges for members', 'No submission fees or page charges', 'Free access for members'],
                      '2022 Journal Impact Factor': '3.5',
                      '5-year Journal Impact Factor': '5.1'
                    },
                    links: [
                      {
                        title: 'View the Journal online',
                        url: ''
                      }, {
                        title: 'Want to submit?',
                        url: ''
                      },
                      {
                        title: 'Subscriptions and prices',
                        url: ''
                      },
                      {
                        title: 'Scope',
                        url: ''
                      },
                      {
                        title: 'Editorial board',
                        url: ''
                      },
                      {
                        title: 'Sign-up for the latest content direct to your inbox',
                        url: ''
                      }
                    ]
                  },
                  {
                    title: 'Endocrine-Related Cancer',
                    description: ' provides a unique international forum for the publication of high quality original articles describing novel, cutting edge basic laboratory, translational and clinical investigations of human health and disease focusing on endocrine neoplasias and hormone-dependent cancers; and for the publication of authoritative review articles in these topics.\n Endocrine neoplasias include adrenal cortex, breast, multiple endocrine neoplasia, neuroendocrine tumours, ovary, prostate, paraganglioma, parathyroid, pheochromocytoma pituitary, testes, thyroid and hormone-dependent cancers. Neoplasias affecting metabolism and energy production such as bladder, bone, kidney, lung, and head and neck, are also considered.',
                    publisher: 'Bioscientifica.',
                    editors: {
                      'Editor-in-Chief': 'Professor Matthew Ringel',
                      'Member Benefits': ['No colour charges for members', 'No submission fees or page charges', 'Free access for members'],
                      '2022 Journal Impact Factor': '3.9',
                      '5-year Journal Impact Factor': '5.1'
                    },
                    links: [
                      {
                        title: 'View the Journal online',
                        url: ''
                      }, {
                        title: 'Want to submit?',
                        url: ''
                      },
                      {
                        title: 'Subscriptions and prices',
                        url: ''
                      },
                      {
                        title: 'Scope',
                        url: ''
                      },
                      {
                        title: 'Editorial board',
                        url: ''
                      },
                      {
                        title: 'Sign-up for the latest content direct to your inbox',
                        url: ''
                      }
                    ]
                  },
                  {
                    title: 'Endocrine Connections',
                    description: 'is a society-owned open access journal offering authors the highest possible visibility for their work and stimulating cross-discipline collaboration. The journal publishes basic, translational and clinical research and reviews in all areas of endocrinology, including papers that deal with non-classical tissues as source or targets of hormones and endocrine papers that have relevance to endocrine-related and intersecting disciplines and the wider biomedical community. Topics include Metabolic Syndrome and Diabetes, Cardiovascular, Thyroid, Adrenal, Bone and Mineral Metabolism, Hormones and Cancer, Pituitary and Hypothalamus, and Reproduction. The journal considers basic, translational and clinical studies.',
                    publisher: 'Bioscientifica.',
                    editors: {
                      'Editor-in-Chief': 'Professor Adrian Clark',
                      'Member Benefits': ['Society members get 40% discount on the full Article Publishing Charge.'],
                      '2022 Journal Impact Factor': '2.9',
                      '5-year Journal Impact Factor': '3.3'
                    },
                    links: [
                      {
                        title: 'View the Journal online',
                        url: ''
                      },
                      {
                        title: 'Scope',
                        url: ''
                      },
                      {
                        title: 'Want to submit?',
                        url: ''
                      },
                      {
                        title: 'Editorial board',
                        url: ''
                      },
                      {
                        title: 'Subscriptions and prices',
                        url: ''
                      },
                      {
                        title: 'Sign-up for the latest content direct to your inbox',
                        url: ''
                      }
                    ]
                  },
                  {
                    title: 'Endocrine Oncology',
                    description: ' is an open-access, peer-reviewed journal publishing basic, translational and clinical research and reviews on the interplay between hormones and cancer, and related topics. Endocrine Oncology will consider for publication all articles which contribute to the advancement of the field and are scientifically sound. Topics include, but are not limited to, neuroendocrine tumours, and tumours of the adrenal, pituitary, breast, prostate, thyroid, gynecological, pancreas, parathyroid and bone, pheochromocytoma/paraganglioma, multiple endocrine neoplasia, and the interplay of diabetes, obesity, metabolism and cancer.',
                    publisher: 'Bioscientifica.',
                    editors: {
                      'Editor-in-Chief': 'Professor Justo P. Castano',
                      'Member Benefits': ['Open access article publication charge waived during launch years of the journal.', 'All profits from the journal are given back to the Society for Endocrinology.']
                    },
                    links: [
                      {
                        title: 'View the Journal online',
                        url: ''
                      },
                      {
                        title: 'Scope',
                        url: ''
                      },
                      {
                        title: 'Want to submit?',
                        url: ''
                      },
                      {
                        title: 'Editorial board',
                        url: ''
                      },
                      {
                        title: 'Free to publish during launch years',
                        url: ''
                      },
                      {
                        title: 'Sign-up for the latest content direct to your inbox',
                        url: ''
                      }
                    ]
                  },
                  {
                    title: 'Endocrinology, Diabetes & Metabolism Case Reports',
                    description: 'publishes case reports on common and rare conditions in all areas of clinical endocrinology, diabetes and metabolism. The types of cases of interest include: novel diagnostic procedures, novel treatment, unusual effects of medical treatment, new disease or syndrome, unique/unexpected presentation of a disease or errors in diagnosis/pitfalls and caveats.',
                    publisher: 'Bioscientifica.',
                    editors: {
                      'Co-Editor-in-Chief': 'Dr Jerry Greenfield and Dr Sarantis Livadas (Acting)',
                      'Member Benefits': ['Society members get a 25% discount on the full Article Publishing Charges', 'Indexed in PubMed and Emerging Sources Citation Index', 'All profits from the journal are given back to the Society for Endocrinology'],
                      '2022 Journal Impact Factor': '0.9',
                      '5-year Journal Impact Factor': '1'
                    },
                    links: [
                      {
                        title: 'View the Journal online',
                        url: ''
                      },
                      {
                        title: 'Scope',
                        url: ''
                      },
                      {
                        title: 'Want to submit?',
                        url: ''
                      },
                      {
                        title: 'Editorial board',
                        url: ''
                      },
                      {
                        title: 'Free to publish during launch years',
                        url: ''
                      },
                      {
                        title: 'Sign-up for the latest content direct to your inbox',
                        url: ''
                      }
                    ]
                  }
                ]"
                :key="index"
                class="py-8 flex flex-wrap md:flex-nowrap"
              >
                <div class="flex justify-between gap-x-6">
                  <div class="w-6/12 mx-auto">
                    <div class="md:flex-grow space-y-3">
                      <h2 class="text-2xl font-medium text-gray-900 title-font mb-2">
                        {{ item.title }}
                      </h2>
                      <p class="leading-relaxed text-justify">
                        {{ item.description }}
                      </p>
                      <p class="text-sm">
                        Published by: <span class="text-blue-600 font-medium">{{ item.publisher }}</span>
                      </p>
                      <a
                        class="group relative inline-block rounded-md overflow-hidden border border-indigo-600 px-8 py-2 focus:outline-none focus:ring"
                        href="/download"
                      >
                        <span
                          class="absolute inset-y-0 left-0 w-[2px] bg-indigo-600 transition-all group-hover:w-full group-active:bg-indigo-500"
                        />

                        <span
                          class="relative text-sm font-medium text-indigo-600 transition-colors group-hover:text-white"
                        >
                         View this publication
                        </span>
                      </a>
                    </div>
                  </div>
                  <div class="w-3/12 mx-auto space-y-6 border border-gray-300 rounded-md p-3">
                    <div v-for="(value, key, idx) in item.editors" :key="idx" class="">
                      <h1 class="font-medium text-gray-900 underline text-sm">
                        {{ key }}
                      </h1>
                      <div v-if="key === 'Member Benefits'" class="space-y-3">
                        <p v-for="(itm, i) in value" :key="i" class="text-xs">
                          {{ itm }}
                        </p>
                      </div>
                      <p v-else class="text-gray-600 text-xs">
                        {{ value }}
                      </p>
                    </div>
                  </div>
                  <div class="w-3/12 mx-auto space-y-4 border border-gray-300 rounded-md p-4">
                    <div v-for="(itm, idx) in item.links" :key="idx" class="">
                      <nuxt-link :to="itm.url" class="text-blue-700 text-sm">
                        {{ itm.title }}
                      </nuxt-link>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </section>
      </div>
    </section>
  </main>
</template>

<script>
export default {
  data () {
    return {
      pulications: [
        {
          title: 'Journal of Endocrinology',
          description: 'is the Society\'s official journal and publishes articles on the clinical aspects of endocrinology, including the clinical application of molecular endocrinology. It features reviews, original papers, commentaries, cases of the month, clinical questions, book reviews and letters. Clinical Endocrinology is essential reading not only for those engaged in research but also for those involved primarily in clinical practice.',
          publisher: 'Wiley.',
          editors: {
            'Co-Editors-in-Chief': 'Prof Maralyn Druce and Prof Aled Rees',
            'Member Benefits': ['Free access for members'],
            '2022 Journal Impact Factor': '3.2'
          },
          links: [
            {
              title: 'View Clinical Endocrinology online',
              url: ''
            }, {
              title: 'Sign-up for content alerts',
              url: ''
            },
            {
              title: 'Want to submit?',
              url: ''
            }
          ]
        },
        {
          title: 'Journal of Molecular Endocrinology',
          description: 'Journal of Molecular Endocrinology is a leading global journal that publishes original research articles and reviews. The journal focuses on molecular and cellular mechanisms in endocrinology, including: gene regulation, cell biology, signalling, mutations, transgenics, hormone-dependant cancers, nuclear receptors. Basic and pathophysiological studies at the molecule and cell level are considered, as well as human sample studies where this is the experimental model of choice. Technique studies including Omics, CRISPR or gene editing are also encouraged, provided they are set within a larger endocrinology context. Alongside the core endocrinology topics, the journal also encourages comprehensive mechanistic studies on cardiovascular, muscle and renal endocrinology as well as submissions on the immune system impact on the endocrine system.',
          publisher: 'Bioscientifica.',
          editors: {
            'Co-Editors-in-Chief': 'Prof Maralyn Druce and Prof Aled Rees',
            'Member Benefits': ['No colour charges for members', 'No submission fees or page charges', 'Free access for members'],
            '2022 Journal Impact Factor': '3.5',
            '5-year Journal Impact Factor': '5.1'
          },
          links: [
            {
              title: 'View the Journal online',
              url: ''
            }, {
              title: 'Want to submit?',
              url: ''
            },
            {
              title: 'Subscriptions and prices',
              url: ''
            },
            {
              title: 'Scope',
              url: ''
            },
            {
              title: 'Editorial board',
              url: ''
            },
            {
              title: 'Sign-up for the latest content direct to your inbox',
              url: ''
            }
          ]
        }
      ]
    }
  },
  computed: {},
  watch: {},
  methods: {}
}
</script>
