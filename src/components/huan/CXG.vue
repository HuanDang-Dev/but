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
              src="../../assets/huan/CXG.jpg"
              alt=""
              title="Gia đình nhỏ của Châm"
            />
            <img
              src="../../assets/huan/CXG_giay.jpg"
              alt=""
              title="Gia đình nhỏ của Châm"
            />
          </div>
        </div>
        <div>
          <p>
            Cậu hãy luôn vui vẻ nhé!!! CXG =)) <i class="fas fa-heart"></i
            ><i class="fas fa-heart"></i><i class="fas fa-heart"></i>
          </p>
          <p>
            Chúc cậu và "gia đình" mãi yêu thương, vui vẻ và hạnh phúc bên nhau
            như ý nghĩa của bức ảnh "Treo giày lên cây" ạ
            <i class="far fa-grin-hearts"></i><i class="far fa-grin-hearts"></i
            ><i class="far fa-grin-hearts"></i>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "CXG",
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
  font-size: 16px;
  background-color: #ebeef2;
}

.container {
  box-shadow: 0px 1px 20px 0px #beb0a3;
  border-radius: 0.5rem;
  margin: 5rem;
  .avatar {
    width: 100%;
    .img {
      display: flex;
      flex-direction: column;

      img {
        width: 60rem;
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
