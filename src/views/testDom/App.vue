<template>
  <div class="ATTADreamMaker-dom">
    <div class="MaskNetworkbox">
      <div class="MaskNetwork" @click="ATTAMakerVisible = true;test()">
         <el-dropdown trigger="click">
           <div class="flex">
            <svg xmlns="http://www.w3.org/2000/svg" width="26.25" height="26.25" viewBox="0 0 24 24" fill="none">
              <path d="M12.1707 9.37146C10.5345 9.37146 9.20312 10.7028 9.20312 12.339C9.20312 13.9752 10.5345 15.3065 12.1707 15.3065C13.8069 15.3065 15.1382 13.9752 15.1382 12.339C15.1382 10.7028 13.8069 9.37146 12.1707 9.37146ZM12.1707 13.7447C11.3953 13.7447 10.765 13.1143 10.765 12.339C10.765 11.5637 11.3953 10.9333 12.1707 10.9333C12.946 10.9333 13.5763 11.5637 13.5763 12.339C13.5763 13.1143 12.946 13.7447 12.1707 13.7447Z" fill="black" stroke="black" stroke-width="0.2"/>
              <path d="M22.7213 17.7489L15.2147 3.9221C14.5613 2.7187 13.3806 2 12.0571 2C10.7337 2 9.55303 2.7187 8.89959 3.9221L1.39297 17.7489C0.595009 19.2186 1.12165 20.695 1.99729 21.5057C2.93176 22.3703 4.24322 22.5157 5.33877 21.8756L6.71877 21.07C8.35124 20.1167 10.1973 19.6125 12.0571 19.6125C13.9169 19.6125 15.7625 20.1162 17.3955 21.07L18.7755 21.8756C19.2296 22.1408 19.7214 22.2711 20.2075 22.2711C20.8941 22.2711 21.5698 22.0115 22.117 21.5057C22.9926 20.695 23.5193 19.2186 22.7213 17.7489ZM21.134 20.495C20.9078 20.7039 20.2972 21.1407 19.5089 20.6805L18.1289 19.8749C16.2748 18.7924 14.1751 18.2197 12.0571 18.2197C9.93916 18.2197 7.83945 18.7919 5.98536 19.8749L4.60536 20.6805C3.81711 21.1407 3.20651 20.7039 2.98031 20.495C2.49594 20.0465 2.20692 19.2248 2.65473 18.4008L10.1614 4.57394C10.5629 3.83463 11.2718 3.39282 12.0571 3.39282C12.8425 3.39282 13.5514 3.83407 13.9529 4.57394L21.4596 18.4008C21.9068 19.2253 21.6183 20.0465 21.134 20.495Z" fill="black" stroke="black" stroke-width="0.5"/>
            </svg>
            <p class="wordtitle">ATTA Dream Maker</p>
           </div>
          <el-dropdown-menu slot="dropdown">
              <el-dropdown-item>Create NFT</el-dropdown-item>
              <el-dropdown-item>Create poster NFT</el-dropdown-item>
              <el-dropdown-item>Create Co-NFT</el-dropdown-item>
              <el-dropdown-item>NFT Hall</el-dropdown-item>
              <el-dropdown-item>My NFTs</el-dropdown-item>
          </el-dropdown-menu>
        </el-dropdown>



        
      </div>
      <!-- <el-dialog
        :visible.sync="ATTAMakerVisible"
        width="20%"
        :modal="false"
        :show-close="false"
        custom-class="MaskNetwork-dialogbox"
      >
        <el-button @click="ATTAMakerVisible = false">Create NFT</el-button>
        <el-button @click="ATTAMakerVisible = false">Create poster NFT</el-button>
        <el-button @click="ATTAMakerVisible = false">Create Co-NFT</el-button>
        <el-button @click="ATTAMakerVisible = false">NFT Hall</el-button>
        <el-button @click="ATTAMakerVisible = false">My NFTs</el-button>
      </el-dialog> -->
    </div>
    <div class="ConnectWalletbox">
      <div class="ConnectWallet flex" @click="ConnectWalletloading = true">
        <svg xmlns="http://www.w3.org/2000/svg" width="26.25" height="26.25" viewBox="0 0 24 24" fill="none">
          <path d="M11.8736 7.54291C10.4022 7.54291 9.20508 8.74007 9.20508 10.2114C9.20508 11.6827 10.4022 12.8799 11.8736 12.8799C13.3449 12.8799 14.542 11.6827 14.542 10.2114C14.542 8.74007 13.3449 7.54291 11.8736 7.54291ZM11.8736 11.4754C11.1764 11.4754 10.6095 10.9086 10.6095 10.2114C10.6095 9.51421 11.1764 8.94737 11.8736 8.94737C12.5707 8.94737 13.1376 9.51421 13.1376 10.2114C13.1376 10.9086 12.5707 11.4754 11.8736 11.4754Z" fill="black" stroke="black" stroke-width="0.2"/>
          <path d="M21.3605 15.0761L14.6103 2.6427C14.0227 1.56058 12.9611 0.914307 11.771 0.914307C10.5809 0.914307 9.51922 1.56058 8.93163 2.6427L2.18149 15.0761C1.46395 16.3977 1.93752 17.7253 2.72491 18.4543C3.56521 19.2318 4.74451 19.3626 5.72965 18.7869L6.97059 18.0625C8.43854 17.2053 10.0986 16.7519 11.771 16.7519C13.4434 16.7519 15.1029 17.2048 16.5714 18.0625L17.8123 18.7869C18.2206 19.0254 18.6629 19.1426 19.1 19.1426C19.7174 19.1426 20.325 18.9092 20.8171 18.4543C21.6044 17.7253 22.078 16.3977 21.3605 15.0761ZM19.9331 17.5455C19.7297 17.7334 19.1806 18.1261 18.4718 17.7123L17.2309 16.9879C15.5636 16.0145 13.6755 15.4995 11.771 15.4995C9.86644 15.4995 7.97833 16.014 6.31108 16.9879L5.07015 17.7123C4.36134 18.1261 3.81227 17.7334 3.60887 17.5455C3.17331 17.1422 2.91342 16.4032 3.3161 15.6623L10.0662 3.22886C10.4273 2.56405 11.0647 2.16677 11.771 2.16677C12.4772 2.16677 13.1146 2.56355 13.4757 3.22886L20.2259 15.6623C20.628 16.4037 20.3686 17.1422 19.9331 17.5455Z" fill="black" stroke="black" stroke-width="0.5"/>
          <path d="M7.18172 20.269C6.95236 20.0905 6.66469 20 6.32566 20C5.97009 20 5.65673 20.1384 5.39474 20.4108C5.13274 20.6781 5 21.0214 5 21.4318C5 21.8423 5.13274 22.1856 5.39474 22.4529C5.65848 22.7218 5.97183 22.8585 6.32566 22.8585C6.65816 22.8585 6.94583 22.7692 7.18172 22.5939V22.8223H7.92767V20.037H7.18172V20.269ZM6.95976 21.9907C6.80831 22.1317 6.6364 22.203 6.44795 22.203C6.01535 22.203 5.72463 21.8932 5.72463 21.4318C5.72463 20.9675 6.01535 20.6554 6.44795 20.6554C6.63814 20.6554 6.81005 20.7285 6.95932 20.8726C7.1086 21.0171 7.18128 21.1999 7.18128 21.4314C7.18172 21.6638 7.10947 21.8466 6.95976 21.9907Z" fill="black" stroke="black" stroke-width="0.3"/>
          <path d="M8.92773 20.6981H9.9322V22.8437H10.6782V20.6981H11.6761V20.0366H8.92773V20.6981Z" fill="black" stroke="black" stroke-width="0.3"/>
          <path d="M12.6758 20.6981H13.6802V22.8437H14.4262V20.6981H15.4241V20.0366H12.6758V20.6981Z" fill="black" stroke="black" stroke-width="0.3"/>
          <path d="M18.6055 20.269C18.3762 20.0905 18.0885 20 17.7495 20C17.3939 20 17.0806 20.1384 16.8186 20.4108C16.5566 20.6781 16.4238 21.0214 16.4238 21.4318C16.4238 21.8423 16.5566 22.1856 16.8186 22.4529C17.0823 22.7218 17.3957 22.8585 17.7495 22.8585C18.082 22.8585 18.3697 22.7692 18.6055 22.5939V22.8223H19.3515V20.037H18.6055V20.269ZM18.3836 21.9907C18.2321 22.1317 18.0602 22.203 17.8718 22.203C17.4392 22.203 17.1485 21.8932 17.1485 21.4318C17.1485 20.9675 17.4392 20.6554 17.8718 20.6554C18.062 20.6554 18.2339 20.7285 18.3832 20.8726C18.5329 21.0171 18.6055 21.1999 18.6055 21.4314C18.6055 21.6638 18.5329 21.8466 18.3836 21.9907Z" fill="black" stroke="black" stroke-width="0.3"/>
        </svg>
        <p class="wordtitle">Connect Wallet</p>
      </div>
      <!-- 选择钱包插件 -->
      <el-dialog
        :visible.sync="ConnectWalletVisible"
        width="50%"
        :modal="false"
        custom-class="MaskNetwork-dialogbox"
      >
        <img src="" alt="">
        <el-button @click="ConnectWalletVisible = false">按钮4</el-button>
        <img src="" alt="">
        <el-button @click="ConnectWalletVisible = false">按钮5</el-button>
      </el-dialog>
      <el-dialog
        title="账户"
        :visible.sync="ConnectWalletloading"
        width="50%"
        :modal="false"
      >
        <img src="" alt="">
        <div>
          <p>MetaMask</p>
          <img src="" alt="">
          <p>address地址</p>
          <img src="" alt="">
          <img src="" alt="">
        </div>
        <el-button @click="userwalletdialog()">更改</el-button>
      </el-dialog>
    </div>
  </div>
