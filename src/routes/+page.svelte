<script>
    let number = 5;
</script>

<form action="/submit.html"
    on:change={()=>console.log("form changed")}
    on:update={()=>console.log("form updated")}
    on:paste={()=>console.log("form pasted")}
    on:input={()=>console.log("form inputed")}
    method="post">
    Value is {number}.<br>
    <input type="number"
        on:update={()=>console.log("updated")}
        on:paste={()=>console.log("pasted")}
        bind:value="{number}"
        on:change={()=>console.log("changed")}
        on:input={()=>console.log("inputed")}
        class="form-control" id="some_input"><br>
    <button type="submit">Submit</button>
</form>