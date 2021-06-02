<script>
    import logo from './logo.svg';
    import Typewriter from 'svelte-typewriter'
</script>

<div class="logo">
    <a href="/">
        <!-- <img src={logo} alt="Leonela Venturo" /> -->
        <h2>
            <span style="color: #FFB3DD">L</span><span style="color: #C7F3A4">E</span><span style="color: #FFFA9D">O</span><span style="color: #AFE2FF">N</span><span style="color: #D7A2F9">E</span><span style="color: #FFB3DD">L</span><span style="color: #C7F3A4">A</span><span style="color: #FFFA9D">&nbsp;</span><span style="color: #FFB3DD">V</span><span style="color: #C7F3A4">E</span><span style="color: #FFFA9D">N</span><span style="color: #AFE2FF">T</span><span style="color: #D7A2F9">U</span><span style="color: #FFB3DD">R</span><span style="color: #C7F3A4">O</span>
        </h2>
        <!-- <h2>LEONELA VENTURO</h2> -->
        <Typewriter cursor={'white'} interval={160}><h1>Redactora SEO</h1></Typewriter>

    </a>
</div>

<style>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Lato:wght@400&display=swap');
.logo{
    position: absolute;
    top: 10px;
    left: 0;
    right: 0;
    margin: auto;
    height: 80px;
    display: flex;
    justify-content: center;
    overflow: hidden;
}
a{
    text-decoration: none;
    text-align: center;
}
h2{
    /* letter-spacing: 1.3px; */
    margin: 0;
    font-family: "Montserrat";
    font-size: 1.8rem;
	text-transform: uppercase;
	/* background: linear-gradient(to right, #FFB3DD 0%, #C7F3A4 33%, #FFFA9D 66%, #AFE2FF 100%);
	-webkit-background-clip: text;
	-webkit-text-fill-color: transparent; */
}
h1{
    font-family: 'Lato', sans-serif;
    letter-spacing: 1px;
    text-transform: uppercase;
    margin: 5px 0 0 0;
    font-size: 1.1rem;
    color: #fff ;
}
span{
    margin: 0 1.5px 0 0;
}
</style>