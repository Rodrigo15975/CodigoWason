# CodigoWason
Codigo


@import url('https://fonts.googleapis.com/css2?family=Condiment&family=Corinthia:wght@400;700&family=Jacques+Francois&family=Jacques+Francois+Shadow&family=Jost&family=Kumbh+Sans:wght@300;400;500;600&family=Merienda+One&family=Merienda:wght@400;700&family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;0,800;1,300;1,400;1,500;1,600;1,700;1,800&family=Roboto&family=Uchen&display=swap');


:root{
    --Font-Text-KUMB: 'Kumbh Sans', sans-serif;
    --FonMerienda: 'Merienda', cursive;
    --FontMeriendaOne: 'Merienda One', cursive; 
    --FontCorinthia: 'Corinthia', cursive;
    --FontJaques1: 'Jacques Francois', serif;
    --FontJaques2: 'Jacques Francois Shadow';
    --fontJost: 'Jost',sans-serif;
    --FontOpenSans: 'Open Sans', sans-serif;
    --FontRoboto: 'Roboto',sans-serif;
    --FontUchen: 'Uchen', serif;     
    --FontCondiment: 'Condiment',cursive;

    --step--2: clamp(0.91rem, calc(0.75rem + 0.83vw), 0.96rem);
    --step--1: clamp(1.09rem, calc(0.73rem + 1.81vw), 1.20rem);
    --step-0: clamp(1.31rem, calc(0.67rem + 3.19vw), 1.50rem);
    --step-1: clamp(1.58rem, calc(0.55rem + 5.11vw), 1.88rem);
    --step-2: clamp(1.89rem, calc(0.35rem + 7.72vw), 2.34rem);
    --step-3: clamp(2.27rem, calc(0.01rem + 11.27vw), 2.93rem);
    --step-4: clamp(2.72rem, calc(-0.48rem + 16.00vw), 3.66rem);
    --step-5: clamp(3.27rem, calc(-1.20rem + 22.33vw), 4.58rem);
    --step-6: clamp(3.92rem, calc(-2.22rem + 30.68vw), 5.72rem);
    --step-7: clamp(4.70rem, calc(-3.64rem + 41.69vw), 7.15rem);
    --step-8: clamp(5.64rem, calc(-5.58rem + 56.12vw), 8.94rem);
    --step-9: clamp(6.77rem, calc(-8.22rem + 74.95vw), 11.18rem);
    --step-10: clamp(8.13rem, calc(-11.76rem + 99.46vw), 13.97rem);

    scroll-behavior: smooth;
}
/*Header*/
.header{
    margin: auto;
    max-width: 120em;    
    background-color: black;
    position: relative;
    z-index: 995;
    display: flex;
    flex-direction: column;
    
    //Border white
    .cont-border-header{       
        position: absolute;      
        z-index: 994; 
        width: 100%;
        height: 100%;
        padding: 1em;
        .border-header{
            width: 100%;
            height: 100%;
            border: 0.2em solid rgb(255, 255, 255);
            border-radius: 0.5em;
        }
    }
    //Contenedor de title, y btns
    .conteiner-header-principal{
       position: absolute;
       top: 0;
       bottom: 0;
       left: 0;
       right: 0;
       display: flex;
       flex-direction: column;
       justify-content: space-evenly;
       z-index: 996;
       //title
       .cont-title-header{
            flex: 0 1 40%;
            display: flex;
            justify-content: center;
            align-items: center;     

            img{               
               width: 60%;
            }
       }
       //texto y btn
       .cont-text-btn-header{
            flex: 0 1 50%;
            display: flex;
            flex-direction: column;
            justify-content: space-evenly;
            align-content: center;
            align-items: center;
            .cont-button-header {
                    display: flex;       
                    a{
                        display: flex;
                        align-items: center;
                        height: 65%;
                        img{
                            height: 100%;
                        }
                    }         
            }
       }
    }

    //Navegación mobile
    .nav-mobile{       
        
        .cont-nav-mobile{   
            transform: translateY(-150em);
            position: fixed;
            z-index: 998;
            top: 0;
            bottom: 0;
            left: 0;
            right: 0;

            transition: transform 0.3s linear;
            background-color: rgba(0, 0, 0, 0.493);
            display: flex;
            flex-direction: column;
            justify-content: space-evenly;
            align-items: center;         
            font-size: var(--FontJaques2);   
            .link-nav-mobile{
                font-family: var(--FontOpenSans);
                font-weight: 700;
                color: rgb(255, 255, 255);
                width: 100%;
                height: 100%;
                display: flex;
                justify-content: center;
                align-items: center;                
                background-color: rgb(255, 255, 255);
                
                .icon-mobile{
                    padding-right: 0.2em;
                    padding-bottom: 0.2em;
                    padding-top: 0.2em;
                }
            }
            .red{
                background-color: rgb(224, 38, 69);
            }
            .white{
                background-color: white;
                color: rgb(0, 0, 0);
            }
                        // .link-nav-mobile:hover {
                        //     background-color: rgba(0, 0, 0, 0.514);
                        //     color: white;                          
                        // }
            .border-bottom-mobile{
                
                border-bottom: 0.1em solid rgb(0, 0, 0);
            }
           
        }   
        .MostrarMenuJs {
                transform: translateY(0);        
               
    }
    
}
    //Icono del burger
    .icon-burger-mobile{
        position: fixed;
        z-index: 999;
        width: 2.5em;
        height: 2.5em;
        top: 2em;
        right: 2em;
        background-color: rgb(255, 255, 255);
        border-radius: 0.5em;
        cursor: pointer;
    }

}
.cortina-relative-button{
    position: relative;
}
.cortina-relative-button::before{
    position: absolute;
    content: "";
    width: 75%;
    height: 100%;
    left: 0;
    top: 0;
    right: 0;
    bottom: 0;
    margin: auto;
    background-color: rgb(255, 255, 255);
    opacity: 0.4;
    border-radius: 0.5em;
    transition: width 0.3s linear , background-color 0.3s linear, transform 0.3s linear;
}

