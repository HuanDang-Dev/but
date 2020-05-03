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
              src="../../assets/huan/avatar_cham.jpg"
              alt=""
              title="Nguyễn Ngọc Châm"
            />
            <img
              src="../../assets/huan/avatar_huan.png"
              alt=""
              title="Huấn Đặng"
            />
          </div>
        </div>
        <div>
          <p>
            Đây là Châm dưới góc nhìn của một người em, và Huấn dưới góc nhìn
            của Châm <i class="far fa-grin-hearts"></i
            ><i class="far fa-grin-hearts"></i
            ><i class="far fa-grin-hearts"></i>
          </p>
          <p>Tớ và cậu đều đẹp mà nhờ =)))</p>
          <p>Đẹp dưới mọi góc độ ấy =))))</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "avatar",
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
    margin: 1px;
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
