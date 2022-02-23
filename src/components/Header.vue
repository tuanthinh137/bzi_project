<template>
  <div class="header">
    <div class="f jcb header__inner">
      <div class="f aic header__left">
        <div class="f aic header__logo">
          <a class="header__logo-link" href="/">
            <img src="../assets/images/logo.jpg" alt="logo">
          </a>
        </div>
        <div class="header__language">
          <svg class="header__language-icon" width="20" height="20" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path fill="currentColor" d="M9.99 0C4.47 0 0 4.48 0 10s4.47 10 9.99 10C15.52 20 20 15.52 20 10S15.52 0 9.99 0Zm6.93 6h-2.95a15.65 15.65 0 0 0-1.38-3.56A8.03 8.03 0 0 1 16.92 6ZM10 2.04c.83 1.2 1.48 2.53 1.91 3.96H8.09C8.52 4.57 9.17 3.24 10 2.04ZM2.26 12C2.1 11.36 2 10.69 2 10s.1-1.36.26-2h3.38c-.08.66-.14 1.32-.14 2 0 .68.06 1.34.14 2H2.26Zm.82 2h2.95c.32 1.25.78 2.45 1.38 3.56A7.987 7.987 0 0 1 3.08 14Zm2.95-8H3.08a7.987 7.987 0 0 1 4.33-3.56A15.65 15.65 0 0 0 6.03 6ZM10 17.96c-.83-1.2-1.48-2.53-1.91-3.96h3.82c-.43 1.43-1.08 2.76-1.91 3.96ZM12.34 12H7.66c-.09-.66-.16-1.32-.16-2 0-.68.07-1.35.16-2h4.68c.09.65.16 1.32.16 2 0 .68-.07 1.34-.16 2Zm.25 5.56c.6-1.11 1.06-2.31 1.38-3.56h2.95a8.03 8.03 0 0 1-4.33 3.56ZM14.36 12c.08-.66.14-1.32.14-2 0-.68-.06-1.34-.14-2h3.38c.16.64.26 1.31.26 2s-.1 1.36-.26 2h-3.38Z"/>
          </svg>
        </div>
        <a class="header__link" href="#">Xem gian hàng</a>
      </div>
      <div class="f aic header__right">
        <div class="header__notification">
          <svg class="header__notification-icon" width="22" height="27" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M11 26.333c1.467 0 2.667-1.2 2.667-2.666H8.333c0 1.466 1.2 2.666 2.667 2.666Zm8-8v-6.666c0-4.094-2.173-7.52-6-8.427v-.907c0-1.106-.893-2-2-2s-2 .894-2 2v.907c-3.813.907-6 4.32-6 8.427v6.666L.333 21v1.333h21.334V21L19 18.333Zm-2.667 1.334H5.667v-8c0-3.307 2.013-6 5.333-6 3.32 0 5.333 2.693 5.333 6v8Z" fill="currentColor"/>
          </svg>
        </div>
        <div class="f fdc aic jcc header__user">
          <div class="f jcs header__user-wrapper">
            <div class="header__user-label">Số dư</div>
            <div class="header__user-name">Ví BZI</div>
          </div>
          <div class="f aic jcs header__user-price">
            <div class="f aic jcc header__user-price-info">
              <svg class="header__user-price-icon" width="8" height="7" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3.89 7H2.185V5.814h1.646c.409 0 .753-.072 1.032-.217.281-.147.492-.374.633-.68.143-.31.214-.708.214-1.196 0-.484-.071-.879-.214-1.186a1.386 1.386 0 0 0-.63-.677c-.279-.145-.623-.218-1.032-.218H2.157V.455h1.751c.659 0 1.226.13 1.7.393.476.26.841.634 1.097 1.121.258.488.387 1.072.387 1.752 0 .682-.13 1.268-.387 1.758-.256.49-.623.866-1.103 1.128C5.125 6.869 4.554 7 3.89 7ZM2.952.455V7H1.569V.455h1.384ZM.66 3.95v-.805h3.187v.805H.66Z" fill="#fff"/>
              </svg>
            </div>
            <label class="header__user-price-label">10,660,800</label>
          </div>
        </div>
        <div class="header__account">
          <div class="f aic jcs header__account-wrapper">
            <svg class="icon icon--account" width="28" height="28" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M14 .667C6.64.667.667 6.64.667 14S6.64 27.333 14 27.333 27.333 21.36 27.333 14 21.36.667 14 .667ZM7.427 22.373C8 21.173 11.493 20 14 20c2.507 0 6.013 1.173 6.573 2.373A10.524 10.524 0 0 1 14 24.667c-2.48 0-4.76-.854-6.573-2.294ZM22.48 20.44c-1.907-2.32-6.533-3.107-8.48-3.107s-6.573.787-8.48 3.107A10.6 10.6 0 0 1 3.333 14C3.333 8.12 8.12 3.333 14 3.333S24.667 8.12 24.667 14a10.6 10.6 0 0 1-2.187 6.44ZM14 6a4.655 4.655 0 0 0-4.667 4.667A4.655 4.655 0 0 0 14 15.333a4.655 4.655 0 0 0 4.667-4.666A4.655 4.655 0 0 0 14 6Zm0 6.667c-1.107 0-2-.894-2-2 0-1.107.893-2 2-2s2 .893 2 2c0 1.106-.893 2-2 2Z" fill="currentColor"/><defs><linearGradient id="a" x1="14" y1=".667" x2="14" y2="27.333" gradientUnits="userSpaceOnUse"><stop stop-color="#F41436"/><stop offset="1" stop-color="#A50000"/></linearGradient></defs>
            </svg>
            <div class="header__account-name">Nguyễn Văn Bill</div>
            <svg class="icon icon--arrow" width="12" height="8" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M1.41.59 6 5.17 10.59.59 12 2 6 8 0 2 1.41.59Z" fill="currentColor"/>
            </svg>
          </div>
          <div class="f fdc ais header__account-list">
            <a href="#" class="f aic jcs header__account-link">
              <svg class="icon icon--account-2" width="20" height="20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M10 0C4.48 0 0 4.48 0 10s4.48 10 10 10 10-4.48 10-10S15.52 0 10 0ZM5.07 16.28c.43-.9 3.05-1.78 4.93-1.78s4.51.88 4.93 1.78A7.893 7.893 0 0 1 10 18c-1.86 0-3.57-.64-4.93-1.72Zm11.29-1.45c-1.43-1.74-4.9-2.33-6.36-2.33s-4.93.59-6.36 2.33A7.95 7.95 0 0 1 2 10c0-4.41 3.59-8 8-8s8 3.59 8 8c0 1.82-.62 3.49-1.64 4.83ZM10 4C8.06 4 6.5 5.56 6.5 7.5S8.06 11 10 11s3.5-1.56 3.5-3.5S11.94 4 10 4Zm0 5c-.83 0-1.5-.67-1.5-1.5S9.17 6 10 6s1.5.67 1.5 1.5S10.83 9 10 9Z" fill="url(#a)"/><defs><linearGradient id="a" x1="10" y1="0" x2="10" y2="20" gradientUnits="userSpaceOnUse"><stop stop-color="#FF5A73"/><stop offset="1" stop-color="#A50000"/></linearGradient></defs>
              </svg>
              Truy cập trang tài khoản
            </a>
            <a href="#" class="f aic jcs header__account-link">
              <svg class="icon icon--book" width="18" height="20" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 14h7v2H4v-2Zm0-4h10v2H4v-2Zm0-4h10v2H4V6Zm12-4h-4.18C11.4.84 10.3 0 9 0 7.7 0 6.6.84 6.18 2H2c-.14 0-.27.01-.4.04A2.008 2.008 0 0 0 .16 3.23C.06 3.47 0 3.72 0 4v14c0 .27.06.54.16.78s.25.45.43.64c.27.27.62.47 1.01.55.13.02.26.03.4.03h14c1.1 0 2-.9 2-2V4c0-1.1-.9-2-2-2Zm-7-.25c.41 0 .75.34.75.75s-.34.75-.75.75-.75-.34-.75-.75.34-.75.75-.75ZM16 18H2V4h14v14Z" fill="#28293D"/>
              </svg>
              Chính sách & điều khoản
            </a>
            <a href="#" class="f aic jcs header__account-link">
              <svg class="icon icon--logout" width="18" height="18" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M7.09 12.59 8.5 14l5-5-5-5-1.41 1.41L9.67 8H0v2h9.67l-2.58 2.59ZM16 0H2a2 2 0 0 0-2 2v4h2V2h14v14H2v-4H0v4a2 2 0 0 0 2 2h14c1.1 0 2-.9 2-2V2c0-1.1-.9-2-2-2Z" fill="#28293D"/>
              </svg>
              Đăng xuất
            </a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.header {
  position: sticky;
  z-index: 10;
  top: 0;
  height: 70px;
  background: var(--c-white);
  border-bottom: 1px solid var(--c-light-gray-2);
}

