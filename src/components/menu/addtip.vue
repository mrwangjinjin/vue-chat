<template>
 <div class="add-content">
   <div>
    <a @click="showSearchFriendDialog" class="iconsize wx-chat-icon"><i class="iconfont icon-pengyou iconhover"></i> 添加好友 </a>
   </div> 
   <div>
    <a class="iconsize wx-chat-icon"><i class="iconfont icon-pengyou iconhover"></i> 创建群聊 </a>
   </div>
  </div>
</template>

<script>
export default {
	name: 'addtip',
	methods: {
		showSearchFriendDialog(){
             this.$store.state.showSearchFriendDialog = true;
		}
	}    
}
</script>

<style scoped>
.add-content {
	position: absolute;
	background: #fff;
	width: 112px;
	text-align: center;
	top: 230px;
	z-index: 20;
	padding: 8px 0;
	box-shadow: 0 2px 6px 0 rgba(0,0,0,0.2);
	border-radius: 4px
}
.add-content a {
	display: flex;
	align-items: center;
	justify-content: center;
	height: 40px;
	position: relative;
	cursor: pointer;
	font-size: 14px;
	color: #333
}

.add-content a .iconfont {
	font-size: 16px;
	color: #333;
	margin-right: 8px
}

.add-content a:hover {
	color: #09ab9b
}

.add-content a:hover i {
	color: #09ab9b
}

.iconhover:hover {
	color: #09ab9b
}

.iconhover.on:hover {
	color: #009788
}
</style>