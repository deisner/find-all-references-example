<template>
  <div>
    {{ foo }}
    {{ dublin }}
  </div>
</template>

<script>
import * as _ from 'lodash'
import { doubleIt } from './utils';
export default {
  props: ['foo', 'bar'],
  computed: {
    dublin() {
      return doubleIt(7);
    }
  }
}
</script>