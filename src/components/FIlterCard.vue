<template>
  <div class="min-height">
    <div class="chat-template">
      <div class="container res">
        <div class="row">
          <div class="col-sm-4">
            <div class="row">
              <div class="sidebar">
                <div class="chat-scroller">
                  <ul class="lister">
                    <ListingTemplate
                      @click="selectChat(i)"
                      v-for="(chat, i) in chats"
                      :key="i"
                      :chat="chat"
                    />
                  </ul>
                </div>
              </div>
            </div>
          </div>
          <div class="col-sm-8">
            <div class="row">
              <div class="chat-section">
                <Topbar :chat="selectedChat" />
                <input
                  type="text"
                  class="form-control searchbox"
                  v-model="search"
                  placeholder="Search"
                />
                <MessagesTemplate :chat="filteredChat" />
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Topbar from "./templates/Topbar";
import MessagesTemplate from "./templates/MessagesTemplate";
import ListingTemplate from "./templates/ListingTemplate";

export default {
  data() {
    return {
      selectedChat: {
        value: {
          to: []
        }
      },
      search: "",
      chats: [
        {
          date: "2019-12-11",
          value: {
            from: "a",
            email: "pushan@test.in",
            to: [
              {
                user: "b",
                msg: "Hi 11",
                time: "10:12:21"
              },
              {
                user: "c",
                msg: "Hello 11",
                time: "10:12:21"
              },
              {
                user: "d",
                msg: "Bye 11",
                time: "10:11:21"
              }
            ]
          }
        },
        {
          date: "2019-12-12",
          value: {
            from: "a",
            email: "pushan@test.in",
            to: [
              {
                user: "b",
                msg: "Hi 12",
                time: "10:12:21"
              },
              {
                user: "c",
                msg: "Hello 12",
                time: "10:11:21"
              },
              {
                user: "d",
                msg: "Bye 12",
                time: "10:16:21"
              }
            ]
          }
        },
        {
          date: "2019-12-11",
          value: {
            from: "a",
            email: "pushan@test.in",
            to: [
              {
                user: "b",
                msg: "Hi 11.1",
                time: "12:11:21"
              },
              {
                user: "c",
                msg: "Hello 11.1",
                time: "10:12:21"
              },
              {
                user: "d",
                msg: "Bye 11.1",
                time: "15:12:21"
              }
            ]
          }
        },
        {
          date: "2019-12-13",
          value: {
            from: "a",
            email: "pushan@test.in",
            to: [
              {
                user: "b",
                msg: "Hi 13",
                time: "15:12:21"
              },
              {
                user: "c",
                msg: "Hello 13",
                time: "13:12:21"
              },
              {
                user: "d",
                msg: "Bye 13",
                time: "09:12:21"
              }
            ]
          }
        },
        {
          date: "2019-12-10",
          value: {
            from: "a",
            email: "pushan@test.in",
            to: [
              {
                user: "b",
                msg: "Hi 10",
                time: "16:12:21"
              },
              {
                user: "c",
                msg: "Hello 10",
                time: "13:12:21"
              },
              {
                user: "d",
                msg: "Bye 10",
                time: "10:12:21"
              }
            ]
          }
        }
      ]
    };
  },
  computed: {
    filteredChat() {
      let _this = this;
      return this.selectedChat.value.to.filter(post => {
        return post.msg
          .toLowerCase()
          .includes((_this.search && _this.search.toLowerCase()) || "");
      });
    }
  },
  mounted() {
    this.getMessages();
  },
  methods: {
    getMessages() {
      this.chats.sort(function(a, b) {
        return new Date(b.date) - new Date(a.date);
      });
      this.selectChat(0);
    },
    selectChat(index) {
      this.search = "";
      this.selectedChat = this.chats[index];
      this.selectedChat.value.to.sort(function(a, b) {
        if (a.time < b.time) return -1;

        if (a.time > b.time) return 1;

        return 0;
      });
    }
  },
  components: {
    Topbar,
    MessagesTemplate,
    ListingTemplate
  }
};
</script>
