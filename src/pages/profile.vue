<template>
<h3 class="text-2xl font-bold text-left py-2">Form lowongan</h3>
  <div class="section">
    <div class="container">
      <div class="columns">
        <div class="column is-5 is-offset-3">
          <form @submit.prevent="handleSubmit" class="py-3 px-10 text-center">
            <tr>
              <textarea class="bg-gray-200"
                                    placeholder="    Title"
                                    rows="1"
                                    cols="170"
                                    v-model="form.title"
                                /><br>
              <textarea class="bg-gray-200"
                                    placeholder="    Summary"
                                    rows="1"
                                    cols="170"
                                    v-model="form.summary"
                                /><br>
              <textarea class= 'bg-gray-200'
                                  placeholder="    Deskripsi"
                                    rows="4"
                                    cols="170"
                                    v-model="form.deskripsi"
                                />
                      <br>
              <textarea class="bg-gray-200"
                                    placeholder="    Linkedin"
                                    rows="1"
                                    cols="170"
                                    v-model="form.Linkedin"
                                /><br>
              <textarea class="bg-gray-200"
                                    placeholder="    Glints link"
                                    rows="1"
                                    cols="170"
                                    v-model="form.Glints"
                                /><br><br>
            <div class="field is-grouped">
              <div class="control">
                <button type="submit" class="button is-link bg-gray-400 px-4">Submit</button>
              </div>
            </div>
          </tr>
          </form>
        </div>
        </div>
      </div>
    </div>

</template>

<script>
 export default {
  data() {
        return {
            text: "",
            form: {
                lowongan: null,
                deskripsi: null,
            },
        };
    },
  }
</script>