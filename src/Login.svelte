<!-- src/Login.svelte -->
<script>
    let email = '';
    let password = '';

    function handleLogin() {
        // 여기에서 로그인 로직을 처리할 수 있습니다.
        console.log('로그인 시도:', email, password);
    }
</script>

<h1>로그인</h1>

<form on:submit={handleLogin}>
    <label for="email">이메일:</label>
    <input type="email" id="email" bind:value={email} />

    <label for="password">비밀번호:</label>
    <input type="password" id="password" bind:value={password} />

    <button type="submit">로그인</button>
</form>
