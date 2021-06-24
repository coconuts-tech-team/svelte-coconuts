<script>
  import axios from "axios";
  import Parser from "fast-xml-parser";
  import Card from "./Card.svelte";

  console.log("cards start");
  const getRssFeeds = async () => {
    const rssJson = await axios
      .get("https://anchor.fm/s/4881bfd0/podcast/rss")
      .then((res) => Parser.parse(res.data))
      .catch((err) => console.error(err));
    return rssJson.rss.channel.item;
  };
  const feedPromise = getRssFeeds();
</script>

{#await feedPromise}
  fetching feeds...
{:then feeds}
  {#each feeds as feed}
    <Card title={feed.title} summary={feed.description} />
  {/each}
{/await}
