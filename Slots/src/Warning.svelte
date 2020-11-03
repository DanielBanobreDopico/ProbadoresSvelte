<script></script>

<div>
    <img alt='alert' src='./imgs/alert.svg'>
    <slot>Pon aquí tu advertencia</slot>
</div>

<style>
    div > img {
        height: 1em;
        float: left;
        margin-right: 1em;
    }
    div {
        background-color: yellow;
        border-style: dashed;
        border-color: black;
        border-width: 0.5em;
        padding: 1em;
        margin: 5em 10em;
    }
    * {
        font-size: 2em;
    }
</style>