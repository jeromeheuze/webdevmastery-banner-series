<template>
  <div class="pixels container-fluid">
    <nav>
      <div class="menu-icon"><em></em><em></em><em></em></div>
      <ul>
        <li><a class="active" href="javascript:;">Home</a></li>
        <li><a href="javascript:;">About Us</a></li>
        <li><a href="javascript:;">Shop</a></li>
        <li><a href="javascript:;">Contact Us</a></li>
        <li><a class="btn primary" href="javascript:;">Log In</a></li>
      </ul>
    </nav>
    <div class="hero">
      <div class="text">
        <h1>Retro Game Station</h1>
        <p>Best place to buy all the retro games and gaming consoles in one place.</p>
        <a href="javascript:;" class="btn secondary">Shop Online</a>
      </div>
      <div class="graphic">
        <div class="img_overlay">
          <img src="https://storage.googleapis.com/tutorial_asset/pngfind.com-nintendo-nes-png-4992364.png" alt="retro gaming" width="1047" height="729"/>
        </div>
      </div>
    </div>
    <div class="below">
      <div class="arrows">
        <div class="down"></div><div class="second"></div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    layout: 'retro'
  }
</script>

<style lang="scss">
.pixels {
  a, p {
    font-family: 'Kenney Future', sans-serif;
  }
  a.btn {
    color: #d6acf7;
    padding: 10px 20px;
    text-decoration: none;
    &.primary {
      border: 1px solid #fff;
      border-radius: 10px;
      &:hover, &:active {
        border-color: #d6acf7;
        color: #d6acf7;
      }
    }
    &.secondary {
      border: 1px solid #d6acf7;
      border-radius: 10px;
      box-shadow: 0 0 10px 0 rgba(214,172,247,0.81);
      -webkit-box-shadow: 0 0 10px 0 rgba(214,172,247,0.81);
      -moz-box-shadow: 0 0 10px 0 rgba(214,172,247,0.81);
      &:hover, &:active {
        border-color: #d6acf7;
        background: #d6acf7;
        color: #111;
      }
    }
  }
  nav {
    margin: 4rem 2rem 1rem 2rem;
    display: flex;
    align-content: space-between;
    justify-content: space-between;
    align-items: center;
    .menu-icon {
      width: 30px;
      height: 30px;
      cursor: pointer;
      &:hover em, &:active em {
        background: #f1b125;
      }
      em {
        display: block;
        width: 100%;
        height: 1px;
        background: #fff;
        margin-bottom: 5px;
        &:last-child {
          margin-bottom: 0;
        }
      }
    }
    ul {
      list-style-type: none;
      display: flex;
      li {
        padding: 1rem;
        margin: 0.5rem 1rem;
        a {
          color: #fff;
          font-size: 1em;
          line-height: 1.1em;
          font-family: 'Kenney Future', sans-serif;
          text-decoration: none;
          &:hover, &:active, &.active {
            color: #f1b125;
          }
        }
      }
    }
  }
  .hero {
    display: flex;
    justify-content: center;
    align-content: center;
    align-items: center;
    height: 80vh;
    .text {
      padding: 10rem 5rem;
      h1 {
        font-family: 'Kenney Thick', sans-serif;
        font-size: 5em;
        line-height: 1.5em;
        color: #f1b125;
        text-shadow: 0 10px 0 rgba(255,255,255,1);
      }
      p {
        width: 80%;
        color: #fff;
        font-size: 1.4em;
        text-transform: uppercase;
        margin: 4rem 0;
      }
      a.btn {
        text-transform: uppercase;
      }
    }
    .graphic {
      .img_overlay {
        img {
          width: 75%;
          height: 75%;
        }
      }
    }
  }
  .below {
    display: flex;
    align-items: center;
    justify-content: center;
    .arrows {
      position: relative;
      .down {
        box-sizing: border-box;
        height: 30px;
        width: 30px;
        border-style: solid;
        border-color: #63616a;
        border-width: 0 1px 1px 0;
        transform: rotate(45deg);
        position: absolute;
        bottom: 15px;
      }
      .second {
        box-sizing: border-box;
        height: 30px;
        width: 30px;
        border-style: solid;
        border-color: #f1b125;
        border-width: 0 1px 1px 0;
        transform: rotate(45deg);
        position: absolute;
        bottom: 0;
      }
    }
  }
}
</style>
