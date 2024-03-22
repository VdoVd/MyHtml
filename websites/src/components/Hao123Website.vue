<template>
    <div class="container">
        <div class="row1">
            <img class="hao" src="../static/hao123/10001.png"/>
            <div class="right">
                <div>
                    <p>深圳</p>
                    <p>未来七天</p>
                </div>
                <img class="clound" src="../static/hao123/10012.png"/>
                <p class="du">20°</p>
            </div>
          
        </div>
        <div class="row2">
            <p>搜你想搜的</p>
            <div class="right">
                <img src="../static/hao123/10016.png"/>
                <div>
                    百度一下
                </div>
            </div>
        </div>
        <div class="row3">
            <div>
                杜海涛爆改
            </div>
            <div>
                韩版凯特门
            </div>
            <div>
                鲜芋仙致歉声明
            </div>
        </div>
        
        
    </div>
    <div id="content">
        <div class="container2" v-for="list in lists" :key="list.id">
            <img :src="list.path" />
            <p>{{ list.content }}</p>
        </div>

        <div class="container3" v-for="(list ,index) in lists2" :key="index">
          <p>{{ list }}</p>
        </div>
     </div>
  </template>
  
  <script setup>
   let lists=[{path:require('../static/hao123/10019.png'),content:'百度'}
        ,{path:require('../static/hao123/10020.png'),content:'凤凰'}
        ,{path:require('../static/hao123/10021.png'),content:'腾讯'}
        ,{path:require('../static/hao123/10022.png'),content:'搜狐'}
        ,{path:require('../static/hao123/10023.png'),content:'新浪'}
        ,{path:require('../static/hao123/10024.png'),content:'网易'}
        ,{path:require('../static/hao123/10025.png'),content:'东方财富'}
        ,{path:require('../static/hao123/10026.png'),content:'58同城'}
        ,{path:require('../static/hao123/10027.png'),content:'百度地图'}
        ,{path:require('../static/hao123/10028.jpg'),content:'百度翻译'}
        ,{path:require('../static/hao123/10029.png'),content:'爱奇艺'}
        ,{path:require('../static/hao123/10030.png'),content:'好看视频'}
        ,{path:require('../static/hao123/10031.png'),content:'京东'}
        ,{path:require('../static/hao123/10032.png'),content:'哔哩哔哩'}
        ,{path:require('../static/hao123/10033.png'),content:'淘宝网'}
        ,{path:require('../static/hao123/10034.png'),content:'爱淘宝'}
        ,{path:require('../static/hao123/10035.png'),content:'百度手助'}
        ,{path:require('../static/hao123/10036.png'),content:'研招网'}
        ,{path:require('../static/hao123/10037.png'),content:'天猫国际'}
        ,{path:require('../static/hao123/10038.png'),content:'优酷'}
        ,{path:require('../static/hao123/10039.png'),content:'虎扑'}
        ,{path:require('../static/hao123/10040.png'),content:'知乎'}
        ,{path:require('../static/hao123/10041.png'),content:'百度文库'}
        ,{path:require('../static/hao123/10042.png'),content:'12306'}
        ]

        let lists2=['国际超市','惠生活','限时优惠','QQ音乐','违章查询','前程无忧','百度文库','精选商品','双色球','网址大全']
  </script>
  
  <!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container{
    margin: 0 auto;
    position: relative;
    top: 0;
    background-color: rgb(126,204,242);
    padding: 15px;
    display: flex;
    justify-content: space-around;
    flex-direction: column;
    .row1{
        width: 100%;
        display: flex;
        justify-content: space-between;
        .hao{
            width: 100px;
            height: 27px;
            align-self:self-end;
            margin-right: 70px;
    
        }
        .right{
            flex: 1;
            display: flex;
            flex-direction: row;
            justify-content: space-around;
        
        div{
            display: flex;
            margin: 0;
            padding: 0;
            justify-content: center;
            flex-direction: column;
            p{
                color: white;
                padding: 0;
                text-align: center;
                font-size:12px ;
                margin: 0px;
            }
            align-self: self-end;
    
        }
        .clound{
            width: 35px;
            height: 35px;
            align-self: self-end;
        }
        .du{
            color: white;
            font-size: 30px;
            display: block;
            text-align: end; 
            margin: 0;
            width: 30px;
            height: 30px;
            padding: 0;
        }
    }
       
    }
    .row2{
        height: 43px;
        margin-top: 10px;
        display: flex;
        flex-direction: row;
        background-color: white;
        p{
            flex: 1;
            font-size: 16px;
            color: gray;
            margin: 10px;
        }
        .right{
            flex-direction: row;
            display: flex;
            align-items: center;
            img{
                height: 16px;
                width: 22px;
                margin-right: 15px;
            }
            div{
                background-color: #F2F2F2;
                height: 43px;
                text-align: center;
                align-self: center;
                padding: 0 8px;
                display: flex;
                align-items: center;
            }
        }
    }
    .row3{
        display: flex;
        justify-content: start;
        color: white;
        font-size: 13px;
        div{
            margin-top: 10px;
            margin-right: 10px;
        }
    }
    
}
#content{
    
    display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    margin-top: 20px;
    .container2{
        width: 16%;
        height: 60px;
        margin-bottom: 5px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        img{
          width: 25px;
          height: 25px;
        }
        p{
          width: 100%;
          text-align: center;
          font-size: 13px;
        }
    }

    .container3 {
      p{
        width: 20vw;
        font-size: 15px;
        text-align: center;
      }
      

    }
}


  </style>
  