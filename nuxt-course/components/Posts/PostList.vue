<template>
    <div class="posts-list">
        <section class="post-list">
            <PostPreview
                id="1"
                :is-admin="isAdmin"
                thumbnail="https://www.thomsonreuters.com/content/dam/ewp-m/images/image-library/en/photography/201138-118072186.jpeg"
                title="Hello there!"
                previewText="This is my first post!"
            />
            <PostPreview
                id="2"
                :is-admin="isAdmin"
                thumbnail="https://www.thomsonreuters.com/content/dam/ewp-m/images/image-library/en/photography/201138-118072186.jpeg"
                title="Hello there!"
                previewText="This is my second post!"
            />
            <PostPreview
                id="3"
                :is-admin="isAdmin"
                thumbnail="https://www.thomsonreuters.com/content/dam/ewp-m/images/image-library/en/photography/201138-118072186.jpeg"
                title="Hello there!"
                previewText="This is my third post!"
            />
        </section>
    </div>
</template>

<script>
import PostPreview from "@/components/Posts/PostPreview.vue";

export default {
    components: {
        PostPreview
    },
    props: {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
};
</script>

<style scoped>
.post-list {
    display: flex;
    padding: 20px;
    box-sizing: border-box;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}
</style>
