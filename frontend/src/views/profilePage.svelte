<script>
import Navbar from "../components/Navbar/navbar.svelte";

</script>

<main>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
    <Navbar />
    <body>
        <div class="container">
            <div class="main">
                <div class="topbar">
                    <a href="">Logout</a>
                    <a href="">Support</a>
                    <a href="">Work</a>
                    <a href="">Home</a>
                </div>
                <div class="row">
                    <div class="col-md-4 mt-1">
                        <div class="card text-center sidebar">
                            <div class="card-body">
                                <div class="mt-3">
                                    <h3>Sergen Berke Altan</h3>
                                    <a href="">Home</a>
                                    <a href="">Work</a>
                                    <a href="">Support</a>
                                    <a href="">Settings</a>
                                    <a href="">Signout</a>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div class="col-md-8 mt-1">
                        <div class="card mb-3 content">
                            <h1 class="m-3 pt-3">About</h1>
                            <div class="card-body">
                                <div class="row">
                                    <div class="col-md-3">
                                        <h5>Full Name</h5>
                                    </div>
                                    <div class="col-md-9 text-secondary">
                                        Sergen Berke Altan
                                    </div>
                                </div>
                                <hr>
                                <div class="row">
                                    <div class="col-md-3">
                                        <h5>E-mail</h5>
                                    </div>
                                    <div class="col-md-9 text-secondary">
                                        sergen.altan190@gmail.com
                                    </div>
                                </div>
                                <hr>
                                <div class="row">
                                    <div class="col-md-3">
                                        <h5>Phone</h5>
                                    </div>
                                    <div class="col-md-9 text-secondary">
                                        53472880842
                                    </div>
                                </div>
                                <div class="row">
                                    <div class="col-md-3">
                                        <h5>Adress</h5>
                                    </div>
                                    <div class="col-md-9 text-secondary">
                                        Çorlu/Tekirdağ
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </body>
</main>

<style>
    body{
    margin-top: 100px;
    background-color: lightgray;
}

.main{
    padding: 15px;
    font-family: Arial, Helvetica, sans-serif;
}

.topbar{
    background-color: teal;
    overflow: hidden;
}

.topbar a{
    float: left;
    color: whitesmoke;
    text-align: center;
    padding: 20px 26px;
    text-decoration: none;
    font-size: 26px;
}

.sidebar{
    background-color: #333;
    color: white;
    height: 100%;
}

.sidebar a{
    margin-left: 10px;
    display: block;
    color: white;
    padding-bottom: 10px;
    font-size: 15px;
    text-decoration: none;
}

.card{
    position: relative;
    display: flex;
    flex-direction: column;
}

.content{
    background-color: whitesmoke;
}
</style>