<template>
  <div>
    <div class="top-page">
    <h1>Ryoichi</h1>
    <p>そこら辺にいる中学生が作ったポートフォリオサイト</p>
    </div>
    <div class="about">
      <h1>About</h1>
      <div class="explanation">
        <img class="profile-img" src="/Profile.png">
          <div class="right">  
            <p class="title">Ryoichi</p>
            <p class="text">中学校１年の時に始めてプログラミングを学んだ。</p>
            <p class="text">趣味はゲームをしたり、アニメを見たりする事です。</p>
            <p class="text">プロフィールの写真は修学旅行で撮った写真でお気に入りです。</p>
            <p class="text">「僕のSNSリンク」</p>
            <div class="sns-icon">
            <a href="https://twitter.com/Ryo211222"><img class="x-icon" src="/X-icon.png"></a>
            <a href="https://github.com/RyoichiKami"><img class="github-icon" src="/github-mark.png"></a>
          </div>
          </div>  
      </div>
    </div>
    <div class="skill">
      <h1>SKILL</h1>
      <div class="my-skill">
      <p>HTML・CSS・JavaScript・Rubyが使えます。</p>
      <p>フレームワークは、JavaScriptがNuxt.jsでRubyがRailsです。</p>
      <p>このポートフォリオサイトもNuxt.jsで作りました。</p>
      <p>GoやTypeScriptも習いたいです。</p>
      </div>
    </div>
    <div class="projects">
      <h1>Project</h1>
      <div class="project-list">
      <div class="project">
            <img src="https://via.placeholder.com/300x200">
            <h2>作品の名前</h2>
            <p>作品1の説明文や特徴などをここに記述します。</p>
            <a href="#">詳細を見る</a>
        </div>
        <div class="project">
            <img src="https://via.placeholder.com/300x200">
            <h2>作品の名前</h2>
            <p>作品2の説明文や特徴などをここに記述します。</p>
            <a href="#">詳細を見る</a>
        </div>
        <div class="project">
            <img src="https://via.placeholder.com/300x200">
            <h2>作品の名前</h2>
            <p>作品3の説明文や特徴などをここに記述します。</p>
            <a href="#">詳細を見る</a>
        </div>
         
      </div>
     <div class="project-link">
      <p>全ての作品はこちら</p>
      <nuxt-link to="/projects">ALL Projects</nuxt-link>
      </div>
    </div>
    <div class="contact">
      <h1>Contact</h1>
      <p>連絡はこちらから</p> 
      <nuxt-link to="/contact">Contact Me</nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Index',
}
</script>

<style scoped>
.top-page { 
  text-align: center;
  margin-top: 170px;
  margin-bottom: 170px;
}

.about {
  margin-bottom: 100px;
}

.about h1 {
  text-align: center;
  border-bottom: 5px solid #b8e8de;
  padding: 10px;
}

.explanation {
  display: flex;
  padding-top: 100px;
}

.explanation .profile-img {
  width: 20%; /*画像サイズ指定*/
  margin: 0;
  padding: 0;
  border-radius: 50%;
  overflow: hidden;
  position: relative;
  left: 300px;
}

.explanation .right {
  margin: 0 0 0 500px;
  padding: 0;
}

.explanation .title{
  margin: 0;
  padding: 0;
  font-weight: bold;
  font-size: 18px;
}

.explanation .text {
  margin: 10px 0 0;
  padding: 0;
}

.sns-icon {
  padding-top: 15px;
  position: relative;
}
.x-icon {
  width: 9%; /*画像サイズ指定*/
  margin: 0;
  padding: 0;
}

.github-icon {
  width: 7%; /*画像サイズ指定*/
  margin: 0;
  padding: 0;
  margin-bottom: 10px;
  position: relative;
  left: 10px;
}


.skill {
  margin-bottom: 50px;
}

.skill h1 {
  border-bottom: 5px solid #b8e8de;
  text-align: center;
  padding: 10px;
}

.my-skill {
  display: flex;
  flex-direction: column; /* 列に配置する */
  align-items: center; /* 列を中央揃えにする */
}

.my-skill p {
  width: 40%;
  margin: 10px;
  padding: 1px;
}

.projects {
  margin-bottom: 200px;
}
.projects h1 {
  border-bottom: 5px solid #b8e8de;
  text-align: center;
  padding: 10px;
}

.project-link {
 text-align: center;
 top: 450px;
}

.project-link p {
  padding-bottom: 20px;
}

.projects-link a {
  text-decoration: none;
  color: black;
}

.project-list {
  display: flex;
    flex-wrap: wrap;
    justify-content: space-around;
    padding: 30px;
    padding: 10px;
}

.project {
    box-sizing: border-box;
    width: 330px;
    margin: 20px;
    padding: 15px;
    border: 1px solid #ddd; 
    border-radius: 8px;
}

.project-link a:hover {
  color: white;
}

.contact {
  margin-bottom: 110px;
  text-align: center;
}

.contact h1 {
  border-bottom: 5px solid #b8e8de;
  text-align: center;
  padding: 20px;
}

.contact a {
  text-decoration: none;
  color: black;
  line-height: 20px;
  background-color: #b8e8de;
  padding: 10px 5px 10px 5px;
  border-radius: 10px;
  position: relative;
  top: 20px;
}

.contact a:hover {
  color: white;
}

</style>
