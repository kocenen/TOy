<template>
  <div class="memo-app">
    Test Memo App
    <MemoForm></MemoForm>
    <!-- <MemoApp></MemoApp> -->
  </div>
</template>

<script>
import MemoForm from "./MemoForm";
// import MemoApp from "./MemoApp";

export default {
  name: "MemoApp",
  data() {
    return {
      memoArr: []
    };
  },
  created() {
    this.memoArr = localStorage.memos ? Json.parse(localStorage.memos) : [];
  }
};
</script>