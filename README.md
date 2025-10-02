<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>myntra-online shopping</title>
    <link rel="stylesheet" href="styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css"> 
</head>
<body>
    <header>
        <img width="40px" height="40px" src="./img"alt="Myntra">
        <nav>
            <ul>
                <li><a href="#">Men</a></li>
                <li><a href="#">Women</a></li>
                <li><a href="#">Kids</a></li>
                <li><a href="#">Home & Living</a></li>
                <li><a href="#">Beauty</a></li>
            </ul>
            </nav>
            <div class="search-bar">
                <input type="text" placeholder="search for the products,brands and more">
                <button>Search</button>
            </div>
            <div class="icons">
              <span><i class="fa-regular fa-user"></i>Profile</span>  
              <span><i class="fa-regular fa-heart"></i>Wishlist</span>  
              <span><i class="fa-solid fa-bag-shopping"></i>Cart</span>  
            </div>
            </header>
            
             <section class="banner">
                <h2>Big Fashion Festival Sale!</h2>
                <p>up to 70% Off on Top Brands</p>
             </section>
            
             <main>
                <h2>Featured Products</h2>
                <div class="product-grid"> 

                     <div class="product">
                        <img src="./image"alt="product">
                        <h3>T-SHIRT</h3>
                        <p>&#8377;599</p>
                        <button onclick="addToCart('T-Shirt')"><i class="fa-solid fa-cart-plus"></i>Add To Cart</button>
                    </div>
                    <div class="product">
                        <img src="./jeans"alt="product">
                        <h3>JEANS</h3>
                        <p>&#8377; 1999</p>
                        <button onclick="addToCart('jeans')"><i class="fa-solid fa-cart-plus"></i>Add To Cart</button>
                    </div>
                    <div class="product">
                        <img src="./sneakers"alt="product">
                        <h3>SNEAKERS</h3>
                        <p>&#8377; 2999</p>
                        <button onclick="addToCart('sneakers')"><i class="fa-solid fa-cart-plus"></i>Add To Cart</button>
                    </div>
                </div>
                
             </main>
             <footer>
                <p> &copf; 2025 Myntra  | All Rights Reserved </p>
             </footer>
             <script src="./script.js"></script>
        </nav>
     </header> 
 </body>
</html>

css code

*{
    margin:0 ;
    padding: 0;
    box-sizing: border-box;
}
body{
    font-family: Arial, sans-serif;
    background: #f4f4f9;
    color: #333;
}
header{
    display: flex;
    justify-content:space-between ;
    align-items: center;
    background: white;
    padding: 15px 30px;
    box-shadow: 0 2px 5px rgba(0,0,0,0.1);
    position: sticky;
    top: 0;
    z-index: 1000;
}
nav ul{
    display: flex;
    list-style: none;
}
nav ul li{
    margin: 0 15px;
}
nav ul li a{
    text-decoration: none;
    color: #333;
    font-weight: bold;
}
.search-bar{
    display: flex;
    align-items: center;
}
.search-bar input{
    padding: 7px;
    border: 1px solid #ccc;
    border-radius: 4px;
}
.search-bar button{
    padding: 7px 10px;
    border:none ;
    background: #ff3f6c;
    color: white;
    margin-left: 5px;
    cursor: pointer;
    border-radius: 4px;
}
.icon span{
    margin-left:20px ;
    font-size: 14px;
}
.banner{
    text-align: center;
    background: #ff3f6c;
    color: whhite;
    padding: 50px 20px;
    margin-bottom: 20px;
}
.banner h2{
    font-size: 30px;
    margin-bottom: 10px;
}
main{
    padding: 20px;
}
main h2{
    text-align: center;
    margin-bottom: 20px;
}
.product-grid{
    display: grid;
    grid-template-columns: repeat(auto-fit,minmax(220px,1fr));
    gap: 20px;
}
.product{
    background: white;
    padding: 15px;
    border-radius: 8px;
    text-align: center;
    box-shadow: 0 2px 8px rgba(0,0,0,0.1);
}
.product img{
    max-width: 100%;
    border-radius: 8px;
    width: 100%;
    height: 300px;
    object-fit: contain;
}
.product button{
    margin-top: 10px;
    padding: 10px;
    background: #ff3f6c;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
}
.product button:hover {
background: #e12d56;
}
footer{
    text-align: center;
    padding: 15px;
    background: #222;
    color: white;
    margin-top: 20px;
}

java script

function addToCart(product){
    alert(product + " added to cart ");
}