.cortina-relative-button:hover::before {
    position: absolute;
    content: "";
    width: 0%;      
}

//Desapareciendo img del desktop
.img-desktop{
    display: none;

}
 
.slide-in-blurred-top {
    -webkit-animation: slide-in-blurred-top .6s cubic-bezier(.23, 1.000, .32, 1.000) both;
    animation: slide-in-blurred-top .6s cubic-bezier(.23, 1.000, .32, 1.000) both
}

@-webkit-keyframes slide-in-blurred-top {
    0% {
        -webkit-transform: translateY(-1000px) scaleY(2.5) scaleX(.2);
        transform: translateY(-1000px) scaleY(2.5) scaleX(.2);
        -webkit-transform-origin: 50% 0;
        transform-origin: 50% 0;
        -webkit-filter: blur(40px);
        filter: blur(40px);
        opacity: 0
    }

    100% {
        -webkit-transform: translateY(0) scaleY(1) scaleX(1);
        transform: translateY(0) scaleY(1) scaleX(1);
        -webkit-transform-origin: 50% 50%;
        transform-origin: 50% 50%;
        -webkit-filter: blur(0);
        filter: blur(0);
        opacity: 1
    }
}

@keyframes slide-in-blurred-top {
    0% {
        -webkit-transform: translateY(-1000px) scaleY(2.5) scaleX(.2);
        transform: translateY(-1000px) scaleY(2.5) scaleX(.2);
        -webkit-transform-origin: 50% 0;
        transform-origin: 50% 0;
        -webkit-filter: blur(40px);
        filter: blur(40px);
        opacity: 0
    }

    100% {
        -webkit-transform: translateY(0) scaleY(1) scaleX(1);
        transform: translateY(0) scaleY(1) scaleX(1);
        -webkit-transform-origin: 50% 50%;
        transform-origin: 50% 50%;
        -webkit-filter: blur(0);
        filter: blur(0);
        opacity: 1
    }
}

//Whassap icon
.fixed-whassap{
    position: fixed;
    width: 3em;
    height: 3em;
    bottom: 0.8em;
    right: 0.8em;
    padding: 0.4em;
    border-radius: 0.8em;
    transition: background-color 0.3s linear, transform 0.3s ease-in;
    background-color: rgb(107, 255, 139);
 
}
.fixed-whassap:hover{
    background-color: rgb(202, 255, 219);
    
}
//FACEBOOK ICON
.fixed-facebook {
   
    width: 3em;
    height: 3em;
    position: fixed;
    bottom: 4.5em;
    right: 0.8em;
    border-radius: 0.8em;
    transition: background-color 0.3s linear;
}
.img-fb-fixed{
    transition: transform 0.3s ease-in;
}
.img-fb-fixed:hover, .fixed-whassap:hover{
    transform: scale(1.2);
    
}

