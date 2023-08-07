<script lang="ts">
    console.log("ahoj");

    //TS - deklarace urcit datový typ

</script>

<header>
    <nav>
        <ul>
            <li><a href="test1">test1</a></li>
            <li><a href="/">test2</a></li>
            <li><a href="#">test3</a></li>
        </ul>
    </nav>
</header>

<style lang="stylus">

    :global(body)
        margin 0
        padding 0
        
    header
        background-color grey
        margin 0
        padding 0

        
        ul
            margin 0
            padding 15px
            display flex
            list-style-type none
            gap 24px
            justify-content center

            li
                a
                    text-decoration none
                    color white

                    &:hover
                        text-decoration underline

</style>