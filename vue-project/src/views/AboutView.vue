<template>
  <div class="about">
    <div class="container">
      <br />
      <h1>會員資料查詢</h1>
      <p>請輸入會員資料</p>
      <br />
      <form>
        <div class="form-group">
          <label for="name" class="mx-5">會員姓名</label>
          <input
            type="text"
            class="form-control "
            id="name"
            aria-describedby="emailHelp"
            placeholder="請輸入會員姓名"
          />
        </div>
        <br />
        <div class="form-group">
          <label for="memberNumber">會員編號</label>
          <input
            type="text"
            class="form-control"
            id="memberNumber"
            placeholder="請輸入會員編號"
          />
        </div>
        <br />
        <button type="submit" class="btn btn-primary">查詢</button>
      </form>
    </div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .about {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