/*-----------------------------*/

//Titulo barber wason

.article-barber-wason{
    display: flex;   
    .conteiner-barber-wason{
        
        .cont-title-barber-wason{
            font-family: var(--FonMerienda);        
        }


    }
}

//----------

/*--------------*/
@media (max-width: 819px) {
    .cont-txt-header {
        width: 50%;
        display: inherit;
        justify-content: center;

        img {
            width: 100%;
        }
    }

    .cont-button-header {
        .button-no-mobile {
            display: none;
        }
    }

    .cont-nav-desktop {
        display: none;
    }

    .img-txt-barbero {
        width: 100%;
        height: 10em;
        display: flex;
        align-items: flex-end;
        margin-bottom: 1em;

        img {
            width: 100%;
        }
    }

    .cont-button-mobile-1 {
        width: 100%;
        height: 4.4rem;
        display: flex;
        justify-content: center;
        
    }    
    .article-barber-wason{    
        padding: 1em 0 1em 0;
        justify-content: center;
        position: relative;
      .conteiner-barber-wason{   
        display: flex;
        flex-direction: column;
        align-content: center;
        align-items: center;
        gap: 2em;
        background-color: rgb(255, 255, 255);
        border: 0.3em solid rgb(0, 0, 0);
        padding: 0.8em 0 0.8em 0;
        border-radius: 0.8em;
        width: 95%;

        .cont-title-barber-wason {
            width: 95%;
            border-radius: 0.5em;
            text-align: center;
            padding: 0.5em;
            background-color: rgba(0, 0, 0, 0.856);
    
            .title-wason {
                font-size: var(--step-2);
                color: hsl(0, 0%, 100%);
                font-weight: 100;
            }
        }
        .cont-text-barber{
            text-align: center;
            font-family: var(--Font-Text-KUMB);
            font-weight: 100;
            font-size: 1.3em;
            color: rgba(0, 0, 0, 0.822);
            padding: 0.5em;
            .text-barber{
                padding: 0.3em;
                text-shadow: 0 0 1.5px rgb(0, 0, 0);
            }
        }   
        .cont-img-barber{           
            padding: 0.5em;
            .img-barber{
                border-radius: 0.8em;
            }
        }
      }
        
    }
    .article-barber-wason::after{
        position: absolute;
        content: "Quitar cortina";
        font-family: var(--FonMerienda);
        display: flex;
        font-weight: 100;
        align-items: center;
        justify-content: center;
        color: white;
        width: 95%;
        border-radius: 0.8em;
        height: 96%;
        opacity: 0.5;
        transition: opacity 0.53s ease-in-out; ;
        background-color: black;
        
        animation: movete 2s linear  infinite alternate both;
    }

    .article-barber-wason:hover::after{
        opacity: 0;
    }

    @keyframes movete {
        0%{
            transform: translateY(-3px);
        }
    }

    //Section-heider-gilder
    // .section-info-barbers {
    //     display: grid;
    //     grid-template-columns: repeat(auto-fit, minmax(min-content, 350px));
    //     justify-content: space-evenly;
    //     justify-items: center;
    //     gap: 1em;
    //     padding: 1em 0 1em 0 ;
    //     background-color: rgb(255, 255, 255);
        
    //     .cont-barbers {
    //         display: flex;
    //         flex-direction: column;
    //         justify-content: center;
    //         align-items: center;
    //         border: 0.2em solid rgb(0, 0, 0);
    //         box-shadow: -5px -1px 1px rgba(0, 0, 0, 0.384);
    //         border-radius: 0.5em;
    //         transition: box-shadow 0.3s linear;
    //         .border-bottom-barbers{
    //             border-bottom: 0.1em solid black;
    //         }
    //     }
    //     .cont-barbers:hover{
    //         box-shadow: none;
    //     }
    // }
    //---------------

    .section-horario-wason{
        max-width: 120em;
        min-height: 90vh;
        background-image: url(Fotos/Cabezera2.svg);
        background-position: center;
        background-size: cover;
        background-attachment: fixed;
        display: grid;
        justify-content: center;
        //Una sola clase dado flex a los horarios-contenedores
        .cont-horarios{
            width: 100%;
            display: flex;      
            justify-content: center;     
                font-family: var(--FontMeriendaOne);
        }
        .cont-title-horario{
            justify-content: center;
            text-align: center;
           
          .title-horario{       
           color: rgb(255, 255, 255);
           font-weight: bold;
           font-size: var(--step-1);
            text-shadow: 0 0 3px ;
            padding: 0.5em 0 0 0;
            
           
          }
        }
        .cont-lunes-sabado{
            padding-bottom: 1em;       
            .lunes-sabado{
                width: 100%;
                height: 60%;
                background-color: rgba(0, 0, 0, 0.733);
           
                border-radius: 0.5em;             
                display: flex;
                flex-direction: column;
                justify-content: center;
                align-items: center;
                align-content: center;
                text-align: center;
                gap: 1em;
                .text-lunes-sabado{
                    font-size: var(--step-2);
                    color: rgb(255, 255, 255);                
                    text-shadow: 0 0 3px;
                }
                .text-horario-ls{
                    color: rgb(255, 153, 153);
                    text-shadow: 0 0 3px white;
                    font-size: 1.2em;
                }
                
            }
        }
        .domingo{
            width: 100%;
            padding: 0.4em;
            height: 60%;
            display: flex;
            flex-direction: column;
            background-color: rgba(0, 0, 0, 0.733);
                   
            border-radius: 0.5em;
            justify-content: center;
            align-items: center;
            gap: 1em;
                .text-domingo{
                    font-size: var(--step-2);
                    color: white;
                    text-shadow: 0 0 3px;
                }
                .text-horario-domingo{
                color: rgb(255, 153, 153);
                    text-shadow: 0 0 3px white;
                    font-size: 1.2em;
                }
        }
    }

    
}


