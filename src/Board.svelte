<!-- src/Board.svelte -->
<script>
   let posts = [
       { id: 1, title: '첫 번째 게시물', content: '내용입니다.' },
       { id: 2, title: '두 번째 게시물', content: '내용입니다.' },
       // 추가 게시물...
   ];
</script>

<h1>게시판</h1>

<ul>
    {#each posts as post (post.id)}
        <li>{post.title}</li>
    {/each}
</ul>
