<template>
  <div class="memo-form">
    <form>
      <fieldset>
        <div>
          <input class="memo-title" type="text" placeholder="제목" />
          <textarea class="memo-content" placeholder="내용" />
          <button type="reset">
            <i class="fas fa-sync-alt" />
          </button>
        </div>
        <button type="submit">등록</button>
      </fieldset>
    </form>
  </div>
</template>

<script>
export default {
  name: "memo-form"
};
</script>

<style scoped>
.memo-form {
  margin-bottom: 24px;
  padding-bottom: 40px;
  border-bottom: 1px solid #eee;
}
.memo-form form fieldset div {
  position: relative;
  padding: 24px;
  margin-bottom: 20px;
  box-shadow: 0 4px 10px -4px rgba(0, 0, 0, 0.2);
}

.memo-form form fieldset div button[type="reset"] {
  position: absolute;
  right: 20px;
  bottom: 20px;
  font-size: 16px;
  background: none;
}

.memo-form form fieldset div button[type="submit"] {
  float: right;
  width: 96px;
  padding: 12px 0;
  border-radius: 4px;
  background-color: #ff5a00;
  color: #fff;
  font-size: 16px;
}
.memo-form fieldset .memo-title {
  width: 100%;
  margin-bottom: 12px;
  font-size: 18px;
  line-height: 26px;
}
.memo-form fieldset .memo-content {
  width: 100%;
  height: 66px;
  font-size: 14px;
  line-height: 22px;
  vertical-align: top;
}
.memo-form input:focus {
  outline: none;
}
</style>