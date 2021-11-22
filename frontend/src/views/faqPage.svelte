<script>
import Navbar from "../components/Navbar/navbar.svelte";

</script>

<main>
    <link href="https://unpkg.com/ionicons@4.5.10-0/dist/css/ionicons.min.css" rel="stylesheet">
    <Navbar />

    <body>
        <section>
            <div class="container">
                <div class="accordion">
                    <div class="accordion-item"  id="question1">
                        <a class="accordion-link" href="#question1">
                            How often do you go to beach?
                            <i class="icon ion-md-add"></i>
                            <i class="icon ion-md-remove"></i>
                        </a>
                        <div class="answer">
                            <p>
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum asperiores nisi aliquam magnam modi perspiciatis, dolorum illo eveniet! Quasi qui temporibus aperiam unde laudantium atque libero recusandae sequi dolorum voluptate!
                            </p>
                        </div>
                    </div>
                    <div class="accordion-item"  id="question2">
                        <a class="accordion-link" href="#question2">
                            How often do you go to beach?
                            <i class="icon ion-md-add"></i>
                            <i class="icon ion-md-remove"></i>
                        </a>
                        <div class="answer">
                            <p>                        
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum asperiores nisi aliquam magnam modi perspiciatis, dolorum illo eveniet! Quasi qui temporibus aperiam unde laudantium atque libero recusandae sequi dolorum voluptate!
                             </p>
                        </div>
                    </div>
                    <div class="accordion-item"  id="question3">
                        <a class="accordion-link" href="#question3">
                            How often do you go to beach?
                            <i class="icon ion-md-add"></i>
                            <i class="icon ion-md-remove"></i>
                        </a>
                        <div class="answer">
                            <p>
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum asperiores nisi aliquam magnam modi perspiciatis, dolorum illo eveniet! Quasi qui temporibus aperiam unde laudantium atque libero recusandae sequi dolorum voluptate!
                            </p>
                        </div>
                    </div>
                    <div class="accordion-item"  id="question4">
                        <a class="accordion-link" href="#question4">
                            How often do you go to beach?
                            <i class="icon ion-md-add"></i>
                            <i class="icon ion-md-remove"></i>
                        </a>
                        <div class="answer">
                            <p>
                                Lorem ipsum dolor sit amet consectetur adipisicing elit. Voluptatum asperiores nisi aliquam magnam modi perspiciatis, dolorum illo eveniet! Quasi qui temporibus aperiam unde laudantium atque libero recusandae sequi dolorum voluptate!
                            </p>
                        </div>
                    </div>
                </div>
            </div>
        </section>
    </body>
</main>

<style>
    *,
*::before,
*::after{
    margin: 0;
    padding: 0;
    box-sizing: inherit;
}

html{
    font-family: "Roboto", sans-serif;
    font-size: 10px;
    box-sizing: border-box;
}

section{
    width: 100%;
    height: 100vh;
    background-color: #3c4053;
    display: flex;
    align-items: center;
    justify-content: center;
}

.container{
    width: 100%;
    max-width: 80rem;
    margin: 0 auto;
    padding: 0 1.5rem;
}

.accordion-item{
    background-color: #283042;
    border-radius: 0.6rem;
    margin-bottom: 10px;
    padding: 10px;
    box-shadow: 0.5rem 2px 0.5rem rgba(0,0,0,0.2);
}

.accordion-link{
    font-size: 1.6rem;
    color: gainsboro;
    text-decoration: none;
    background-color: #283042;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 10px 0;
}

.accordion-link i{
    color: #e7d5ff;
    padding: 5px;
}

.accordion-link .ion-md-remove{
    display: none;
}

.answer{
    max-height: 0;
    overflow: hidden;
    position: relative;
    background-color: #212838;
    transition: max-height 1200ms;
}

.answer::before{
    content: "";
    position: absolute;
    width: 0.6rem;
    height: 100%;
    background-color: #8fc460;
    top: 50%;
    left: 0;
    transform: translateY(-50%);
}

.answer p {
    color: gainsboro;
    font-size: 14px;
    padding: 20px;
}

.accordion-item:target .answer{
    max-height: 20rem;
}

.accordion-item:target .accordion-link .ion-md-add{
    display: none;
}

.accordion-item:target .accordion-link .ion-md-remove{
    display: block;
}
</style>