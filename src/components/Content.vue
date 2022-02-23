<template>
  <div class="content">
    <div class="content__header">
      <h3 class="content__header-title">
        <span class="content__header-name">Ví BZI</span>
        <span class="content__header-label">Ví BZI</span>
      </h3>
      <div class="f content__header-content">
        <div class="content__header-search">
          <svg class="content__header-search-icon" width="15" height="15" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M13.89 13.574c.165.146.165.301 0 .465l-.6.602c-.165.164-.32.164-.466 0l-3.308-3.309c-.073-.073-.11-.146-.11-.219v-.383c-1.075.93-2.315 1.395-3.719 1.395-1.567 0-2.907-.556-4.019-1.668C.556 9.345 0 8.005 0 6.437 0 4.87.556 3.53 1.668 2.418 2.78 1.306 4.12.75 5.688.75c1.567 0 2.907.556 4.019 1.668 1.112 1.112 1.668 2.452 1.668 4.02 0 1.403-.465 2.643-1.395 3.718h.383a.26.26 0 0 1 .219.11l3.309 3.308ZM2.599 9.527c.856.857 1.886 1.286 3.09 1.286 1.203 0 2.233-.429 3.09-1.286.856-.856 1.284-1.886 1.284-3.09 0-1.203-.428-2.233-1.285-3.09-.856-.856-1.886-1.284-3.09-1.284-1.203 0-2.233.428-3.09 1.285-.856.856-1.284 1.886-1.284 3.09 0 1.203.428 2.233 1.285 3.09Z" fill="#28293D"/>
          </svg>
          <input class="content__header-input" type="text" placeholder="Nhập mã giao dịch bạn muốn tìm" v-model="searchValue">
        </div>
        <div class="button content__header-button">
          <svg width="16" height="16" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M3 2h10L7.99 8.3 3 2ZM.25 1.61C2.27 4.2 6 9 6 9v6c0 .55.45 1 1 1h2c.55 0 1-.45 1-1V9s3.72-4.8 5.74-7.39A.998.998 0 0 0 14.95 0H1.04C.21 0-.26.95.25 1.61Z" fill="#28293D"/>
          </svg>
        </div>
      </div>
      <label v-if="finalData.length === 0" class="message">Sorry, nothing found for <b>{{ searchResultString }}</b></label>
    </div>
    <div class="f content__wrapper">
      <div class="content__left">
        <div class="content__info">
          <div class="content__info-title">Ví BZI</div>
          <div class="card">
            <div class="card__inner">
              <div class="f aic jcb card__header">
                <div class="f fdc card__title">
                  <h4 class="card__label">Ví BZI</h4>
                  <p class="card__description">Khách hàng mới</p>
                </div>
                <div class="button button--icon">
                  <svg width="20" height="20" fill="none" xmlns="http://www.w3.org/2000/svg">
                    <path d="M10 0C4.48 0 0 4.48 0 10s4.48 10 10 10 10-4.48 10-10S15.52 0 10 0Zm0 18c-4.41 0-8-3.59-8-8s3.59-8 8-8 8 3.59 8 8-3.59 8-8 8Zm.31-8.86c-1.77-.45-2.34-.94-2.34-1.67 0-.84.79-1.43 2.1-1.43 1.38 0 1.9.66 1.94 1.64h1.71c-.05-1.34-.87-2.57-2.49-2.97V3H8.9v1.69c-1.51.32-2.72 1.3-2.72 2.81 0 1.79 1.49 2.69 3.66 3.21 1.95.46 2.34 1.15 2.34 1.87 0 .53-.39 1.39-2.1 1.39-1.6 0-2.23-.72-2.32-1.64H6.04c.1 1.7 1.36 2.66 2.86 2.97V17h2.34v-1.67c1.52-.29 2.72-1.16 2.73-2.77-.01-2.2-1.9-2.96-3.66-3.42Z" fill="url(#a)"/><defs><linearGradient id="a" x1="10" y1="0" x2="10" y2="20" gradientUnits="userSpaceOnUse"><stop stop-color="#F41436"/><stop offset="1" stop-color="#A50000"/></linearGradient></defs>
                  </svg>
                  Nạp tiền
                </div>
              </div>
              <p class="card__price">15.000.000VNĐ</p>
              <p class="card__price-info">Số dư trong ví</p>
              <div class="f jcb card__status">
                <div class="card__status-left">
                  <div class="card__status-name">Tên chủ thẻ</div>
                  <div class="card__status-value">Nguyễn Thị Bill</div>
                </div>
                <div class="card__status-right">
                  <div class="card__status-name">Trạng thái</div>
                  <div class="card__status-value">Đã liên kết thẻ thanh toán</div>
                </div>
              </div>
            </div>
          </div>
          <div class="content__footer">
            <div class="content__footer-title">Thẻ đang liên kết</div>
            <div class="f content__footer-content">
              <img src="../assets/images/bank.png" alt="bank logo">
              <div class="content__footer-description">
                <div class="content__footer-name">Nguyễn Thị Bill</div>
                <div class="content__footer-number">123 456 789 123</div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="content__right">
        <div class="table-wrapper">
          <table class="table-list">
            <thead>
              <th>
                <input id="check_all" type="checkbox" name="check_all" class="form__checkbox" :checked="isChecked" ref="checkAll">
                <label for="check_all" class="form__label form__label--checkbox" @click="handleCheckAll"/>
              </th>
              <th>STT</th>
              <th>Loại hình giao dịch</th>
              <th>Ngày khởi tạo</th>
              <th>Tổng giao dịch</th>
              <th>Trạng thái giao dịch</th>
              <th>Hành động</th>
            </thead>
            <tr
                v-for="(item, index) in finalData"
                :key="item.id"
                class="content__item"
            >
              <td>
                <div class="form">
                  <input :id="item.id" type="checkbox" :name="item.id" class="form__checkbox" :checked="isChecked">
                  <label :for="item.id" class="form__label form__label--checkbox" @click="userChecked(item.id)"/>
                </div>
              </td>
              <td>{{ handleNo(index + 1) }}</td>
              <td>
                <p class="label">{{ item.name }}</p>
                <p>{{ item.id }}</p>
              </td>
              <td>{{ item.date }}</td>
              <td>{{ item.price }}</td>
              <td>
                <button :class="['button', {'button--success': item.status}]">
                  {{ handleStatus(item) }}
                </button>
              </td>
              <td><a :href="handleDetail(item)">Xem chi tiết</a></td>
            </tr>
          </table>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
