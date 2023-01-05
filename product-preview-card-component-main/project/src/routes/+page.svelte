
<style>
    body {
        padding: 0;
        margin: 0;
        display: flex;
        justify-content: center;
        align-items: center;
        height: 100vh;
        font-family: "Montserrat";
        font-size: 14px;
        color: hsl(228, 12%, 48%);
        font-weight: normal;
        line-height: 1.5rem;
    }

    .card {
        display: flex;
        flex: 1;
        height: full;
        width: 60vw;
        background: white;
        border-radius: 10px;
        overflow: hidden;
        box-shadow: 2px 2px 8px 2px #6d6d6d18;
    }

    .content {
        flex: 1;
        display:flex;
        flex-direction: column;
        padding: 2rem;
        justify-content: space-between;
    }

    .preview {
        text-transform: uppercase;
        letter-spacing: 0.2rem;
        font-size: 0.8rem;
    }

    .image-desktop {
        flex:1;
        width: 50%;
        object-fit: cover;    

    }

    .image-mobile {
        display: none;
    }

    .prizes {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 1rem;
        padding-bottom: 1rem;
    }

    .small-prize {
        text-decoration: line-through;
        font-size: 0.9rem;
        font-weight: 500;
    }

    .title {
        font-family: 'fraunces';
        font-size: 2rem;
        color: black;
        line-height:2rem;
    }

    .big-prize {
        font-family: 'fraunces';
        font-size:2rem;
        color:hsl(158, 36%, 37%);
    }

    button {
        background:hsl(158, 36%, 37%);
        padding: 15px 10px;
        display: flex;
        gap: 1rem;
        justify-content: center;
        color: white;
        font-family: "montserrat";
        border: none;
        border-radius: 7px;
        font-weight: bold;
    }

    @media only screen and (max-width: 960px) {
        body {
            font-size: 12px;
        }
        .content {
            padding: 1.5rem;
        }
        .title {
            font-size: 1.7rem;
        }
        .big-prize {
            font-size: 1.7rem;
        }
        .small-prize {
            font-size: 0.7rem;
        }
        button {
            padding: 12px 8px;
        }
        .preview {
            font-size: 0.7rem;
        }
    }

    @media only screen and (max-width: 820px) {
        .card {
            flex-direction: column;
            max-width: 350px;
        }

        .image-desktop {
            display: none;
        }

        .image-mobile {
            display: block;
        }
    }
</style>

<body>
    <div class="card">
     
            <img class="image-desktop" src="/images/image-product-desktop.jpg" alt="Product">
            <img class="image-mobile" src="/images/image-product-mobile.jpg" alt="Product">
        
        <div class="content">
            <span class='preview'>Perfume</span>
  
            <span class='title'>Gabrielle Essence Eau De Parfum</span>
          
            <p>A floral, solar and voluptuous interpretation composed by Olivier Polge, 
            Perfumer-Creator for the House of CHANEL.</p>
          
            <div class='prizes'>
                <span class='big-prize'>$149.99</span>
                <span class='small-prize'>$169.99</span>
            </div>
                
            <button><img src="/images/icon-cart.svg" alt="cart-icon">Add to Cart</button>
            
        </div>
    </div>

  </body>