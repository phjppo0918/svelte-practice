<!-- src/Signup.svelte -->
<script>
    let username = '';
    let email = '';
    let password = '';

    function handleSignup() {
        // 여기에서 회원가입 로직을 처리할 수 있습니다.
        console.log('회원가입 시도:', username, email, password);
    }
</script>

<h1>회원가입</h1>

<form on:submit={handleSignup}>
    <label for="username">사용자 이름:</label>
    <input type="text" id="username" bind:value={username} />

    <label for="email">이메일:</label>
    <input type="email" id="email" bind:value={email} />

    <label for="password">비밀번호:</label>
    <input type="password" id="password" bind:value={password} />

    <button type="submit">회원가입</button>
</form>
