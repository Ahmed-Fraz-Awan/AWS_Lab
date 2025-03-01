# AWS_Lab
<button onclick="fetchData()">Get Message</button>
<p id="message"></p>
<script>
    async function fetchData() {
        const response = await fetch('YOUR_API_GATEWAY_URL');
        const data = await response.json();
        document.getElementById('message').textContent = data.message;
    }
</script>
