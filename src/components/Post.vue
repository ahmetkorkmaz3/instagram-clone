<template>
  <div class="post">
    <!-- header -->
    <header class="header section">
      <div class="header-author">
        <Avatar :size="40" />
        <div class="header-author-info">
          <div>
            <CustomText tag="b">ahmetkorkmaz3</CustomText>
          </div>
          <div>
            <CustomText size="x-small">Istanbul, Turkey</CustomText>
          </div>
        </div>
      </div>
      <div class="header-more">
        <button type="button">
          <IconMore />
        </button>
      </div>
    </header>

    <!-- media -->
    <div class="post-media">
      <img
        src="https://instagram.fist4-1.fna.fbcdn.net/v/t51.2885-15/e35/p1080x1080/144182879_1534474853402768_4114809594159491067_n.jpg?_nc_ht=instagram.fist4-1.fna.fbcdn.net&_nc_cat=1&_nc_ohc=Ncz-tYFx2roAX9LkBgn&tp=1&oh=c61a15c2f5c55994eca9fd84d626c944&oe=604488DB"
        alt=""
      />
    </div>

    <!-- actions -->
    <div class="action-buttons section">
      <button type="button">
        <IconLike />
      </button>
      <button type="button">
        <IconComment />
      </button>
      <button type="button">
        <IconDirect />
      </button>
      <button type="button" class="action-save">
        <IconSave />
      </button>
    </div>

    <!-- view count -->
    <div class="view-count section">
      <CustomText tag="b">1.345 likes</CustomText>
    </div>
    <!-- comments list -->
    <!-- datetime -->
    <!-- comment form -->
  </div>
</template>

<script>
import Avatar from '@/components/Avatar'
import CustomText from '@/components/CustomText'
import IconMore from '@/icons/more.svg'
import IconLike from '@/icons/like.svg'
import IconComment from '@/icons/comment.svg'
import IconDirect from '@/icons/direct.svg'
import IconSave from '@/icons/save.svg'

export default {
  name: 'Post',
  components: {
    CustomText,
    Avatar,
    IconMore,
    IconLike,
    IconComment,
    IconDirect,
    IconSave
  }
}
</script>

<style scoped>
.post {
  border: 1px solid rgb(var(--b6a));
  border-radius: 3px;
}

.section {
  padding-left: 16px;
  padding-right: 16px;
}

.header {
  height: 60px;
  display: flex;
  align-items: center;

  &-author {
    display: flex;
    align-items: center;

    &-info {
      margin-left: 8px;
    }
  }

  &-more {
    margin-left: auto;
  }
}

.action-buttons {
  padding-left: 16px;
  padding-right: 16px;
  height: 45px;
  display: flex;
  align-items: center;

  button {
    margin-right: 16px;
  }

  button.action-save {
    margin-left: auto;
    margin-right: 0;
  }
}
</style>