</template>
<script>
import '../../../public/js/web3/web3.min.js'
import '../../../public/js/web3/web3-provider.min.js'
import '../../../public/js/web3/chainSetting.js'
import '../../../public/js/web3/chainProvider.js'
export default {
  data() {
    return {
      ATTAMakerVisible: false,//ATTA Dream Maker弹框控制
      ConnectWalletVisible: false,//选择钱包插件弹框控制
      ConnectWalletloading: false, // 钱包账户弹框控制
    };
  },
  mounted() {
    console.log(localStorage.getItem("_grecaptcha"),'测试缓存');
    let leftdom = document.querySelector('[aria-label][role="navigation"]');
    let crdom = document.querySelector(".ATTADreamMaker-dom");
    console.log(leftdom);
    leftdom.appendChild(crdom);
  },
  methods: {
    test(){

    console.log(window.CHAIN,'测试数据');
    },
    userwalletdialog(){
      this.ConnectWalletloading = false;
      this.ConnectWalletVisible = true;
    }
  },
};
</script>

<style lang="scss" scoped>
.flex{
  display: flex;
  align-items: center;
}
.MaskNetworkbox,.ConnectWalletbox{
  padding: 6px 14px;
  position: relative;
  transition-property: background-color, box-shadow;
  // transition-duration: 0.2s;
  .MaskNetwork,.ConnectWallet{
    font-weight: 400;
    font-size: 1rem;
    cursor: pointer;
    svg{
      flex-shrink: 0;
    }
    .wordtitle{
      margin: 4px 16px 4px 20px;
      font-family: inherit;
      font-weight: 400;
      font-size: 20px;
      color: rgb(15, 20, 25);
    }
  }
  .MaskNetwork-dialogbox{
    // position: absolute;
  }
}
.MaskNetworkbox:hover,.ConnectWalletbox:hover{
  background: rgba(15, 20, 25, 0.1);
  border-radius: 9999px;
}
</style>
