<script>
import Navbar from "../components/Navbar/navbar.svelte";

</script>

<main>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta2/css/all.min.css">

    <body>
        <Navbar />
        <!--Alert Messages Start
            <div class="alert-success">
                <span>Message Sent! Thank you for contacting us.</span>
            </div>
            <div class="alert-error">
                <span>Something went wrong! Please try again.</span>
            </div>
        Alert Messages End-->
        
            <!--Contact Section Start-->
            <div class="contact-section">
                <div class="contact-info">
                    <div><i class="fa-solid fa-location-dot"></i>Adress,City,Country</div>
                    <div><i class="fa-solid fa-envelope"></i>contact@gmail.com</div>
                    <div><i class="fa-solid fa-phone"></i>+00 000 000 00 00</div>
                    <div><i class="fa-solid fa-clock"></i>7/24</div>
                </div>
                <div class="contact-form">
                    <h2>Contact Us</h2>
                    <form class="contact" action="" method="post"></form>
                    <input type="text" name="name" class="text-box" placeholder="Your Name" required>
                    <input type="email" name="email" class="text-box" placeholder="Your E-mail" required>
                    <textarea name="message" rows="5" placeholder="Your Message"></textarea>
                    <input type="submit" name="submit" class="send-button" value="Send">
                </div>
            </div>
        </body>
</main>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Ubuntu:wght@400;500;700&display=swap');


*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Ubuntu" ,sans-serif;
}

body{
    min-height: 100vh;
    background-image: url("../assets/Müşteri Hizmetleri Background.jpg") ;
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    justify-content: center;
    align-items: center;
}

.contact-section{
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
}

.contact-info{
    color: #fff;
    max-width: 500px;
    line-height: 65px;
    padding-left: 50px;
    font-size: 18px;
}

.contact-info i{
    margin-right: 20px;
    font-size: 25px;
}

.contact-form{
    max-width: 700px;
    margin-right: 50px;
}

.contact-info , .contact-form{
    flex: 1;
}

.contact-form h2{
    color: #fff;
    text-align: center;
    font-size: 35px;
    text-transform: uppercase;
    margin-bottom: 30px;
}

.contact-form .text-box{
    background:#000;
    color: #fff;
    border: none;
    width: calc(50% - 10px);
    height: 50px;
    padding: 12px;
    font-size: 15px;
    border-radius: 10px;
    box-shadow: 0 1px 1px rgba(0, 0, 0, 0.1);
    margin-bottom: 20px;
    opacity: 0.9;
}

.contact-form .text-box:last-child{
    margin-left: 15px;
}

.contact-form textarea{
    background:#000;
    color: #fff;
    border: none;
    width: 100%;
    padding: 12px;
    font-size: 15px;
    min-height: 200px;
    max-height: 400px;
    resize: vertical;
    border-radius: 10px;
    box-shadow: 0 1px 1px rgba(0, 0, 0, 0.1);
    margin-bottom: 20px;
    opacity: 0.9;
}

.contact-form .send-button{
    float: right;
    background: #2e94e3;
    color: #fff;
    border: none;
    width: 120px;
    height: 40px;
    font-size: 15px;
    font-weight: 700;
    text-transform: uppercase;
    letter-spacing: 2px;
    border-radius: 10px;
    cursor: pointer;
    transition: 0.3s;
    transition-property: background;
}

.contact-form .send-button:hover{
    background: #0582e3;
}

@media screen and (max-width:950px){
    .contact-section{
        flex-direction: column;
    }

    .contact-info, .contact-form{
        margin: 30px 50px;
    }

    .contact-form h2{
        font-size: 30px;
    }

    .contact-form .text-box{
        width: 100%;
    }
}

/*Css for Alert Messages*/

.alert-success{
    z-index: 1;
    background: #D4EDDA;
    font-size: 18px;
    padding: 20px 40px;
    min-width: 420px;
    position: fixed;
    right: 0;
    top: 10px;
    border-left: 8px solid #3ad66e;
    border-radius: 5px;
}

.alert-error{
    z-index: 1;
    background: #fff3cd;
    font-size: 18px;
    padding: 20px 40px;
    min-width: 420px;
    position: fixed;
    right: 0;
    top: 10px;
    border-left: 8px solid #ffa502;
    border-radius: 5px;
}

</style>