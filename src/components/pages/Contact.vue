<template>
  <v-container>
    <v-row>
      <v-col>
        <h1 class="mb-10">お問い合わせ</h1>
        <p>ご連絡はTwitterのDM、または以下のフォームからお願いいたします。</p>
        <div class="pa-10">
          <v-text-field
              label="お名前"
              :rules="rules"
              hide-details="auto"
              class="mb-10"
          ></v-text-field>
          <v-text-field
              label="メールアドレス"
              :rules="rulesForEmail"
              class="mb-10"
          ></v-text-field>
          <v-textarea
              label="メッセージ内容"
              :rules="rulesForMessage"
              auto-grow
              autofocus
              filled
              class="mb-10"
          ></v-textarea>

          <div class="text-center">
            <v-btn
                rounded
                color="primary"
                dark
            >
              送信する
            </v-btn>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: "Contact",
  data: () => ({
    rules: [
      value => !!value || '名前は必須です。',
      value => (value && value.length >= 3) || '三文字以上で入力してください。',
    ],
    rulesForEmail: [
      value => !!value || 'メールアドレスは必須です',
      value => !value || /^\w+([.-]?\w+)*@\w+([.-]?\w+)*(\.\w{2,3})+$/.test(value) || '無効なメールアドレスです。'
    ],
    rulesForMessage: [
      value => !!value || 'メッセージは必須です',
    ]
  }),
}
</script>

<style scoped>

</style>
