<template>
  <div id="app">
    <router-view />
  </div>
</template>

<script>
export default {
  name: 'App',
  data(){
    return{
    }
  },
  mounted(){
    
  },
  methods:{
  }
}
</script>

<style>
  @import "assets/font/iconfont.css";
  html,body{
    height: 100%;
    font-size: 14px;
  }
  body{
    min-width: 1220px;
  }
  #app{
    height: 100%;
  }
*{
	margin: 0;
  box-sizing: border-box;
}
ul li,
dl dd,
dl dd dt{
  list-style: none;
}
a,
a:focus,
a:link,
a:active,
a:hover{
	color: inherit;
	text-decoration: none;
}

input:focus{
  outline: none;
}

#resetModal .el-dialog{
  width: 400px;
}
#resetModal .el-menu-item-group{
  overflow: hidden;
}
.el-menu-item-group__title{
  display: none;
}

.clearfix:after{
  content: '';
  height: 0;
  width: 0;
  display: block;
  visibility: hidden;
  clear: both;
}

button:focus,
button:active{
  outline: none ;
}


  .el-dialog__header{
    padding: 15px 20px 0 !important;;
  }
  .el-dialog__body{
    padding: 20px !important;;
  }
  /*表格组件样式覆盖*/
  .el-table td,
  .el-table th{
    padding: 0!important;
    height: 40px!important;
    text-align: center !important;;
  }

  .el-table th{
    color: #333333 !important;;
    background: #C0ECAA !important;;
  }

  .el-table__body tr:nth-child(2n){
    background: #EEEEEE !important;;
  }

  .el-table--border td, .el-table--border th, .el-table__body-wrapper .el-table--border.is-scrolling-left~.el-table__fixed{
    border: none !important;;
  }
  .el-table--striped .el-table__body tr.el-table__row--striped.current-row td,
  .el-table__body tr.current-row>td,
  .el-table__body tr.hover-row.current-row>td,
  .el-table__body tr.hover-row.el-table__row--striped.current-row>td,
  .el-table__body tr.hover-row.el-table__row--striped>td,
  .el-table__body tr.hover-row>td{
    background: none !important;;
  }
  .el-table--border, .el-table--group{
    border: none !important;;
  }
  .el-table--border::after, .el-table--group::after, .el-table::before{
    background: none !important;;
  }
  .el-table__fixed-right::before, .el-table__fixed::before{
    background: none !important;;
  }
  .el-table__fixed-right-patch{
    background: #C0ECAA !important;;
  }
  .el-table td, .el-table th.is-leaf{
    border: none !important;;
  }
  .el-table .cell{
    height: 40px !important;;
    line-height: 40px !important;;
    overflow: hidden !important;;
    text-overflow: ellipsis !important;;
    white-space: nowrap !important;;
  }
  .el-table .cell .td-content{
    width: 100% !important;;
    overflow: hidden !important;;
    text-overflow: ellipsis !important;;
    white-space: nowrap !important;;
  }
  /*分页插件*/
  .el-pagination{
    text-align: center !important;
  }

  /* 高德地图样式 */
  .amap-marker-label{
      border:solid 1px #ddd;
      padding: 10px;
  }

  @media (max-width: 1440px) {
    .el-table td,
    .el-table th{
      padding: 0!important;
      height: 32px!important;
      text-align: center;
    }
    .el-table .cell{
      height: 32px !important;;
      line-height: 32px !important;;
      overflow: hidden !important;;
      text-overflow: ellipsis !important;;
      white-space: nowrap !important;;
    }
    .el-pagination .el-input__inner {
      height: 32px !important;;
      line-height: 32px !important;;
    }

  }

  /* 滚动条 */
  /*滚动条整体部分,必须要设置*/
  ::-webkit-scrollbar{
      width: 8px;
      height: 8px;
      background-color: #fff;
  }
  /*滚动条的轨道*/
  ::-webkit-scrollbar-track{
      background-color: rgb(207, 207, 207);
      border-radius: 10px;
  }
  /*滚动条的滑块按钮*/
  ::-webkit-scrollbar-thumb{
      border-radius: 10px;
      background-color: rgb(151, 151, 151);
  }
  /*滚动条的上下两端的按钮*/
  ::-webkit-scrollbar-button{
  }

  .amap-logo{
    z-index: 0!important;
  }
  .amap-copyright{
    z-index: 0!important;
  }
</style>
