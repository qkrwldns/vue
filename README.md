# vue 사나래 더미페이지 
https://codingapple.com/unit/vue-build-and-deploy-with-github-pages/

만든 vue 페이지 정적페이지로 호스팅, 나중에 다시 코드 바꾸면 yarn build하고 dist 폴더안의 파일들을 여기에 올리면 됨 

근데 route가 안먹혀서 
import { createWebHistory, createRouter } from "vue-router"; 이거를 import { createRouter, createWebHashHistory } from 'vue-router'; 이걸로 바꾸고   
const router = createRouter({
  history: createWebHashHistory(),
  routes,
});

export default router;

이렇게 하니까 됐음 