.header__inner {
  height: 100%;
}

.header__logo {
  height: 100%;
  padding: 0 24px;
  border-right: 1px solid var(--c-light-gray-2);
}

.header__logo-link {
  width: 99px;
  height: auto;
}

.header__language {
  margin-left: 12px;
  cursor: pointer;
}

@media (min-width: 1024px) {
  .header__notification {
    margin-left: 26px;
  }
}

.header__language-icon {
  width: 20px;
  height: 20px;
  color: var(--c-blue);
}

.header__link {
  margin-left: 10px;
  color: var(--c-blue);
  font-size: 12px;
  line-height: 18px;
  font-weight: 600;
}

@media (max-width: 767px) {
  .header__link {
    display: none;
  }
}

.header__notification {
  position: relative;
  margin-right: 12px;
  cursor: pointer;
}

@media (min-width: 1024px) {
  .header__notification {
    margin-right: 30px;
  }
}

.header__notification:after {
  content: '';
  position: absolute;
  top: 1px;
  right: 1px;
  width: 8px;
  height: 8px;
  border-radius: 50%;
  background: var(--c-red);
}

.header__notification-icon {
  color: var(--c-light-blue-1);
}

.header__user {
  height: 100%;
  padding: 0 24px;
  border-right: 1px solid var(--c-light-gray-2);
  border-left: 1px solid var(--c-light-gray-2);
  color: var(--c-light-blue-1);
  background: var(--c-light-gray-1);
  font-size: 12px;
  line-height: 18px;
}

