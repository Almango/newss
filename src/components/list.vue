

<template>
  <div class="main_constainer" v-for="(value, index) in List_infomaction">

    <div class="list_icon"><img :src="value.icon"></div>
    <div class="list_description">
      <div class="description_title">
        <p>{{value.title}}</p>
      </div>
      <div class="description_about">
        <p>{{value.about}}</p>
      </div>
      <div class="description_version">
        <p>{{value.version}}</p>
      </div>
    </div>
    <div class="list_ip">
      <p>{{value.ip}}</p>
    </div>
    <div class="list_type">
      <p>{{value.type}}</p>
    </div>
    <div class="list_person">
      <p>{{value.person}}</p>
    </div>
    <div class="list_more">
      <button>更多详情</button>
    </div>
  </div>
</template>
<script setup>
import {reactive} from "vue";

const List_infomaction = reactive(
    [
      {
        title: "佳莉敦の世界",
        icon: 'https://t.tutu.to/th/NqJU7',
        about: "以原版纯生存为核心的长期性公益服务器，人数限制为14人，服务器限制性较少，反对作弊，在这里你可以着手与好友组建自己的小镇，探案更多未开发的大陆。***目前服务器趋于原版，没有过多插件，基本实现了原版生存休闲性***",
        version: "1.21.4",
        ip: "12m.rainplay.cn:35226",
        type: "生存",
        person: "2/14",
        time:"2025-2-15",
      },
      {
        title: "慵懒の世界",
        icon: 'https://t.tutu.to/th/NqOpw',
        about: "原版 | 纯净生存 | 长期",
        version: "1.21.4",
        ip: "12m.rainplay.cn:35226",
        type: "生存",
        person: "2/14",
        time:"2025-2-15",
      },
      {
        title: "Bamboss",
        icon: 'https://tietu.mclists.cn/server/icon/3144.png',
        about: "服务器是1.16.5的群组服务器,每个子服都有不同的玩法,OMO然后.....然后...我0m0..我不会写简介耶。",
        version: "1.21.4",
        ip: "bamboss.mossmc.top:25565",
        type: "生存",
        person: "2/14",
        time:"2025-2-15",
      },
      {
        title: "幻梦世界 | 海量原创 | 1.21.1",
        icon: 'https://tietu.mclists.cn/server/icon/2498.png',
        about: "以原版生存为核心，融合副本RPG元素，精炼，熔炼，锻造，副本，日常，挑战，轻松愉快",
        version: "1.21.4",
        ip: "hmsj.online:25565",
        type: "生存",
        person: "12 / 2025",
        time:"2025-2-15",
      },
      {
        title: "慵懒の世界",
        icon: 'https://t.tutu.to/th/NqOpw',
        about: "原版 | 纯净生存 | 长期",
        version: "1.21.4",
        ip: "12m.rainplay.cn:35226",
        type: "生存",
        person: "2/14",
        time:"2025-2-15",
      },
    ]
)
</script>
<style scoped>
.body{
  background-image: url("https://t.tutu.to/th/NqOpw.png");
}
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.main_constainer{
  width: 1200px;
  height: 100px;
  margin:  0 auto;
  box-shadow: rgba(0, 0, 0, 0.05) 0px 0px 0px 1px;
  display: flex;
}
.list_icon{
  width: 100px;
  height: 100px;
  //background: #c08ecf;
  padding: 10px;
}
.list_icon img {
  width: 80px;
  height: 80px;
  border-radius: 15px;
}
.list_description{
  width: 490px;
  height: 80px;
  //background-color: aqua;
  margin-top: 10px;
}
.description_title{
  width: 100%;
  height: 25px;
  //background-color: brown;
}
.description_title p{
  font-size: 17px;
  margin: 0;

}
.description_about{
  width: 100%;
  height: 25px;
  //background-color: rgb(111, 163, 43);
  overflow: hidden;
}
.description_about p{
  margin: 0;
  font-size: 15px;
  color: #979797;
}
.description_version{
  width: 100%;
  height: 30px;
  //background-color: #19a6a6;
}
.description_version p{
  margin: 0;
  font-size: 12px;
  display: inline-block;
  padding: 0 6px 0 6px;
  background: #e188d3;
  border-radius: 10px;
  border: 1px solid #7e7eff;
  color: #fff;
}
.list_ip{
  width: 500px;
  height: 100px;
  //background-color: blue;
}
.list_ip p{
  text-align: center;
  margin-top: 40px;
  color: #7e7eff;
}

.list_type{
  width: 250px;
  height: 100px;
  //background: #39783a;
}
.list_type p{
  text-align: center;
  margin-top: 40px;
  color: #717171;
}
.list_person{
  width: 250px;
  height: 100px;
  //background: #976c6c;
}
.list_person p{
  text-align: center;
  margin-top: 40px;
  color: #000000;
}
.list_more{
  width: 300px;
  height: 100px;
  //background: #852020;
}
.list_more button{
  width: 100px;
  height: 50px;
  margin-top: 25px;
  margin-left: 40px;
  outline: none;
  background-color: #c08ecf;
  color: white;
  border: 0;
  cursor: pointer;
}

</style>