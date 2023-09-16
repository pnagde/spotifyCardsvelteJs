<script>
  import poster from "$lib/images/Heeriye.jpg";
  import playButton from "$lib/images/Button.png";
</script>

<body class="center">
  <div id="card">
    <div class="main">
        <div class="poster">
            <img id="image" src={poster} alt="poster" />
            <img id="play" src={playButton} alt="play button"/>
          </div>
          <div class="body">
            <span class="title">Todays’s Top Hits</span>
            <br />
            <span class="description">
              Heeriye is on the top of the hottest 50!
            </span>
          </div>
    </div>
  </div>
</body>

<style>
  #play {
    position: absolute;
    bottom: 0;
    right: 0;
    padding: 20px;
    opacity: 0;
    cursor: pointer;
  }
  .description {
    color: grey;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    font-weight: 400;
    font-size: 14px;
  }
  .poster {
    position: relative;
  }
  .body {
    padding-left: 10px;
    padding-right: 10px;
  }
  .title {
    color: white;
    font-family: "Segoe UI", Tahoma, Geneva, Verdana, sans-serif;
    font-weight: bold;
    font-size: 20px;
  }
  .poster #image {
    height: 225px;
    width: 225px;
    object-fit: cover;
    margin: 12px;
    border-radius: 10px;
  }
  .center {
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .main{
    height: 330px;
    width: 250px;
  }
  #card {
    height: 330px;
    width: 250px;
    background-color: #222222;
    box-shadow: 2px 2px 10px #222222;
    border-radius: 10px;
  }
  #card :hover {
    border-radius: 10px;
    background-color: #4b4a4a;
  }
  #card :hover #play {
   opacity: 1;
  }
  #play:hover{
    background-color: transparent;
  }
</style>
