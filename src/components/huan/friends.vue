<template>
  <div>
    <div class="draw__arrow">
      <div class="arrow__up"></div>
    </div>
    <div class="avatar__img">
      <div class="container">
        <div class="avatar">
          <div class="img">
            <img
              src="../../assets/huan/cham.jpg"
              alt=""
              title="Nguyễn Ngọc Châm"
            />
            <img src="../../assets/huan/huan.jpg" alt="" title="Huấn Đặng" />
          </div>
        </div>
        <div>
          <p>
            Cùng vào ngày chụp kỷ yếu. Có 2 người đã nhìn về hướng của nhau như
            báo trước có ngày quen nhau vậy c nhỉ =))
          </p>
          <p>
            Gặp nhau là cái "duyên". Duyên này quá sức tưởng tượng của tớ và cậu
            và thậm trí của mọi người =))
          </p>
          <p>
            Mọi người nghĩ sao tớ mặc kệ. Tớ chỉ quan tâm cậu nghĩ gì thôi =))
          </p>
          <p>
            Vậy nên tớ sẽ giữ trọn "duyên" trời ban này
            <i class="fas fa-heart"></i>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "friends",
  props: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import url("https://use.fontawesome.com/releases/v5.13.0/css/all.css");

.avatar__img {
  font-family: "Baloo Thambi 2", cursive;
  background: rgb(237, 241, 250);
  display: flex;
  justify-content: center;
  align-items: center;
  height: 97vh;
  font-size: 16px;
  background-color: #ebeef2;
}

.container {
  background-color: white;
  box-shadow: 0px 1px 20px 0px #beb0a3;
  border-radius: 0.5rem;
  .avatar {
    width: 100%;
    .img {
      display: flex;
      width: 60rem;
      img {
        width: 30rem;
        height: 30rem;
      }
    }
  }
  p {
    margin: 1rem;
  }
  i {
    color: red;
  }
}

.draw__arrow {
  display: flex;
  justify-content: center;
  align-items: center;
}
.arrow__up {
  width: 0;
  height: 0;
  border-left: 20px solid transparent;
  border-right: 20px solid transparent;

  border-bottom: 20px solid #e9eaf3;
}
</style>
