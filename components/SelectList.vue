<template>
  <div class="mt-5 mb-5">
    <div>
      <multiselect
        :close-on-select="false"
        :searchable="true"
        placeholder="Use Optima to work"
        :options="options"
        :show-labels="false"
      >
        <template slot="option" slot-scope="props">
          <a href="/userguide/optima" target="_blank"
            ><p>{{ props.option }}</p></a
          >
        </template>
      </multiselect>
      <div>
        <multiselect
          :searchable="true"
          placeholder="Get started with Optima"
          :options="getStartedOptions"
          :show-labels="false"
          :close-on-select="false"
        >
          <template slot="option" slot-scope="props">
            <a href="/userguide/optima" target="_blank"
              ><p>{{ props.option }}</p></a
            >
          </template>
        </multiselect>
      </div>
      <div>
        <multiselect
          :close-on-select="false"
          :searchable="true"
          placeholder="Create and personalize a profile"
          :options="getStartedOptions"
          :show-labels="false"
        >
          <template slot="option" slot-scope="props">
            <a href="/userguide/optima" target="_blank"
              ><p>{{ props.option }}</p></a
            >
          </template>
        </multiselect>
      </div>

      <div>
        <multiselect
          :close-on-select="false"
          :searchable="true"
          placeholder="Control your safety and privacy"
          :options="getStartedOptions"
          :show-labels="false"
        >
          <template slot="option" slot-scope="props">
            <a href="/userguide/optima" target="_blank"
              ><p>{{ props.option }}</p></a
            >
          </template>
        </multiselect>
      </div>

      <div>
        <multiselect
          :close-on-select="false"
          :searchable="true"
          placeholder="Change Optima settings"
          :options="getStartedOptions"
          :show-labels="false"
        >
          <template slot="option" slot-scope="props">
            <a href="/userguide/optima" target="_blank"
              ><p>{{ props.option }}</p></a
            >
          </template>
        </multiselect>
      </div>

      <div>
        <multiselect
          :close-on-select="false"
          :searchable="true"
          placeholder="Privacy in Optima"
          :options="getStartedOptions"
          :show-labels="false"
        >
          <template slot="option" slot-scope="props">
            <a href="/userguide/optima" target="_blank"
              ><p>{{ props.option }}</p></a
            >
          </template>
        </multiselect>
      </div>

      <div>
        <multiselect
          :close-on-select="false"
          :searchable="true"
          placeholder="Create and personalize a profile"
          :options="getStartedOptions"
          :show-labels="false"
        >
          <template slot="option" slot-scope="props">
            <a href="/userguide/optima" target="_blank"
              ><p>{{ props.option }}</p></a
            >
          </template>
        </multiselect>
      </div>
    </div>
    <!-- <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Use Optima to work"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div>

    <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Get started with Optima"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div>

    <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Create and personalize a profile"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div>

    <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Control your safety and privacy"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div>

    <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Change Optima settings"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div>

    <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Privacy in Optima"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div>

    <div>
      <multiselect
        v-model="value"
        :options="options"
        :searchable="true"
        :close-on-select="true"
        :show-labels="true"
        placeholder="Create and personalize a profile"
      >
        <pre class="language-json"><code>{{ value  }}</code></pre>
      </multiselect>
    </div> -->
  </div>
</template>

<script>
import Multiselect from 'vue-multiselect'

export default {
  components: {
    Multiselect,
  },
  data() {
    return {
      isOpen: false,
      value: '',
      //   options: ['Select option', 'label', 'touched'],
      //   options: [
      //     { name: 'Orange', value: 'orange' },
      //     { name: 'Apple', value: 'apple' },
      //     { name: 'Grape', value: 'grape' },
      //   ],
      options: ['Learn How to use Optima'],

      getStartedOptions: [
        'Get started with Optima',
        'How do i log in on the app?',
        'Tips and Tricks of Optima',
      ],
    }
  },
  head() {
    return {
      link: [
        {
          rel: 'stylesheet',
          href:
            'https://db.onlinewebfonts.com/c/0007c768c0c6149485a44a0409d9433c?family=GalanoGrotesque-Regular',
        },
      ],
    }
  },
}
</script>

<style src="vue-multiselect/dist/vue-multiselect.min.css"></style>

<style scoped>
* {
  font-family: 'GalanoGrotesque-Regular', 'Quicksand', 'Source Sans Pro',
    -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue',
    Arial, sans-serif;
}
</style>