.header__user-label {
  color: var(--c-light-blue-1);
  font-size: 12px;
  line-height: 18px;
}

.header__user-name {
  padding-left: 36px;
  color: var(--c-blue);
  font-weight: var(--fw-semibold);
}

.header__user-price-info {
  width: 16px;
  height: 16px;
  background: linear-gradient(180deg, #F41436 0%, #A50000 100%);
  border-radius: 4px;
}

.header__user-price-icon {
  width: 8px;
  height: 8px;
}

.header__user-price-label {
  margin-left: 10px;
  color: var(--c-dark-blue-1);
  font-size: 14px;
  font-weight: 600;
  line-height: 21px;
}

.header__account {
  position: relative;
  display: none;
  height: 100%;
  margin-left: 12px;
}

@media (min-width: 768px) {
  .header__account {
    display: block;
    margin-left: 30px;
    margin-right: 20px;
  }
}

@media (min-width: 1024px) {
  .header__account {
    margin-left: 30px;
    margin-right: 118px;
  }
}

.header__account:hover .header__account-list {
  transform: translateY(4px);
  opacity: 1;
  visibility: visible;
}

.header__account-wrapper {
  height: 100%;
}

.header__account-icon svg {
  width: 27px;
  height: 27px;
  background: linear-gradient(180deg, #F41436 0%, #A50000 100%);
}

.header__account-list {
  position: absolute;
  top: 100%;
  right: 0;
  min-width: 238px;
  padding: 18px;
  background: var(--c-white);
  border-radius: 8px;
  box-shadow: 0px 2px 8px rgba(40, 41, 61, 0.04), 0px 16px 24px rgba(96, 97, 112, 0.16);
  transform: translateY(20px);
  opacity: 0;
  visibility: hidden;
  transition: all .3s ease-in-out;
}

.header__account-link {
  width: 100%;
  padding: 9px 0;
  color: var(--c-dark-blue-1);
  font-size: 14px;
  font-weight: var(--fw-medium);
  line-height: 21px;
}

.header__account-link:hover {
  color: var(--c-light-red-1);
}

.header__account-link:last-child {
  margin-top: 9px;
  padding-top: 20px;
  border-top: 1px solid var(--c-light-gray-2);
}

.header__account-link svg {
  margin-right: 10px;
}
</style>
