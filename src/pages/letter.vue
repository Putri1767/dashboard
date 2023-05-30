<template>
    <h3 class="text-2xl font-bold text-left py-2">Letter Type Information</h3>
      <div class="section">
        <div class="container">
          <div class="columns">
            <div class="column is-5 is-offset-3">
              <form @submit.prevent="handleSubmit" class="py-3 px-10 text-left">
                <tr>
                  <label > Letter Name</label>
                  <textarea class="bg-gray-200"
                                        placeholder ="    Surat Keterangan"
                                        rows="2"
                                        cols="170"
                                        v-model="form.name"
                                    /><br>
                 <label> Format</label>
                  <textarea class="bg-gray-200 "
                                        placeholder="    xxx/S.Pk/BKJ/mm/YYYY"
                                        rows="2"
                                        cols="170"
                                        v-model="form.format"
                                    /><br>
                 <label> Restart Num Typle</label>
                  <textarea class= 'bg-gray-200'
                                      placeholder="    Monthly"
                                        rows="2"
                                        cols="170"
                                        v-model="form.restart"
                                    />
                          <br>
                <div class="field is-grouped">
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