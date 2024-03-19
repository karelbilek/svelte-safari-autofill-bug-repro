<script>
    let number = 5;
</script>

<form action="/submit.html" method="post">
    Value is {number}.<br>
    <input type="number" bind:value="{number}" class="form-control" id="some_input"><br>
    <button type="submit">Submit</button>
</form>