const endpoint = 'http://localhost:3001/stores'
export default {
  name: 'Content',
  data () {
    return {
      userData: [],
      finalData: [],
      isChecked: false,
      searchValue: '',
      searchResultString: ''
    }
  },
  watch: {
    searchValue (newValue) {
      this.filterData(newValue)
    }
  },
  async created () {
    this.userData = await this.fetchProductData(endpoint)
    this.finalData = this.userData
  },
  methods: {
    async fetchProductData (handle) {
      const response = await fetch(handle)
      return response.json()
    },
    handleStatus (user) {
      return user.status ? 'Nạp thành công' : 'Nạp thất bại'
    },
    handleDetail (user) {
      return `/user/${user.id}`
    },
    handleNo (number) {
      return number < 10 ? `0${number}.` : number
    },
    userChecked (user) {
      return user.id
    },
    handleCheckAll () {
      const checkAllEl = this.$refs.checkAll
      checkAllEl && checkAllEl.checked ? this.isChecked = true : this.isChecked = false
    },
    convertText (str) {
      str = str.replace(/à|á|ạ|ả|ã|â|ầ|ấ|ậ|ẩ|ẫ|ă|ằ|ắ|ặ|ẳ|ẵ/g, 'a')
      str = str.replace(/è|é|ẹ|ẻ|ẽ|ê|ề|ế|ệ|ể|ễ/g, 'e')
      str = str.replace(/ì|í|ị|ỉ|ĩ/g, 'i')
      str = str.replace(/ò|ó|ọ|ỏ|õ|ô|ồ|ố|ộ|ổ|ỗ|ơ|ờ|ớ|ợ|ở|ỡ/g, 'o')
      str = str.replace(/ù|ú|ụ|ủ|ũ|ư|ừ|ứ|ự|ử|ữ/g, 'u')
      str = str.replace(/ỳ|ý|ỵ|ỷ|ỹ/g, 'y')
      str = str.replace(/đ/g, 'd')
      str = str.replace(/À|Á|Ạ|Ả|Ã|Â|Ầ|Ấ|Ậ|Ẩ|Ẫ|Ă|Ằ|Ắ|Ặ|Ẳ|Ẵ/g, 'A')
      str = str.replace(/È|É|Ẹ|Ẻ|Ẽ|Ê|Ề|Ế|Ệ|Ể|Ễ/g, 'E')
      str = str.replace(/Ì|Í|Ị|Ỉ|Ĩ/g, 'I')
      str = str.replace(/Ò|Ó|Ọ|Ỏ|Õ|Ô|Ồ|Ố|Ộ|Ổ|Ỗ|Ơ|Ờ|Ớ|Ợ|Ở|Ỡ/g, 'O')
      str = str.replace(/Ù|Ú|Ụ|Ủ|Ũ|Ư|Ừ|Ứ|Ự|Ử|Ữ/g, 'U')
      str = str.replace(/Ỳ|Ý|Ỵ|Ỷ|Ỹ/g, 'Y')
      str = str.replace(/Đ/g, 'D')
      return str
    },
    filterData (data) {
      const searchInputValue = data.replace(/^\s+|\s+$/g, '').toLowerCase().trim().split(' ')
      this.searchResultString = searchInputValue.join(' ')
      this.finalData = this.userData.filter(item => {
        const itemTitle = item.name_handle.replace(/^\s+|\s+$/g, '').toLowerCase().trim()
        return searchInputValue.some(item => itemTitle.includes(item))
      })
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.content {
  padding: 0 18px 100px;
}

@media (min-width: 1024px) {
  .content {
    padding: 0 112px 180px;
  }
}

.content__header {
  margin: 32px 0 37px;
}

.content__header-title {
  margin: 0;
}

.content__header-name {
  display: inline-block;
  padding-right: 16px;
  color: var(--c-black);
  border-right: 1px solid var(--c-light-gray-2);
  font-size: 24px;
  font-weight: var(--fw-bold);
  line-height: 36px;
}

.content__header-label {
  display: inline-block;
  padding-left: 16px;
  color: var(--c-red);
  font-size: 16px;
  font-weight: var(--fw-bold);
  line-height: 24px;
}

.content__header-content {
  margin-top: 24px;
}

.content__header-search {
  position: relative;
  width: 100%;
  max-width: 450px;
  background: var(--c-white);
  border: 1px solid var(--c-light-gray-2);
  border-radius: 4px;
}

.content__header-input {
  width: -webkit-fill-available;
  padding-left: 38px;
  border: none;
}

.content__header-search-icon {
  position: absolute;
  top: 50%;
  left: 12px;
  width: 15px;
  height: 15px;
  transform: translateY(-50%);
}

.content__header-button {
  min-width: auto;
  max-width: 64px;
  height: 45px;
  margin-left: 8px;
  background: var(--c-white);
  border: 1px solid var(--c-light-gray-2);
  box-sizing: border-box;
  border-radius: 8px;
}

.content__left {
  width: 100%;
}

@media (min-width: 1024px) {
  .content__left {
    max-width: 337px;
  }
}

.content__right {
  width: 100%;
}

@media (min-width: 1024px) {
  .content__right {
    width: calc(100% - 337px);
    padding-left: 32px;
  }
}

.table-wrapper {
  overflow-x: auto;
}

.table-list {
  width: 100%;
  border-spacing: 0 16px;
  border-collapse: separate;
}

th {
  text-align: left;
}

td {
  padding: 10px 0;
  color: var(--c-light-blue-1);
  background: var(--c-white);
  font-size: 14px;
  line-height: 21px;
}

th:first-child,
tr td:first-child {
  min-width: 50px;
  padding-left: 20px;
  border-top-left-radius: 8px;
  border-bottom-left-radius: 8px;
}

th:nth-child(2),
td:nth-child(2) {
  min-width: 50px;
}

tr td:last-child {
  border-top-right-radius: 8px;
  border-bottom-right-radius: 8px;
}

th,
td {
  min-width: 150px;
}

th p,
td p {
  margin: 0;
  padding: 0;
}

.content__item {
  background: var(--c-white);
}

.form {
  display: inherit;
}

@media (max-width: 1023px) {
  .content__wrapper {
    flex-direction: column;
  }
}

.content__info {
  padding: 16px 20px;
  background: var(--c-white);
  border-radius: 8px;
}

.content__info-title {
  color: var(--c-red);
  font-size: 16px;
  font-weight: var(--fw-bold);
  line-height: 24px;
}

.card__title {
  font-size: 17px;
  font-weight: var(--fw-bold);
  line-height: 21px;
}

.card {
  margin: 16px 0;
  color: var(--c-white);
  border-radius: 26px;
  background: var(--c-red);
}

.card__inner {
  padding: 16px;
  background: url("../assets/images/round.png") 95px 90px no-repeat;
}

.card__description {
  font-size: 8px;
  font-weight: var(--fw-bold);
  line-height: 10px;
}

.card__price {
  font-size: 21.4918px;
  font-weight: var(--fw-medium);
  line-height: 27px;
}

.card__price-info,
.card__status-name {
  font-size: 10px;
  line-height: 20px;
}

.card__label {
  margin: 0;
}

.content__footer {
  padding-top: 16px;
  border-top: 1px solid var(--c-light-gray-2);
}

.content__footer-title,
.content__footer-name {
  color: var(--c-red);
  font-size: 16px;
  font-weight: var(--fw-bold);
  line-height: 24px;
}

.content__footer-content {
  margin-top: 16px;
}

.content__footer-description {
  margin-left: 16px;
}

.content__footer-name {
  color: var(--c-dark-blue-1);
}

.content__footer-number {
  margin-top: 4px;
  color: var(--c-light-blue-1);
}

.card__status-value {
  font-size: 13px;
  font-weight: var(--fw-medium);
  line-height: 15px;
}

.card__status-right {
  margin-left: 24px;
}
</style>
