<template>
  <div>
    <a  @click="showModal" >
      Login
    </a>
    
     <a-modal v-model="visible" title="Login" on-ok="handleOk">
      <template slot="footer">
        <a-button key="back" @click="handleCancel">
          Return
        </a-button>
        <a-button key="submit" type="primary"  @click="handleOk">
          Submit
        </a-button>
      </template>
      <form action="POST" style="display: flex; flex-direction: column;">
      <label for="" style="margin-right: 10px">Login</label><input type="text" style="border: 1px solid #c3c3c3 !important; padding: 0px 10px;"> 
      <label for="" style="margin-right: 10px">Password</label><input type="text" style="border: 1px solid #c3c3c3 !important; padding: 0px 10px;"> 
      <label for="" style="margin-right: 10px">Email</label><input type="text" style="border: 1px solid #c3c3c3 !important; padding: 0px 10px;"> 
      </form>
      
    </a-modal>
    </div>
</template>
<script>
export default {
  data() {
    return {
      ModalText: 'Content of the modal',
      visible: false,
      confirmLoading: false,
    };
  },
  methods: {
    showModal() {
      this.visible = true;
    },
    handleOk() {
      this.ModalText = 'The modal will be closed after two seconds';
      this.confirmLoading = true;
      setTimeout(() => {
        this.visible = false;
        this.confirmLoading = false;
      }, 2000);
    },
    handleCancel() {
      console.log('Clicked cancel button');
      this.visible = false;
    },
  },
};
</script>
<style lang='scss' scoped>
// @import "../styles/NavBar/styles.scss"
.active{
    color: #1c1c1b !important;
  fill: #1c1c1b !important;
}
</style>