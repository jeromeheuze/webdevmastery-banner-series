<template>
  <div class="crypto container-fluid">
    <header>
      <div class="ribbon">
        <div class="col contact"><span>+1 (415) 000-0000</span> <span>info@cryptocurrency.com</span></div>
        <div class="col social">
          <ul>
            <li><a href="#!"><img src="../static/facebook.svg" alt="Facebook"/></a></li>
            <li><a href="#!"><img src="../static/twitter.svg" alt="Twitter"/></a></li>
            <li><a href="#!"><img src="../static/behance.svg" alt="Behance"/></a></li>
            <li><a href="#!"><img src="../static/instagram.svg" alt="Instagram"/></a></li>
            <li><a href="#!"><img src="../static/youtube.svg" alt="youTube"/></a></li>
          </ul>
        </div>
      </div>
    </header>
    <div class="content">
      <div class="navigation">
        <div class="branding"><a href="#!">crypto<span>currency</span></a></div>
        <nav>
          <ul>
            <li><a href="#!" class="active">Home</a></li>
            <li><a href="#!">About us</a></li>
            <li><a href="#!">Services</a></li>
            <li><a href="#!">Shop</a></li>
            <li><a href="#!">Contact us</a></li>
            <li><a href="#!">Blog</a></li>
            <li><a href="#!" class="btn primary">Sign In</a></li>
          </ul>
        </nav>
      </div>
      <div class="hero">
        <div class="hero-cont">
          <h1>We trade crypto currency<span>.</span></h1>
          <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc vitae felis non magna euismod sodales ut id libero. Donec semper leo metus, et ultrices turpis consectetur eu.</p>
          <a class="btn primary" href="#!">Learn More</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: 'crypto'
}
</script>

<style lang="scss">
.crypto {
  header {
    padding: 0 5rem;
    background: #1b1b1c;
    @media screen and (max-width: 600px) {
      padding: 0 1rem;
    }
    .ribbon {
      display: flex;
      align-content: center;
      justify-content: space-between;
      @media screen and (max-width: 600px) {
        flex-wrap: wrap;
        justify-content: center;
      }
      .col {
        width: fit-content;
        &.contact {
          align-items: flex-start;
          @media screen and (max-width: 600px) {
            text-align: center;
          }
          span {
            display:inline-block;
            padding: 1rem 1rem 0 1rem;
            text-transform: uppercase;
            @media screen and (max-width: 600px) {
              padding: 0 1rem 1rem 1rem;
            }
            &:first-of-type {
              @media screen and (max-width: 600px) {
                padding-top: 1.5rem;
              }
            }
          }
        }
        &.social {
          align-items: flex-end;
          ul {
            list-style-type: none;
            background: #fab915;
            padding: 0;
            li {
              display: inline-block;
              padding: 0.65rem;
              margin: 0;
              &:hover {
                background: #1b1b1c;
              }
              img {
                width: 20px;
                height: 20px;
              }
            }
          }
        }
      }
    }
  }
  .content {
    position: relative;
    .navigation {
      padding: 2.5rem 5rem;
      border-bottom: 1px solid #304496;
      display: flex;
      align-content: center;
      align-items: center;
      justify-content: space-between;
      @media screen and (max-width: 600px) {
        flex-wrap: wrap;
        justify-content: center;
        padding: 0 1rem;
      }
      .branding {
        a {
          text-decoration: none;
          color: #fff;
          font-family: 'Russo One', sans-serif;
          font-size: 2rem;
          span {
            color: #fab915;
          }
        }
      }
      ul {
        list-style-type: none;
        padding: 0;
        li {
          display: inline-block;
          padding: 0.65rem;
          margin: 0;
          a {
            color: #fff;
            text-decoration: none;
            font-size: 1.1rem;
            text-transform: uppercase;
            &:hover {
              color: #fab915;
            }
          }
        }
      }
    }
    .hero {
      position: relative;
      width: 100%;
      height: auto;
      display: block;
      padding: 7rem 5rem;
      h1 {
        font-family: 'Russo One', sans-serif;
        font-size: 7rem;
        line-height: 6rem;
        width: 80%;
        span {
          color: #fab915;
        }
      }
      p {
        padding: 4rem 0;
        font-size: 1.4rem;
        line-height: 1.8rem;
        text-transform: uppercase;
        width: 60%;
      }
      .btn {
        text-transform: uppercase;
        padding: 1rem 1.5rem;
      }
    }
    .btn {
      padding: 0.65rem 1.4rem;
      display: inline-block;
      text-decoration: none;
      &.primary {
        color: #fff;
        background: #fab915;
      }
    }
  }
}
</style>
