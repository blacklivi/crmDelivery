<template>
  <div>
    <div class="blocks_test">
      <v-row class="blocks blocks_one">
        <v-col
          cols="3"
        >
          <v-img
            height="100%"
          >
            <v-row
              align="end"
              class="fill-height"
            >
              <v-col
                align-self="start"
                class="pa-0"
                cols="12"
              >
                <v-avatar
                  class="profile"
                  color="grey"
                  size="164"
                  tile
                >
                  <v-img
                    src="https://veryimportantlot.com/uploads/over/files/%D0%9D%D0%BE%D0%B2%D0%BE%D1%81%D1%82%D0%B8/2020/%D0%9C%D0%B0%D1%80%D1%82%202020/%D0%9C%D0%B0%D1%80%D1%82%20%D0%A1%D1%82%D0%B0%D1%82%D1%8C%D1%8F%20%D0%B4%D0%BB%D1%8F%20%D0%B1%D0%BB%D0%BE%D0%B3%D0%B0.%20%D0%96%D0%B8%D0%B2%D0%BE%D0%BF%D0%B8%D1%81%D1%8C%2063%20(6.1)%20%D0%9F%D0%BE%D1%80%D1%82%D1%80%D0%B5%D1%82.%20%D0%98%D0%BB%D1%8C%D1%8F%20%D0%A0%D0%B5%D0%BF%D0%B8%D0%BD.%20%C2%AB%D0%9F%D0%BE%D1%80%D1%82%D1%80%D0%B5%D1%82%20%D0%BA%D0%BE%D0%BC%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B0%20%D0%9C%D0%BE%D0%B4%D0%B5%D1%81%D1%82%D0%B0%20%D0%9F%D0%B5%D1%82%D1%80%D0%BE%D0%B2%D0%B8%D1%87%D0%B0%20%D0%9C%D1%83%D1%81%D0%BE%D1%80%D0%B3%D1%81%D0%BA%D0%BE%D0%B3%D0%BE%C2%BB.jpg"
                  />
                </v-avatar>
              </v-col>
            </v-row>
          </v-img>
        </v-col>
        <v-col cols="4">
          <div>
            <h1>
              New user
            </h1>
            <div>
              <v-btn
                class="btn_skill"
                elevation="3"
                outlined
                x-small
              >
                Admin
              </v-btn>

              <v-btn
                class="btn_skill"
                elevation="3"
                outlined
                x-small
              >
                Speaker
              </v-btn>

              <v-btn
                class="btn_skill"
                elevation="3"
                outlined
                x-small
              >
                AMA
              </v-btn>
            </div>
            <br>
            <div>
              Cheerful resident in this wonderful world.
            </div>
            <div>
              Minsk, Belarus
            </div>
          </div>
          <div
            class="block"
          >
            <div class="block_follower">
              <h4>440</h4>
              <p>followers</p>
            </div>
            <div class="block_follower">
              <h4>31</h4>
              <p>following</p>
            </div>
            <div
              class="block_follow"
            >
              <h2>+ Follow</h2>
            </div>
          </div>
        </v-col>
        <v-col cols="4">
          <div class="text-center">
            <v-btn
              class="btn_social"
              color="secondary"
              elevation="3"
              icon
              x-small
              outlined
            >
              1
            </v-btn>

            <v-btn
              color="secondary"
              class="btn_social"
              elevation="3"
              icon
              x-small
              outlined
            >
              1
            </v-btn>

            <v-btn
              color="secondary"
              class="btn_social"
              elevation="3"
              icon
              x-small
              outlined
            >
              1
            </v-btn>

            <v-btn
              color="secondary"
              class="btn_social"
              elevation="3"
              icon
              x-small
              outlined
            >
              1
            </v-btn>

            <v-btn
              color="secondary"
              class="btn_social"
              elevation="3"
              icon
              x-small
              outlined
            >
              1
            </v-btn>
          </div>
          <div>
            <v-btn
              elevation="2"
              text
              tile
              outlined
              x-small
            >
              send message
            </v-btn>
          </div>
        </v-col>
      </v-row>
    </div>
    <v-divider class="separator"/>
    <v-row class="blocks">
      <v-col cols="3">
        <h4>My Core Skills:</h4>
      </v-col>
      <v-col cols="3">
        <button class="rating">
          inbound marketing
          <v-rating
            readonly
            hover
            dense
            length="3"
            size="15"
            value="3"
          />
        </button>
      </v-col>
      <v-col cols="3">
        <button class="rating">
          cool marketing
          <v-rating
            readonly
            hover
            dense
            length="2"
            size="15"
            value="2"
          />
        </button>
      </v-col>
      <v-col cols="3">
        <button class="rating">
          growth marketing
          <v-rating
            readonly
            hover
            dense
            length="1"
            size="15"
            value="1"
          />
        </button>
      </v-col>
    </v-row>
    <v-row class="blocks">
      <v-col cols="8">
        <div>
          <span>Professional Bio</span>
          <span>10 years of experience</span>
          <div>Lorem Ipsum is simply dummy text of the printing and typesetting industry.</div>
          <br>
          <div>
            Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer
            took a galley of type and scrambled it to make a type specimen book.
          </div>
          <br>
          <div>
            It is a long established fact that a reader will be distracted by the readable content of a page when
            looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of
            letters, as opposed to using 'Content here, content here', making it look like readable English. Many
            desktop publishing packages and web page editors now use Lorem Ipsum as their default model text, and a
            search for 'lorem ipsum' will uncover many web sites still in their infancy. Various versions have evolved
            over the years, sometimes by accident, sometimes on purpose (injected humour and the like).
          </div>
        </div>
      </v-col>
      <v-col cols="2">
        where i write
        <ul>
          <li>online.by</li>
          <li>tut.by</li>
          <li>relax.by</li>
          <li>takeout.by</li>
        </ul>
      </v-col>
      <v-col cols="2">
        <br>
        <ul>
          <li>random text</li>
          <li>random text</li>
          <li>random text</li>
          <li>random text</li>
        </ul>
      </v-col>
    </v-row>
  </div>
</template>

<script>
export default {
  name: 'Index'
}
</script>

<style lang="scss" scoped>
.blocks_test {
  width: 100%;
  background-color: #e8f6fa;
  padding-bottom: 24px;
  padding-top: 28px;
}

.blocks {
  width: 85%;
  justify-content: center;
  align-items: center;
  margin-left: auto;
  margin-right: auto;
  margin-top: 20px;
}

.block {
  display: flex;
  position: absolute;
  background-color: white;

  .block_follower {
    width: 165px;
    height: 50px;
    border: 1px solid #e0e0e0;
    text-align: center;
    padding-top: 5px;
  }

  .block_follow {
    width: 330px;
    height: 50px;
    border: 1px solid #e0e0e0;
    text-align: center;
    padding-top: 10px;
    background-color: #3aabf5;
    color: white;
  }
}

.rating {
  display: flex;
  padding: 3px;
  cursor: pointer;
  user-select: none;
  border: none;
  outline: none;
  transition: background 5s;
  border-radius: 3px;
}

.rating:active {
  background: #ff0000;
  transition: background 0s;
  border-radius: 3px;
}

.btn_skill {
  border: 1px orange solid;
}

.btn_social {
  background-color: #fdfd86;
  margin-bottom: 35px;
}

li {
  list-style-type: none;
}

</style>