@media (max-width: 428px) {
    .cont-txt-header {
        width: 80%;
    }

    .cont-text-btn-header {
        display: none;
    }

    .button-mobile {
        width: 100%
    }
    

}



@media (min-width: 51.25em) {
    .img-header-mobile {
        display: none;
        height: 820px;
    }

    .img-desktop {
        display: block;
    }

    //Navegacion pc
    .cont-nav-desktop {       
        background-color: rgba(0, 0, 0, 0.301);
        display: flex;
        flex-direction: column;
        align-items: center;
        align-content: center;
        gap: 2em;
        padding-top: 2em;
        padding-bottom: 0.5em;
        position: sticky;
        top: 0;       
        .nav-desktop {
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 2em;           
            
            .link-desktop {
                color: rgb(255, 255, 255);
                font-family: var(--FontOpenSans);
                font-weight: 500;
                text-shadow: 0 0 1px;
                padding: 0.5em;
                transition: color 0.3s ease-in-out, transform 0.3s ease-in-out, background-color 0.3s linear;
                border-radius: 0.4em;
            }

            .link-desktop:hover {
                color: rgb(160, 2, 63);
                transform: scale(1.5);
                border-radius: 0.5em;
                background-color: rgb(255, 255, 255);
            }
            .icon-mobile{
                padding-right: 0.3em;
            }
        }

        .img-title-desktop {
            width: 45%;
            display: flex;
            justify-content: center;
        }
    }

    .cont-title-header {
        .logo-wason-img {
            height: 60%;
        }
        transition: filter 0.3s linear;
    }    

    .icon-burger-mobile{
        display: none;
    }


       
}
//Animation burger-services-nav
.slide-in-top {
    -webkit-animation: slide-in-top 2s cubic-bezier(.25, .46, .45, .94) both;
    animation: slide-in-top .5s  0.5s cubic-bezier(.25, .46, .45, .94) both 
}


/* ----------------------------------------------
 * Generated by Animista on 2022-8-8 23:33:59
 * Licensed under FreeBSD License.
 * See http://animista.net/license for more info. 
 * w: http://animista.net, t: @cssanimista
 * ---------------------------------------------- */

@-webkit-keyframes slide-in-top {
    0% {
        -webkit-transform: translateY(-1000px);
        transform: translateY(-1000px);
        opacity: 0
    }

    100% {
        -webkit-transform: translateY(0);
        transform: translateY(0);
        opacity: 1
    }
}

@keyframes slide-in-top {
    0% {
        -webkit-transform: translateY(-1000px);
        transform: translateY(-1000px);
        opacity: 0
    }

    100% {
        -webkit-transform: translateY(0);
        transform: translateY(0);
        opacity: 1
    }
}
