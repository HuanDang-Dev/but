<template>
  <div class="huan__dashboard">
    <div class="main">
      <h1>Kỷ niệm tình bạn</h1>
      <p>
        Khoảng thời gian tuy ngắn nhưng nó mang lại một tình bạn không đơn giản
        chút nào cậu nhỉ =)).
      </p>
      <p>
        Do tớ không lên Hà Nội được nên tớ hẹn cậu một ngày không xa =)) tớ và
        cậu sẽ thực hiện chuyến đi đó.
      </p>
      <p>
        Tớ mong muốn thời gian mình quen biết cậu sẽ dài mãi....dài mãi... không
        cần dừng lại đâu ạ =))
      </p>
      <p>
        Văn tớ không tốt nên tớ nói ít mong cậu hiểu nhiều ạ
        <i class="fas fa-heart"></i><i class="fas fa-heart"></i
        ><i class="fas fa-heart"></i>
      </p>
    </div>
    <div class="box__day">
      <ul>
        <li v-for="challenge in challenges" :key="challenge.id">
          <div class="main__action">
            <button class="login__btn" @click="active = challenge.id">
              {{ challenge.day }}
            </button>
          </div>
        </li>
      </ul>
    </div>
    <div class="challenge__view" v-if="active !== null">
      <friends v-if="challenges[0].visible" />
      <avatar v-if="challenges[1].visible" />
      <CXG v-if="challenges[2].visible" />
    </div>
  </div>
</template>
<script>
import friends from "../components/huan/friends";
import avatar from "../components/huan/avatar";
import CXG from "../components/huan/CXG";

export default {
  name: "HuanDashboard",
  components: {
    friends,
    avatar,
    CXG
  },
  data() {
    return {
      challenges: [
        {
          id: 0,
          day: "You and me",
          visible: false
        },
        {
          id: 1,
          day: "Avatar",
          visible: false
        },
        {
          id: 2,
          day: "CXG =))",
          visible: false
        }
      ],
      active: null
    };
  },
  watch: {
    active: function(id) {
      this.challenges.forEach(select => {
        select.visible = false;
        if (select.id == id) {
          select.visible = true;
        }
      });
    }
  }
};
</script>
<style scoped lang="scss">
@import url("https://fonts.googleapis.com/css2?family=Satisfy&display=swap");

.huan__dashboard {
  width: 100%;
  font-family: "Satisfy", cursive;
  font-size: 20px;
}
.main {
  text-align: center;
  i {
    color: red;
    margin: 1px;
  }
}
.box__day {
  display: flex;
  ul {
    display: flex;
    align-items: center;
    justify-content: center;
    width: 100%;
    padding: 0;
    li {
      list-style: none;
    }
  }
}
.main__action {
  display: flex;
  align-items: center;
  margin: 1rem;
  .login__btn {
    background: #ebeef2;
    padding: 1rem;
    width: 7rem;
    border: none;
    outline: none;
    color: #4f5156;
    display: flex;
    justify-content: center;
    align-items: center;
    cursor: pointer;
    box-shadow: 2px 3px 3px 1px #e3e5ee;
    border-radius: 0.5rem;
    font-weight: 600;
  }
}
.login__btn:hover {
  background-color: #ebebeb;
}
</style>
